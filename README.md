# SharpShooters_MSTEST
Testing project for our banking system "Sharps Shooters"
In this project i have tested the methods:
ConvertCurrency()
CalculateTotalBorrowedAmount()
InitializeUser()

ConvertCurrency handles the operation of converting from USD to EURO or EURO to SEK for example. 
1. I began testing to see if it works as intended by just sending USD to an USD account.
2. I sent USD to EURO and the conversion rate of 0.93 worked as intended.
3. I sent USD to a currency that wasn´t implemented in the application and the conversion rate was 1.0 as it was the default in this method.
4. I sent a currency that was equal to null to Dinar that doesn´t exist and the rate was 1.0 here aswell.


CalculateTotalBorrowedAmount handles the operation of checking how much the user has borrowed in total.
1. I made three different loans to see if the total was correct.
2. I sent a null value to the method instead of a list to see if it threw an exception.
3. I made a negative transaction and there is no rule for negative amounts so the result was a loan of -100.


InitializeUser makes sure that each user is create in the system.
1. I check to see if there is as many users in the method as there are hard coded.
2. Testing if Theo is a user, if Theos pincode is 1111, if Theo has 3 accounts. Check if the account balance is equal to a number different from the actual balance (Test fails).

