# TestCase-Samples

Below are some Test Cases Samples that I wrote for my previous projects.

**Project 1-> https://demo.guru99.com/payment-gateway/purchasetoy.php**

_Title:_ Generate Card Number <br/>
_Test CaseID:_ TCG1 <br/>
_Pre-condintions:_ Chrome, Firefox, Edge available <br/>
_Post_conditions:_ - <br/>
_Test Priority:_ 1 <br/>
_Description/Summary:_ We want to generate a valid card number <br/>
_Test Steps:_ <br/> 
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php 
2. Go to Generate Card Number 


_Test Data:_ - <br/>
_Expected Result:_ We should get a valid card Number with CVV, expiration date, Credit Limit <br/>
_Actual Result:_ We receive a valid card number <br/>
_Status:_ PASS <br/>

___

_Title:_ We can make an order with the valid card number <br/>
_Test CaseID:_ TC1 <br/>
_Pre-condintions:_ <br/>
1. Chrome, Firefox, Edge available <br/>
2. We get a valid Card number from the first test case <br/>

_Post_conditions:_ - <br/>
_Test Priority:_ 1 <br/>
_Description/Summary:_ we should be able to complete an order <br/>
_Test Steps:_ <br/>
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php <br/>
2. Choose: Quantity 1 <br/>
3. Press Buy <br/>
4. Fill in all information for the card <br/>
5. Press Buy <br/>

_Test Data:_ Valid card number:  4683284279919555 ,CVV: 456 & Exp: 07/2025 <br/>
_Expected Result:_ We should receive Payment successfully and an Order ID <br/>
_Actual Result:_ We receive Payment successfully and an Order ID <br/>
_Status:_ PASS <br/>

___

_Title:_ We should not be able to  make an order with an invalid card number <br/>
_Test CaseID:_ TC2 <br/>
_Pre-condintions:_ Chrome, Firefox, Edge available <br/>
_Post_conditions:_ - <br/>
_Test Priority:_ 1 <br/>
_Description/Summary:_ We should not be able to complete an order <br/>
_Test Steps:_ <br/>
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php <br/>
2. Choose: Quantity 1 <br/>
3. Press Buy <br/>
4. Fill all information for card (invalid card) <br/>
5. Press Buy <br/>

_Test Data:_ Invalid card: 1234567891234567,CVV: 456 & Exp: 07/2025 <br/>
_Expected Result:_ We should receive an error message <br/>
_Actual Result:_ Receive Payment successfully and an Order ID <br/>
_Status:_ FAILED <br/>

___

_Title:_ Pressing back button after purchase <br/>
_Test CaseID:_ TB1 <br/>
_Pre-condintions:_ Chrome, Firefox, Edge available <br/>
_Post_conditions:_ - <br/>
_Test Priority:_ 1 <br/>
_Description/Summary:_ After we purchased the product we shouldn’t be able  to return to the page with the card details by pressing the back button <br/>
_Test Steps:_ <br/>
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php 
2. Choose: Quantity 1
3. Press Buy
4. Fill all information for card (invalid card)
5. Press Buy
6. Press back button

_Test Data:_ Valid card number:  4683284279919555 ,CVV: 456 & Exp: 07/2025 <br/>
_Expected Result:_ We should receive an error message <br/>
_Actual Result:_ We can go back to the purchase page which contains the card details <br/>
_Status:_ FAILED <br/>

___

_Title:_ Website/webpage responsive on other devices <br/>
_Test CaseID:_ TR1 <br/>
_Pre-condintions:_ Chrome, Firefox, Edge available <br/>
_Post_conditions:_ - <br/>
_Test Priority:_ 3 <br/>
_Description/Summary:_ the website/web page should be responsive on the devices shown in the developer tools <br/>
_Test Steps:_ <br/>
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Go to More tools-developer tools
3. Dimension: Responsive

_Test Data:_ - <br/>
_Expected Result:_ Should be responsive in all devices shown in the developer tool <br/>
_Actual Result:_The menu bar doesn’t appear on all the devices <br/>
_Status:_ FAILED <br/>

___

_Title:_ Modify source code <br/>
_Test CaseID:_ MC3 <br/>
_Pre-condintions:_ Chrome, Firefox, Edge available <br/>
_Post_conditions:_ - <br/>
_Test Priority:_ 1 <br/>
_Description/Summary:_ We should not be able to complete an order with a quantity with a negative value. This value is modified in the code source to a negative value. <br/>
_Test Steps:_ <br/>
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Choose: Quantity -15
3. Press Buy
4. Fill in all information for the card
5. Press Buy

_Test Data:_ Valid card number:  4683284279919555, CVV: 456 & Exp: 07/2025 <br/>
_Expected Result:_ We should receive an error message <br/>
_Actual Result:_ Receive Payment successfully and an Order ID <br/>
_Status:_ FAILED 
 





