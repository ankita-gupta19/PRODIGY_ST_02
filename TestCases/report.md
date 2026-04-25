**Test Case ID: TC_01**

**Title:**
Verify homepage loads successfully across browsers

**Precondition:**
Internet connection available

**Steps:**
1. Open browser
2. Enter URL [(https://shoplane-by-lassie.netlify.app)]
3. Press Enter

**Browsers Tested:**
- Chrome
- Firefox
- Edge

**Expected Result:**
Homepage should load correctly in all browsers without UI issues or functional errors

**Actual Result:**
Homepage loads in all tested browsers, but UI and functional issues are observed:
- Layout breaks on mobile (product cards overlap)
- Search functionality is not working
- Cart icon is not responsive
**Status:**
Fail
**Recommendations:**
- Fix CSS for responsiveness
- Add search validation
- Improve button click handling


**Test Case ID: TC_02**

**Title:**
Verify logo click redirects to homepage

**Precondition:**
User is on any page of the website

**Steps:**
1. Open website [(https://shoplane-by-lassie.netlify.app)]
2. Navigate to any page (if not already on homepage)
3. Click on the website logo

**Expected Result:**
User should be redirected to the homepage

**Actual Result:**
Logo is not clickable on some pages and does not redirect to homepage as expected

**Status:**
 Fail

**Issues Found:**
1. Website logo is not clickable on some pages
2. In some cases, logo click does not redirect to homepage
3. Navigation inconsistency observed when interacting with logo

**Recommendations:**
- Ensure logo has proper anchor tag (<a href="/">)
- Fix click event handling for logo
- Add consistent redirection logic across all pages
- Test logo functionality across all browsers and devices

**Test Case ID: TC_03**

**Title:**
Verify navigation menu links redirect to correct category pages

**Precondition:**
User is on the website and navigation menu is visible

**Steps:**
1. Open website [(https://shoplane-by-lassie.netlify.app)]
2. Observe the navigation menu (e.g., Men, Women, Accessories, etc.)
3. Click on any category from the navigation menu
4. Repeat for all available categories
   
**Expected Result:**

User should be redirected to the selected category page with relevant products displayed

**Actual Result:**
Some navigation menu links do not redirect correctly or load incorrect/empty pages

**Status:**
Fail

**Issues Found:**

Certain category links are not clickable
Some links redirect to incorrect pages
Inconsistent behavior across different categories
Page content does not match selected category

**Recommendations:**

Ensure all navigation links have correct routing paths
Validate category-page mapping in frontend/backend
Fix broken or inactive links
Test navigation across all devices and browsers
Add validation to ensure correct products load per category

**Test Case ID: TC_04**

**Title:**
Verify homepage banner click redirects to the correct page

**Precondition:**
User is on the homepage and banner is visible

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Locate the homepage banner
3. Click on the banner image or CTA button
4. Observe the redirection behavior

**Expected Result:**
User should be redirected to the relevant product or category page associated with the banner

**Actual Result:**
User is successfully redirected to the correct product/category page after clicking the banner

**Status:**
Pass

**Issues Found:**
No issues found. Banner is working as expected.

**Recommendations:**
No changes required. Functionality is working correctly.

**Test Case ID: TC_05**

**Title:**
Verify website layout adjusts properly on mobile devices (Responsive Design)

**Precondition:**
User has access to the website and can switch to mobile view (using browser DevTools or mobile device)

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Open browser Developer Tools
3. Enable mobile view (e.g., iPhone, Android)
4. Refresh the page
5. Observe layout, images, text, and navigation

**Expected Result:**
Website layout should adjust properly to mobile screen size with no overlapping, proper alignment, and readable content

**Actual Result:**
Website layout adjusts correctly for mobile screens; elements are properly aligned and responsive

**Status:**
Pass

**Issues Found:**
No issues found. Website is responsive and works well on mobile devices

**Recommendations:**
No changes required. Responsive design is functioning correctly

**Test Case ID: TC_06**

**Title:**
Verify user can successfully register with valid details

**Precondition:**
User is on the registration/sign-up page

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Navigate to the registration/sign-up page
3. Enter valid user details (e.g., name, email, password)
4. Click on the “Register” or “Sign Up” button
5. Observe the response

**Expected Result:**
User account should be created successfully and user should be redirected to the login or homepage

**Actual Result:**
User is successfully registered and redirected to the appropriate page

**Status:**
Pass

**Issues Found:**
No issues found. Registration process is working correctly

**Recommendations:**
No changes required. Functionality is working as expected

**Test Case ID: TC_07**

**Title:**
Verify system shows error message for invalid email format

**Precondition:**
User is on a page where email input is required (e.g., signup, login, or checkout form)

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Navigate to a form that requires email input
3. Enter an invalid email (e.g., "abc123" or "user@")
4. Click submit or move to next field
5. Observe system response

**Expected Result:**
System should display an error message indicating invalid email format and prevent submission

**Actual Result:**
System does not show any error message and accepts invalid email input

**Status:**
Fail

**Issues Found:**

* Invalid email formats are accepted
* No validation message is displayed
* Form submission is not restricted

**Recommendations:**

* Implement email format validation using regex
* Display clear error message (e.g., "Enter a valid email address")
* Prevent form submission until valid email is entered
* Test validation across different browsers and devices

**Test Case ID: TC_08**

**Title:**
Verify user can log in with valid credentials

**Precondition:**
User is registered on the website and login page is accessible

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Navigate to the login page
3. Enter valid email/username
4. Enter correct password
5. Click on the login button

**Expected Result:**
User should be successfully logged in and redirected to the homepage or dashboard

**Actual Result:**
User is successfully logged in and redirected to the homepage

**Status:**
Pass

**Issues Found:**
No issues found. Login functionality is working correctly

**Recommendations:**
No changes required. Login system is functioning as expected

**Test Case ID: TC_09**

**Title:**
Verify user cannot log in with empty fields

**Precondition:**
User is registered on the website and login page is accessible

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Navigate to the login page
3. Enter valid email/username
4. Enter correct password
5. Click on the login button

**Expected Result:**
User should be successfully logged in and redirected to the homepage or dashboard

**Actual Result:**
User is successfully logged in and redirected to the homepage

**Status:**
Pass

**Issues Found:**
No issues found. Login functionality is working correctly

**Recommendations:**
No changes required. Login system is functioning as expected

***Test Case ID: TC_10****

**Title:**
Verify error message is displayed when user logs in with incorrect password

**Precondition:**
User is on the login page and has a valid registered account

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Navigate to login page
3. Enter valid username/email
4. Enter incorrect password
5. Click on login button

**Expected Result:**
System should display an error message indicating incorrect password and prevent login

**Actual Result:**
Error message is displayed and user is not allowed to log in with incorrect password

**Status:**
Pass

**Issues Found:**
No issues found. Error handling works correctly

**Recommendations:**
No changes required. Validation is working as expected

***Test Case ID: TC_11****

**Title:**
Verify user is successfully logged out from the application

**Precondition:**
User is logged into the website

**Steps:**

1. Open website [(https://e-shoplane.netlify.app)]
2. Ensure user is logged in
3. Click on logout button
4. Observe system behavior

**Expected Result:**
User session should end and user should be redirected to login or homepage

**Actual Result:**
User is successfully logged out and redirected appropriately

**Status:**
Pass

**Issues Found:**
No issues found. Logout functionality works correctly

**Recommendations:**
No changes required. Feature is functioning properly

***Test Case ID: TC_12****

**Title:**
Verify product search functionality returns relevant results

**Precondition:**
User is on the homepage and search bar is visible

**Steps:**

Open website [(https://e-shoplane.netlify.app)]
Locate the search bar
Enter a product keyword (e.g., "shirt")
Press Enter or click search icon

**Expected Result:**
Relevant products related to the search keyword should be displayed

**Actual Result:**
Search functionality is not working and no results are displayed

**Status:**
Fail

**Issues Found:**

Search feature is non-functional
No results displayed
No error or feedback shown

**Recommendations:**

Implement search logic/API
Display “No results found” message if applicable
Add input validation and suggestions

***Test Case ID: TC_13****

**Title:**
Verify product details page displays correct information

**Precondition:**
User is on product listing page

**Steps:**

Open website [(https://e-shoplane.netlify.app)]
Navigate to any product category
Click on any product

**Expected Result:**
Product detail page should display name, image, price, description

**Actual Result:**
Product details are displayed correctly

**Status:**
Pass

**Issues Found:**
No issues found

**Recommendations:**
No changes required

***Test Case ID: TC_14****

**Title:**
Verify “Add to Cart” functionality

**Precondition:**
User is on product details page

**Steps:**

Open website [(https://e-shoplane.netlify.app)]
Select a product
Click “Add to Cart”

**Expected Result:**
Product should be added to cart and reflected in cart icon

**Actual Result:**
Product is added but cart icon is not updating properly

**Status:**
Fail

**Issues Found:**

Cart icon not updating
No confirmation message

**Recommendations:**

Update cart count dynamically
Show success message

***Test Case ID: TC_15****

Verify payment process functionality

**Precondition:**
User is on checkout page

**Steps:**

Enter payment details
Click on pay/confirm

**Expected Result:**
Payment should be processed successfully

**Actual Result:**
Payment functionality is not fully implemented / fails

**Status:**
Fail

**Issues Found:**

Payment gateway not integrated
No success/failure feedback

**Recommendations:**

Integrate payment gateway (Razorpay/Stripe)
Add proper success/failure handling

***Test Case ID: TC_16****

**Title:**
Verify order confirmation after successful checkout

**Precondition:**
Payment is completed

**Steps:**

Complete checkout process
Observe confirmation page

**Expected Result:**
Order confirmation message with details should be displayed

**Actual Result:**
No proper confirmation message displayed

**Status:**
Fail

**Issues Found:**

Missing confirmation page
No order summary

**Recommendations:**

Add order confirmation page
Display order ID and details