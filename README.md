# TestCase-Samples

Below are some Test Cases Samples that I wrote for my previous projects.

**Project 1-> https://demo.guru99.com/payment-gateway/purchasetoy.php**

_Title:_ Generate Card Number <br/>
_Test CaseID:_ TCG1 <br/>
_Pre-condintions:_ Chrome, Firefox, Edge available <br/>
_Post_conditions:_ - <br/>
_Test Priority:_ 1 <br/>
_Description/Summary:_We want to generate a valid card number
_Test Steps:_
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Go to Generate Card Number

_Test Data:_-
_Expected Result:_We should get a valid card Number with CVV, expiration date, Credit Limit
_Actual Result:_We receive a valid card number
_Status:_PASS

___

_Title:_We can make an order with the valid card number 
_Test CaseID:_TC1
_Pre-condintions:_
1. Chrome, Firefox, Edge available
2. We get a valid Card number from the first test case
_Post_conditions:_-
_Test Priority:_1
_Description/Summary:_we should be able to complete an order
_Test Steps:_
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Choose: Quantity 1
3. Press Buy
4. Fill in all information for the card
5. Press Buy
_Test Data:_ Valid card number:  4683284279919555 ,CVV: 456 & Exp: 07/2025
_Expected Result:_We should receive Payment successfully and an Order ID
_Actual Result:_We receive Payment successfully and an Order ID
_Status:_PASS

___

_Title:_We should not be able to  make an order with invalid card number
_Test CaseID:_TC2
_Pre-condintions:_Chrome, Firefox, Edge available
_Post_conditions:_-
_Test Priority:_1
_Description/Summary:_We should not be able to complete an order
_Test Steps:_
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Choose: Quantity 1
3. Press Buy
4. Fill all information for card (invalid card)
5. Press Buy
_Test Data:_Invalid card: 1234567891234567,CVV: 456 & Exp: 07/2025
_Expected Result:_We should receive an error message
_Actual Result:_Receive Payment successfully and an Order ID
_Status:_FAILED

___

_Title:_ Pressing back button after purchase
_Test CaseID:_TB1
_Pre-condintions:_Chrome, Firefox, Edge available
_Post_conditions:_-
_Test Priority:_1
_Description/Summary:_After we purchased the product we shouldn’t be able  to return to the page with the card details by pressing the back button
_Test Steps:_
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Choose: Quantity 1
3. Press Buy
4. Fill all information for card (invalid card)
5. Press Buy
6. Press back button
_Test Data:_Valid card number:  4683284279919555 ,CVV: 456 & Exp: 07/2025
_Expected Result:_We should receive an error message
_Actual Result:_We can go back to the purchase page which contains the card details
_Status:_FAILED

___

_Title:_Website/webpage responsive on other devices
_Test CaseID:_TR1
_Pre-condintions:_Chrome, Firefox, Edge available
_Post_conditions:_-
_Test Priority:_3
_Description/Summary:_the website/web page should be responsive on the devices shown in the developer tools
_Test Steps:_
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Go to More tools-developer tools
3. Dimension: Responsive
_Test Data:_-
_Expected Result:_Should be responsive in all devices shown in the developer tool
_Actual Result:_The menu bar doesn’t appear on all the devices
_Status:_FAILED

___

_Title:_Modify source code
_Test CaseID:_MC3
_Pre-condintions:_Chrome, Firefox, Edge available
_Post_conditions:_-
_Test Priority:_1
_Description/Summary:_We should not be able to complete an order with a quantity with a negative value. This value is modified in the code source to a negative value.
_Test Steps:_
1. Open https://demo.guru99.com/payment-gateway/purchasetoy.php
2. Choose: Quantity -15
3. Press Buy
4. Fill in all information for the card
5. Press Buy
_Test Data:_ Valid card number:  4683284279919555, CVV: 456 & Exp: 07/2025
_Expected Result:_We should receive an error message
_Actual Result:_Receive Payment successfully and an Order ID
_Status:_ FAILED






