# Juice Shope: View Basket  Writeup 

## Challenge Overview  
Title: View Basket
Difficulty: 2/6  
Category: Broken Access Control  
Description: View another user's shopping basket.  
## Tools Used:  
1. Web Browser: To nevigate shopping basket.  
2. BurpSuite: To Intersept and Manipulate Requests to view another user basket.

## Methodology and Solution

### Step 1: capture basket request.  
First of all, I access my basket and capture that request in Burpsuite.  
![My Images](../Images/Basket1.png) 

### Step 2: Change the ID  
Now when I look at the capture request I found that website using user IDs to access user basket. Then, I simply change the ID. Mine was 6 I change it to 5.  
![My Images](../Images/Basket2.png)  

And Done.... 
