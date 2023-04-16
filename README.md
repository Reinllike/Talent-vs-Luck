# Talent-vs-Luck
A reproduction of 'Talent vs Luck' in my way

https://arxiv.org/abs/1802.07068  
A. Pluchino. A. E. Biondo, A. Rapisarda: Talent vs Luck: the role of randomness in success and failure[J].arXiv preprint arXiv:1802.07068

## Rules
### Basic Rules 
1.Set (N_people) to 1000, each with a different gift value(gift).  
2.The gift values(gift) are distributed according to a normal distribution with a mean of 0.6 and a variance of 0.1. Values greater than 0.9 are set to 0.9, and values less than 0.3 are set to 0.3.  
3.Each person has 80 life periods(life_period) and encounters good luck, bad luck, or nothing each time at random.  
4.Set a value(luck_threshold) to represent the probability of good and bad luck occurrence respectively (e.g., luck_threshold = 0.1 represents 10% chance of bad luck, 10% chance of good luck, and 80% chance of no luck).  
5.The gift value affects the chance of grasping good luck (e.g., a gift value of 0.8 gives an 80% chance of grasping good luck).  
6.Each person starts with 10 dollars.  
7.If good luck is grasped, the property is multiplied by 2; if bad luck occurs, the property is halved.  

![1-3_Resize Image](https://user-images.githubusercontent.com/77602608/232327305-45ca34df-396e-4112-b208-913f0947d62e.png)

### Other Adjust

## Experiments
### Introduce 
N_People = 1000  
life_period = 80  
luck_threshold = 0.1

![download](https://user-images.githubusercontent.com/77602608/232327992-a7772eda-4255-4982-a938-03e606257196.png)  
(The figure shows the distribution of gift values among all individuals.)  

life_advance = the distribution of good and bad luck throughout each person's life, with values greater than 0.9 indicating good luck and values less than 0.1 indicating bad luck.  
property1 = the amount of property held by each person after completing their life.  
luck = the combination of each person's gift value and the number of times they encounter good or bad luck throughout their life.  
luck[rich] = the life of the person with the highest amount of property.  

## Scenario1 (Basic Rules)

![download](https://user-images.githubusercontent.com/77602608/232328186-e9352d48-035f-4bbe-8a76-a810a990bd0f.png)  
(The figure shows the correlation between gift values and property1 for all individuals.)  

### RepeatedlyTest
Pick out the gift and properties of the richest person in each test.

Repeat 1000 times with different luck thresholds (0.1 and 0.05), and the resulting means were 0.6973 and 0.6737, respectively.  

![download](https://user-images.githubusercontent.com/77602608/232333071-76c7b559-7f08-4c7e-919c-d8d2ea238135.png)
![download](https://user-images.githubusercontent.com/77602608/232332819-1d80e7cd-1a18-41bc-a80f-c79283911e3a.png)  

The first obtained score(mean) is significantly higher than which was reported in the original paper(0.667).  
When I set luck_threshold from 0.1 to 0.05 ,the number dropped from 0.6973 to 0.6737.  
__So ,luck_threshold play an important role in it.__




## Result

__So ,luck_threshold play an important role in it.__
