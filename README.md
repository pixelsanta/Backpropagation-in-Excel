# Backpropagation-in-Excel
This is the backpropagation of a very simple neural network in Excel to get the hang of Backprop and learning rates




Backpropagation Differentiation
∂E_t/∂w5 = ∂E1/∂a_o1 * ∂a_o1/∂o1 * ∂o1/∂w5 = (a_o1-t1)*a_o1*(1-a_o1)*a_h1
∂E_t/∂w6 = ∂E1/∂a_o1 * ∂a_o1/∂o1 * ∂o1/∂w6 = (a_o1-t1)*a_o1*(1-a_o1)*a_h2
∂E_t/∂w7 = ∂E2/∂a_o2 * ∂a_o2/∂o2 * ∂o2/∂w7 = (a_o2-t2)*a_o2*(1-a_o2)*a_h1
∂E_t/∂w8 = ∂E2/∂a_o2 * ∂a_o2/∂o2 * ∂o2/∂w8 = (a_o2-t2)*a_o2*(1-a_o2)*a_h2

∂E_t/∂a_h1 = (∂E1+∂E2)/∂a_h1 = ∂E1/∂a_o1 * ∂a_o1/∂o1 * ∂o1/∂a_h1 + ∂E2/∂a_o2 * ∂a_o2/∂o2 * ∂o2/∂a_h1 = (a_o1-t1)*a_o1*(1-a_o1)w5 + (a_o2-t2)*a_o2*(1-a_o2)w7
∂E_t/∂a_h2 = (∂E1+∂E2)/∂a_h2 = ∂E1/∂a_o1 * ∂a_o1/∂o1 * ∂o1/∂a_h2 + ∂E2/∂a_o2 * ∂a_o2/∂o2 * ∂o2/∂a_h1 = (a_o1-t1)*a_o1*(1-a_o1)w6 + (a_o2-t2)*a_o2*(1-a_o2)w8

∂E_t/∂w1 = ∂(E1+E2)/∂w1 = ∂(E1+E2)/a_h1 * ∂a_h1/∂h1 * ∂h1/∂w1 = ((a_o1-t1)*a_o1*(1-a_o1)w5 + (a_o2-t2)*a_o2*(1-a_o2)w7)*a_h1*(1-a_h1)*i1
∂E_t/∂w2 = ∂(E1+E2)/∂w2 = ∂(E1+E2)/a_h1 * ∂a_h1/∂h1 * ∂h1/∂w2 = ((a_o1-t1)*a_o1*(1-a_o1)w5 + (a_o2-t2)*a_o2*(1-a_o2)w7)*a_h1*(1-a_h1)*i2
∂E_t/∂w3 = ∂(E1+E2)/∂w3 = ∂(E1+E2)/a_h2 * ∂a_h2/∂h2 * ∂h2/∂w3 = ((a_o1-t1)*a_o1*(1-a_o1)w6 + (a_o2-t2)*a_o2*(1-a_o2)w8)*a_h2*(1-a_h2)*i1
∂E_t/∂w4 = ∂(E1+E2)/∂w4 = ∂(E1+E2)/a_h2 * ∂a_h2/∂h2 * ∂h2/∂w4 = ((a_o1-t1)*a_o1*(1-a_o1)w6 + (a_o2-t2)*a_o2*(1-a_o2)w8)*a_h2*(1-a_h2)*i2



Screenshots

Learning Rate 1
![image](https://user-images.githubusercontent.com/91488625/137532072-a372933e-1ddf-4f88-9b5f-9cad49ed23e0.png)


Learning Rate 2
![image](https://user-images.githubusercontent.com/91488625/137532140-3d7ef790-3e49-47dc-a563-3a1628deac74.png)


Learning Rate 3
![image](https://user-images.githubusercontent.com/91488625/137532160-ee7f2c75-7828-4b70-b837-ba938ed0ee51.png)


Learning Rate 4
![image](https://user-images.githubusercontent.com/91488625/137532190-21b8e6a2-b6ed-4100-aafa-aaba336bf3b8.png)


Learning Rate 5
![image](https://user-images.githubusercontent.com/91488625/137532216-c6a9536d-4549-4b79-bf14-c523b44a914b.png)


Learning Rate 6
![image](https://user-images.githubusercontent.com/91488625/137532253-32a59a60-dce9-44c0-92e6-a5f7cb102b8b.png)
