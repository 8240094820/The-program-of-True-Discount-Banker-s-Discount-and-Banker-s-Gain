# The-program-of-True-Discount-Banker-s-Discount-and-Banker-s-Gain
------------------------------------------------------------------------------------------------------------------------------------------------------
#The program of True Discount, Banker's Discount and Banker's Gain...
#1. Enter the amount of goods
#2. Enter the interest rate
#3. enter the time period
A=int(input("Enter the amount of goods: "))
R=int(input("Enter the rate: "))
T=int(input("Enter the time: "))

#4. SI= Simple Interest
SI= A*(R/100)*(T/12)
Si=A+SI
print("Buyer's have to pay after",T,"month rupees",Si)

#5. After which month you need the money
#6. TD= True Discount
t= int(input("type the month when you Discount: "))
d=A*(R/100)*(t/12)
D=d+A
TD= Si-D
print("True Discount after",t,"month:%.2f "%TD)

#7. Calculating the Banker's Discount(BD) with the help of Remaining monthes & Simple interest amount.
Time=T-t
BD=Si*(R/100)*(Time/12)
print("The Banker's Discount is:%.2f "%BD)

#8. Calculate the Banker's Gain with the help of BD & TD
BG=BD-TD
print("The Banker's Gain is:%.2f "%BG)

#9. The amount which will get the seller for the month when his/her need.
Customer_amount=Si-BD
print("Now customer will get rupees :%.2f"%Customer_amount)
