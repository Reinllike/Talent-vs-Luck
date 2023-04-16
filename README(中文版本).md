# Talent-vs-Luck
A reproduction of 'Talent vs Luck' in my way

https://arxiv.org/abs/1802.07068  
A. Pluchino. A. E. Biondo, A. Rapisarda: Talent vs Luck: the role of randomness in success and failure[J].arXiv preprint arXiv:1802.07068

## Rules
### Basic Concept 
1.設定一千人(N_people)，各自擁有不同的才能值(gift)。  
2.才能(gift)依照常態分佈去分配，平均值為0.6，變異數為0.1，大於0.9為0.9，小於0.3為0.3。  
3.每個人有八十個人生週期(life_period)，每次隨機遇到好運、壞運或者無事發生。  
4.才能值影響把握住好運的機會(才能為0.8則把握住好運的機會為80%)。  
5.好運發生且把握住時，資產*2；壞運發生時，資產必定/2。  

![1-3_Resize Image](https://user-images.githubusercontent.com/77602608/232327305-45ca34df-396e-4112-b208-913f0947d62e.png)

### Other Adjust

## Experiments
### Introduce & Scenario1(Basic Concept)
N_People = 1000  
life_period = 80  

(下圖為所有人的才能分配  
![download](https://user-images.githubusercontent.com/77602608/232327992-a7772eda-4255-4982-a938-03e606257196.png)  
life_advance = 所有人一生的好壞運分配，大於0.9視為遇到好運，小於0.1視為遇到壞運  
property1 = 所有人一生過完後分別的資產量  

(下圖為所有人的才能與資產量的對應  
![download](https://user-images.githubusercontent.com/77602608/232328186-e9352d48-035f-4bbe-8a76-a810a990bd0f.png)  

luck = 所有人的才能值和一生中遇到多少次好運壞運  
luck[rich] = 擁有最多資產的人的一生  
