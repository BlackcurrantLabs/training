# Test Cases Examples : Qafox.com

QaFox is a sample E-commerce website with a slightly complex layout and yet similar to that of typical online shopping platforms. It features a semi-formal design and includes several unique components, making it suitable for practicing and testing various web application functionalities.


**Website:** [ QAFox E-Commerce Website](https://tutorialsninja.com/demo/)

# Home Page


## Qafox Logo

| Test Case | Status | Defects |
|---|---|---|
| Verify that the logo highlights on hover. | PASS | N/A |
| Verify that the logo redirects to home page on click properly. | PASS | N/A |

## Navigation Bar

| Test Case | Status | Defects |
|---|---|---|
| Verify that the 'Currency' dropdown highlights and functions properly. | PASS | N/A |
| Verify that the 'Contact us' highlights and redirects to 'contact' webpage | FAIL | Number in 'Contact us' doesn't highlights when hover and isn't assessible. Only icon is accessible |
| Verify that the 'My Account' drop down highlights and accurately displays Hyperlinks for 'Login' and 'Register' page | PASS | N/A |
| Verify that the 'wishlist' hyperlink highlights and redirects to wishlist page | PASS | N/A |
| Verify that the 'wishlist' hyperlink displays the number of products wishlisted everytime a product is added to the wishlist | PASS | N/A |
| Verify that the 'Shopping cart' hyperlink highlights and redirects to Shopping cart page properly | PASS |  N/A |
| Verify that the 'Checkout' hyperlink highlights and redirects to Checkout page properly | FAIL | Checkout hyperlink redirects to Shopping cart page instead of Checkout page |
| Verify that the Wishlist count remains constant when tabs are switched using browser's nav buttons | FAIL | The content abruptly changes whenever back button from browser's navigations  is used - Wishlist goes back to it's prior state when back button is clicked, regardless of what content is contains currently |

## Search Bar and button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Search Bar highlights and is accessible. | PASS | N/A |
| Verify that the search Bar button functionalities functions accurately.  | FAIL | Button gives search result, even without any input in the search bar |
| Verify that products searched in search bar are visible in product page. | PASS | N/A |

## Cart button and Pop-up

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Cart button is visible and accessible properly | PASS | N/A |
| Verify that the Cart contents remains constant when tabs are switched using browser's nav buttons | FAIL | The content abruptly changes whenever back button from browser's navigations  is used - Cart goes back to it's prior state when back button is clicked, regardless of what content is contains currently |
| Verify that the cart ubttons displayed Pop up with 'Cart empty' message when no items have been carted  | PASS | N/A |
| Verify that the Cart button displays the number and total price of items, everytime an item is carted accurately. | PASS | N/A |
| Verify that the Cart button displays accurate prices when the currency are swaped from currency drop-down list. | FAIL | Prices aren't accurate when currency are swapped.  (Depends on Real time; Could be an exception) |
| Verify that the pop-up is displayed everytime the button is cicked | PASS | N/A |
| Verify that the Product image is displayed for each item carted in cart popup | PASS  | N/A |
| Verify that the product name is displayed in hyper link for each item carted in cart popup | PASS | N/A |
| Veriy that the product name hyperlink redirects to the product information page for each product carted in cart popup | PASS | N/A |
| Verify that the product count is displayed for individual products in cart popup | PASS | N/A |
| Verify that the individual product price is displayed in cart popup | PASS | N/A |
| Verify that the Cross / delete product button is visible and accessible in cart popup | PASS | N/A |
| Verify that item is deleted from the cart when Delete item button is clicked in cart popup | PASS | N/A |
| Verify that the total price (Sub-total price ) of selected / carted item is visible and accurate | PASS | N/A |
| Verify that the Tax (Eco tax) based on all selected Items are displayed and accurate in cart popup | FAIL | Typo error. - Eco TAX (-2.00)   => Minus symbol instead of Plus symbol |
| Verify that the VAT tax with percentage is displayed and is accurately in cart popup | PASS | N/A |
| Verify that the sum total price of all the prices + taxes is accurately and clearly displayed in cart popup | FAIL | Presents incorrect values in total sumup |
| Verify that the currency change is accurately displayed with accurate prices as per currency | FAIL (Improvement) | The conversion of sum total have a very slight error. Example:  If 123.20 USD equals:  75.46 Pounds 96.66 Euros...  then..  848.40 USD would be 519.49 Pounds Sterling and 665.29 Euros  However... it shows 519.65 in Pound Sterling and 665.65 in Euroes |
| Verify that the View cart / checkout hyperlinks are visible and accurately redirects to view cart and checkout page respectively when clicked in cart popup | PASS | N/A |
| Verify that the details in cart pop up, displayed for both guest user and loggedin user is accurate and similar  | FAIL | The pop up doesn't shows Tax, INV etc values for the logged in user |

## Product Navigation Bar

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product nav bar is visible and accessible. | PASS | N/A |
| Verify that the product nav bar accurectly displays product tabs / dropdowns on hover | FAIL | Dropdowns on tabs aren't visible and accessible. :   - Tablets - Softwares - Phones and PDAs - Cameras  |
| Verify that the product nav bar displays categorized products on click | FAIL  | Products for tabs aren't displayed on-click :   - Desktop - Laptops - Components  - MP3 Players |
| Verify that the tabs drop drop-down lists of product navbar, displays the categorized products on Product page section when clicked on specific product category from the list | FAIL | - Doesn't Displays available MP3s in dropdowns |
| Verify that the 'show all products ' hyperlnk within DropDown of product nav bar is clearly visible and accurately displays the related products  | FAIL | Show All Products ' hyperlink has a typo error, there is no Space between 'show all' and the product name . - Ex: 'Show AllCamera' instead of 'Show All Cameras'  |

## Carousel (products)

| Test Case | Status | Defects |
|---|---|---|
| Verify that the carousel sldier is visible and accessible  | PASS | N/A |
| Verify that the caruosel slider displays floating arrows points left / right when hover. | PASS | N/A |
| Verify that the caruosel slider slides according to arrows clicked | PASS | N/A |
| Verify that the caruosel sldier slides by cursor drag towards left or right | PASS | N/A |
| Verify that the carousel slider includes pin-point buttons to illustrate slide numbers and navigate among slides | PASS | N/A |
| Verify that the carousel sldier 's images redirect to displayed product on click. | FAIL | Second image isn't responsive. |

## Product page (Featured Products)

| Test Case | Status | Defects |
|---|---|---|
| Verify that the featured products are visible and accessible | PASS | N/A |
| Verify that the product image redirects to product details page when clicked upon. | PASS | N/A |
| Verify that the featured products includes product details - Product image - Product Name - Product descriptions - Product individual price - Product individual excluding tax price  | PASS | N/A |
| Verify that the 'add to cart ' button visible and accessible for all featured items | PASS | N/A |
| Verify that the 'add to cart' button carts the item when clicked | FAIL | Some items redirects to Product detail page instead of adding to the cart - Apple Cinema 30" - Canon EOS 5D |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist ' button visible and accessible for all featured items | PASS | N/A |
| Verify that the 'add to  Wishlist' button add the item to wishlist when clicked | pASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'add to Compare product' button visible and accessible for all featured items | PASS | N/A |
| Verify that the 'add to Compare product' button add the item to compare products when clicked | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |

## Carousel (brands)

| Test Case | Status | Defects |
|---|---|---|
| Verify that the carousel sldier is visible and accessible  | PASS | N/A |
| Verify that the caruosel slider displays floating arrows points left / right when hover. | PASS | N/A |
| Verify that the caruosel slider slides according to arrows clicked | PASS | N/A |
| Verify that the caruosel slider slides by cursor drag towards left or right | PASS | N/A |
| Verify that the carousel slider includes pin-point buttons to illustrate slide numbers and navigate among slides | PASS | N/A |

# Login Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the login hyperlinks from Navigation bar functions properly | PASS | N/A |
| Verify that the Login form is visible  | PASS | N/A |
| Verify that the Login form heading label is visible | PASS | N/A |
| Verify that the E-mail and password labels are precisely visible | PASS | N/A |

## TextFields

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Textfields of Email and Password are visible and accessible | PASS | N/A |
| Verify that the placeholders for Email and Password are visible and accurate | PASS | N/A |
| Verify that the TextField accepts inputs: - Text  - Numbers - SpecialCharacters | PASS | N/A |
| Verify that the password inputs are encrypted on screen | PASS | N/A |
| Verify that the Autofill functionality properly works for previously logged in users  | PASS | N/A |

## Form

| Test Case | Status | Defects |
|---|---|---|
| Verify that the form restricts unregistered users to log-in without proper credentials | PASS | N/A |
| Verify that the form displays error message if credentials of Email is invalid / incorrect | PASS | Improvement: There should be different messages for Empty textfield errors and invalid credentials error |
| Verify that the form displays error message if credentials of Password is invalid / incorrect | PASS |  |
| Verify that the form displays error message if empty Textfields are submitted | PASS |  |

## Submit Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the submit button is visible clearly and accessible  | PASS | N/A |
| Verify that the submit button is accessible even if there aren't any inputs in the text fields | PASS | Improvement: The submit button shouldn't clickable unless both the email and password textfileds are filled |

## Forgotten Password

| Test Case | Status | Defects |
|---|---|---|
| The hyperlink for 'forgotten password' should be visible and accessible | PASS | N/A |
| The hyperlink for forgotten password should redirect to forgotten password webpage successfully  | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

## Shortcut 

| Test Case | Status | Defects |
|---|---|---|
| Verify that the registration page shortcut is visible on Log-in page and information is accurately dispayed  | PASS | N/A |
| Verify that the redirecting shortcut button is visible and redirects to registration page properly | PASS | N/A |

# Forgotten Password Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the labels and texts on the page is visible and accurate | PASS | N/A |

## TextField

| Test Case | Status | Defects |
|---|---|---|
| Verify that the the placeholders are visible and accurate | PASS | N/A |
| Verify that the textField accepts inputs | PASS | N/A |

## Buttons

| Test Case | Status | Defects |
|---|---|---|
| Verify that the buttons for submission and going back are visible  | PASS | N/A |
| Verify that the 'submit' button functionality is properly functional | PASS | N/A |
| Verify that the 'back' button functionality is properly functional and redirects back to the login page | PASS | N/A |

## Form

| Test Case | Status | Defects |
|---|---|---|
| Verify that the form displays error message when empty textfields are submitted | PASS | N/A |
| Verify that the form displays error message when unregistered email are submitted | PASS | N/A |
| Verify that the form accepts accurate and registered email  | PASS | N/A |
| Verify that the form displays confirmation message when registered email is submitted | PASS | N/A |

## Password Reset Link

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Password Reset Link is sent to inputted Email Address | FAIL | Link is not being sent to the Email |
| Verify that the reset link has time constraint  - User must wait a specified amount of time before requesting the link again - User must have specified amount of chances for sendng email request per day | FAIL | No Such Functionality is available |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Registration Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the labels for Personal Details , Passwords, Privacy hyperlink and Newsletter Subscription is visible clearly | PASS | N/A |
| Verify that the heading for registration page is visible accurately | PASS | N/A |
| Verify that the compulsory feilds are marked by star | PASS | N/A |

## TextField

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the fields are accessible and visible | PASS | N/A |
| Verify that all the fields contains placeholders | PASS | N/A |

## Form

| Test Case | Status | Defects |
|---|---|---|
| Verify that the form doesn't submits unless Privacy checkbox is checked | PASS | N/A |
| Verify that the form doesn't submits with empty values on compulsory fields | PASS | N/A |
| Verify that the form doesn't submits with invalid input formats in the fields | FAIL | Submits numbers and special characters in First Name |
| Verify that the form displays error message if initial and confirm password doesn't match | PASS | N/A |
| Verify that the form displays error message if already registered Email is submitted | PASS | N/A |
| Verify that the form displays error message if already registered Telephone is submitted | FAIL | Accepts pre-registered telephone number |

## Buttons

| Test Case | Status | Defects |
|---|---|---|
| Verify that the buttons for submission and going back are visible  | PASS | N/A |
| Verify that the 'submit' button functionality is properly functional and redirects to Account Confirmation message page | PASS | N/A |

## Hyperlinks

| Test Case | Status | Defects |
|---|---|---|
| Verify that the hyperlink for Privacy policy redirects to the Privacy Policy page | PASS | Improvement: Informations lacking in privacy policy page |
| Verify that the hyperlink for login page redirects to the login page | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

## Email Confirmation

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Email is sent to the user confirming the account registration  | FAIL | Email service is not functional |

# Account Registration Confirmation Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the headings for page is visible and proper. | PASS | N/A |
| Verify that the Information given in the page is accurate | PASS | N/A |

## Hyperlinks

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Contact us hyperlink is visible and accessible | PASS | N/A |
| Verify that the Contact us hyperlink redirects to 'contact us' page | PASS | N/A |

## Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the next/continue button is visible and accessible | PASS | N/A |
| Verify that the button redirects to My Accounts webpage | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Product Detail Page


## Locate

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Product detail is located when any product image is clicked from the product page / home page | PASS | N/A |

## Product Details

| Test Case | Status | Defects |
|---|---|---|
| Verify that the page includes product details such as :    - Valid product image (From different Angles + Variations with a highlighting functionalities) - Correct Product name - Product Brand  - Product Model Number - Individual Product price - Reward points (gainable) - Product price in reward points  - Availability status in Stock  - Product's Ex. Tax   | FAIL | Some Products don't show awardable reward points  |

## Description Tab

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product's detailed description is displayed for every product in Description tab | PASS | N/A |
| Verify that the description is accurate and relatable to the product | FAIL | Not all product contains accurate details in their description  Ex : Instead of specs for devices ,Advertising description is wirtten. |

## Specification Tab

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Products's specification is displayed. | FAIL | for product HP LP3065 , Specification tab is given for specs , mean while other products do no have specification tab |

## Reviews Tab

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product reivews are given on the website for every products | PASS | N/A |
| Verify that if no Review is given by any user , display No reviews plage | PASS | N/A |
| Verify that the count of reviews is displayed in Label of Reviews tab | PASS | N/A |
| Verify that the user is able to make a review of it's own for each product | PASS | N/A |
| Verify that the Review form incldues following components that are visible and accessible :  - User's Name - User's Review in sentences - User's Rasting in stars (outof5)   Verify that the input format is valid | FAIL  | User name which was accepted with registration is required to be changed during review due to review name length capacity |
| Verify that the review form marks compulsory fields and doesn't submits unless all review fields are fillied | PASS | N/A |
| Verify that the system displays error message when invalid or empty reviews are being submitted | PASS | N/A |
| Verify that the review submit confirmation message is displayed after being submitted by the user | PASS | N/A  |
| Verify that review reflects on the page within 24 hours | FAIL | Even after 24 hours, User's review isn't reflected on the page |

## Review Presentation 

| Test Case | Status | Defects |
|---|---|---|
| Verify that the star icons for reviews are visible and arefillied accurately  | FAIL | There are no Reviews on Any product |
| Verify that the write reviews hyperlink should display the 'Write a review page' on click | PASS | N/A |

## Add To Wishlist Icon

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Add to Wish-List button is visible and accessible for each item | PASS | N/A |
| Verify that the wishlist button is functional and Add the product into the wishlist | PASS | N/A |
| Verify that the confirmation message is displayed when Added a product to wishlist | PASS | N/A |

## Add To Compare Icon

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Add to Compare button is visible and accessible for each item | PASS | N/A |
| Verify that the Add to Compare button is functional and Add the product into the Compare List | PASS | N/A |
| Verify that the confirmation message is displayed when Added a product to Compare list | PASS | N/A |

## Cart functionality

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Add to Cart button is visible and accessible for all the products | PASS | N/A |
| Verify that the Add to cart button carts the item depending on the number of quantity selected | PASS | N/A |
| Verify that the confirmation message for Sucessful Carted Products is displayed | PASS | N/A |
| Verify that the products carts is reflected in the Cart icon in the cart icon | PASS | N/A |
| Verify that the quantity selection bar is visible and functional for all the products  | PASS | N/A |
| Verify that the the input in quantity selection bar is only accepted when inputs are valid | FAIL |  Accepts Empty Values |
| Verify tha tthe error message is displayed when invalid input format is entered and submtted  | FAIL | Shows No Error for invalid inputs for Quantity bars |

## Related Products tab

| Test Case | Status | Defects |
|---|---|---|
| Verify that the products in the related products tab are visible and accessible  | FAIL | Some products do not have related products section display even if related products are available  |
| Verify that the functionalities for related products functions like products from product page   - Add to cart - Add to Wishlist  - Add to Compare List  - Product detail page on click | PASS | N/A |

## Available Optionss (Delivary dates)

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Available options for each product displays Delivary date selection for Available products | FAIL | For product Canon EOS 5D, the Delivary date option is incorrectly setted , there aren't any options to select from |

# Shopping Cart Module


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the headings for the shopping cart and text visuals are clearly visible  | PASS | Improvements : The wieght of Electronic products doesn't makes sense in shopping cart |

## Product table

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product details are displays clearly and accurately :   - Product Name - Product Image  - Product Model Name/Number - Quantity of Product selected  - Individual price  - Total Price  | PASS | N/A |
| Verify that the product name is a hyerlnk for that product details page | PASS | N/A |
| Verify that the unavailable  product is marked within the table | FAIL | Product like HTC Touch HD which are available on the product details page are marked out of stock |
| Verify that the system displays alert message for Unavailable product  | PASS | N/A |
| Verify that the product quantity tab contains following functionalities   - The editable textarea to modify the quantity - The Update table button  - The remove product button | PASS | N/A |
| Verify that the system displays appropriate message for cart being modified | PASS | N/A |

## Totals table

| Test Case | Status | Defects |
|---|---|---|
| Verify that the a small table for adding all the prices of every individual items in cart is displayed | PASS | N/A |
| Verify that the prices shown are accurate and resonates accurately with currency change | FAIL | Currency change is not very accurate |
| Verify that the table includes Shipping charges estimates after the shipping charges have been confirmed | PASS | N/A |

## Coupon Code Drop Down

| Test Case | Status | Defects |
|---|---|---|
| Verify that the drop down for applying the coupon code is viable and clearly visible | PASS | N/A |
| Verify that the textField for coupon code entry is  accessible and edittable | PASS | N/A |
| Verify that the system displays error/Alert  message upon entering invalid / expired coupon code | PASS | N/A |
| Verify that the system displays confirmation message upon entering Valid Coupon code  | N/A  | Can't be tested for the reason of a valid coupon code not available |

## Estimation of Shipping and Service taxes Drop down

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Labels and textFelds for Country , Region /States , Post Code are visible and accurate | PASS | N/A |
| Verify that the drop downs and textFields are visible and functional properly | PASS | N/A |
| Verify that the Submit button is visible and accessible  | PASS | N/A |
| Verify that the form doesn't submits empty values  | PASS | N/A |
| Verify that the system displays error message whenever the invalid/null input format is entered in Compulsory fields | FAIL | The TextField for Postal codes accepts Alphanumberic and Special Characters |
| Verify that the system displays an interactable pop up for presenting and confirming shipping charges accurately | FAIL | The charges for shipping is the same (5$) for all the selected regions acorss the globe |
| Verify that the Appy esitmated button isn't clickable unless the the radio button is checked | PASS | N/A |
| Verify that the system displays confirmation alert message for shipping charge | PASS | N/A |

## Use Gift certification Drop Down

| Test Case | Status | Defects |
|---|---|---|
| Verify that the labels for the heading and textsa visible and correctly placed | PASS | N/A |
| Verify tha the the textFields for input is visible and accessible  | PASS | N/A |
| Verify that the system displays error message for invalid code input | PASS | N/A |
| Verify that the submit button is visible and acessible | PASS | N/A |
| Verify that the system displays confirmation message for valid inputs | N/A | Not available code for this field |

## Final Submit button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system doesn't allows user to continue to checkout page when the items are Out of stocks | /PASS | N/A |
| Verify that the submit button is visible and redirects to checkout page | PASS | N/A |
| Verify that the system restricts the user to move to checkout page until the shipping tax has been marked.  | FAIL | User can move on to the checkin page even without selecting shipping method  |

# Check-Out Module


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the heading and related texts are visible and accurate to the user | PASS |  |

## CheckOut options Module

| Test Case | Status | Defects |
|---|---|---|
| Verify that the checkout Options module is visible and accessible to the user | FAIL | Drop down isn't interactable |

## Billing Address Details

| Test Case | Status | Defects |
|---|---|---|
| Verify that the BIlling Details drop down is visible and accessible | PASS | N/A |
| Verify that the radio buttons for selecting between default / added user address and add new user address are visible , Acessible and reversible | PASS | N/A |
| Verify that the address details are accurate for all the addresses added by the user in adress book | PASS | N/A |
| Verify that the form for new address contains all the labels that are visible and accessible | PASS | N/A |
| Verify that all the compulsory fields are marked with star | PASS | N/A |
| Verify that all the fields only submits when filled with valid input formats | FAIL | Name fields accepts numerical and special Values |
| Verify that the form restricts submission of Empty values/fields | PASS | N/A |
| Verify that the fields contains placeholders | PASS | N/A |
| Verify that the Address confirmation message is displayed after successful submission | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always accessable , though submission isn't possible when fields are empty or null |
| Verify that the updates inputs are reflected on the address book | PASS | N/A |

## Delivary Address  Details

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Delivary Adress Details drop down is visible and accessible | PASS | N/A |
| Verify that the radio buttons for selecting between default / added user address and add new user address are visible , Acessible and reversible | PASS | N/A |
| Verify that the address details are accurate for all the addresses added by the user in adress book | PASS | N/A |
| Verify that the form for new address contains all the labels that are visible and accessible | PASS | N/A |
| Verify that all the compulsory fields are marked with star | PASS | N/A |
| Verify that all the fields only submits when filled with valid input formats | FAIL | Name fields accepts numerical and special Values |
| Verify that the form restricts submission of Empty values/fields | PASS | N/A |
| Verify that the fields contains placeholders | PASS | N/A |
| Verify that the Address confirmation message is displayed after successful submission | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always accessable , though submission isn't possible when fields are empty or null |
| Verify that the updates inputs are reflected on the address book | PASS | N/A |

## Delivary Methods

| Test Case | Status | Defects |
|---|---|---|
| Verify that the heading and texts for the module is visible clearly and accurate | PASS | N/A |
| Verify that the Delivary Shipment method is choosable between other methods | FAIL | There is  only one method available for all product |
| Verify that the comment text area is visible and accessible for the user | PASS | N/A |
| Verify that the submission button is visible and accessible | PASS | N/A |

## Payment Methods

| Test Case | Status | Defects |
|---|---|---|
| Verify that the heading and texts for the module is visible clearly and accurate | PASS | N/A |
| Verify that the Payment method is choosable between other methods | FAIL | There is  only one method available for all product |
| Verify that the comment text area is visible and accessible for the user |  |  |
| Verify that the submission button is visible but inaccessible until terms agreement has been checked by the user | FAIL | Button is accessible even when privacy isn't checked |
| Verify that the terms agreement is visible and it's hyperlink redirects to terms and conditon page | PASS | N/A |
| Verify that the system dispays error message when terms and conditions aren't checked and button is clicked | PASS | N/A |

## Order Confirmation Review 

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Order confirmation reivew drop down is visible and accessible | PASS | N/A |
| Verify that the drop down contains tables that includes accurate details related to product:   - Product Name  (Hyperlink for product's detail page + Delivary date if selected from product's detail page) - Model number/name - Quantity - Individual price - total price per product - Sub-total price  - Shipment tax  - Final total price | PASS | N/A |
| Verify that the button for order confirmation is visible and accessible | PASS | N/A |
| Verify that the button redirects to the order sucessful confirmation page if the order is sucessfully placed | PASS | N/A |
| Verify that the button redirects to error page if order is unsuccessful. | FAIL | Can not test this because nahi ata yeh kaise karo |

# Order Confirmation Page


## Order Confirmation Review 

| Test Case | Status | Defects |
|---|---|---|
| Verify that the order confirmation is displayed and redirected to properly | PASS | N/A |
| Verify that the labels and texts arevisible and accurate for the user regarding the order | PASS | N/A |
| Verify that the hyperlinks are visible and acccessible for account page, Account history page , downloads page and contact us page | PASS | N/A |
| Verify that the continue button redirects to the home page  | PASS | N/A |
| Verify that the sms/email notification is forwarded to the user after the order has been placed | FAIL | No SMS / Mail is sent to the user |

# Footer Module


## Footer

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Footer module is visible and accessible on every webpages on of the site | PASS | N/A |

## Information List

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the components of Information List are visible | PASS | Improvement: The texts / informations that to be present on all the webpages are missing. Only heading is visiible. |
| Verify that ' About ' hyperlink redirects to About page | PASS |  |
| Verify that the Delivary Information hyperlink redirects to Delivary information page | PASS |  |
| Veirfy that the privacy policy hyperlink redirects to Privacy Policy page  | PASS |  |
| Verify that the Terms and Conditions hyperlink redirects to Terms and conditions page | PASS |  |

## Customer Service List 

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the components of Information List are visible | PASS | N/A |
| Verify that ' Contact ' hyperlink redirects to Contact us page | PASS | N/A |
| Verify that the 'Returns ' hyperlink redirects to product returns page | PASS | N/A |
| Veirfy that the  'Site map ' hyperlink redirects to site-map page  | PASS | N/A |

## Extras List

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the components of Information List are visible | PASS | N/A |
| Verify that ' Brands' hyperlink redirects to Brands page | PASS | N/A |
| Verify that the ' Gift Certificates' hyperlink redirects to Voucher page | PASS | N/A |
| Veirfy that the ' Affiliates' hyperlink redirects to Affliates page  | FAIL | Hyperlink redirects to My Account webpage instead of Affialiation page |
| Verify that the ' Specials' hyperlink redirects to Specials offers page | PASS | N/A |

## My Account List

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the components of Information List are visible | PASS | N/A |
| Verify that ' My accounts ' hyperlink redirects to My Account page | PASS | N/A |
| Verify that the ' Order history ' hyperlink redirects to Order History page | PASS | N/A |
| Veirfy that the ' Wishlist' hyperlink redirects to Wishlist page  | PASS | N/A |
| Verify that the 'News letter ' hyperlink redirects to NewsLetter Subscription page | PASS | N/A |

## Licensing / Providers

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Licensing and Copyright tags are visible and acessible  | PASS | N/A |
| Verify that the provider's hyperlink is visible and accessible | PASS | N/A |

# Product List Module


## Product list Functionality

| Test Case | Status | Defects |
|---|---|---|
| Verify that the list items expands to show sub-list items when clicked. | FAIL | Expansions on tabs aren't visible and accessible. :   - Tablets - Softwares - Phones and PDAs - Cameras  |
| Verify that the Product list module is displayed everytime tabs of Product nav bars are clicked. | FAIL | Product list module doesn't appears when clicked on tabs like   - Desktop - Laptops - Components  - MP3 Players |

## Path navigation bar

| Test Case | Status | Defects |
|---|---|---|
| Verify that it contains Direct Home locating icon. | PASS | N/A |
| Verify that it carries paths of modules in hyperlink format that are visible and accessbile | PASS | N/A |

## Desktops

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible in the list | FAIL | Page includes ,Product no. 8 (No proper Image and  Proper name  of product) without any proper information |
| Verify that the product detail section and related Products are accurately displayed and accessible | FAIL | Irrelvant products are als included into the product page - Mobile phones - Cameras |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | NA |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | PASS | N/A |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | FAIL | Some products redirects to Product Information Page rathern than adding the product to the cart. -  - Apple Cinema 30" - Canon EOS 5D - HP LP3065 - Product 8  |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## Laptops & Notebooks

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | PASS | N/A |
| Verify that the product detail section and related Products are accurately displayed and accessible | PASS | N/A |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS  | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | FAIL | Refine hyperlinks shows 0 count of windows and Mac sub-sections even tho there atleast 05 laptop  |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | FAIL | Product HP LP3065 redirects to product detail page instead of adding product to the cart  |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## Components

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | FAIL | Doesn't diplays two available monitors on the product page |
| Verify that the product detail section and related Products are accurately displayed and accessible | PASS | N/A |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | FAIL | Displays  futher sub-sub section  of test 01 and tesr 02 refined search which is empty and irrelevant  |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | FAIL | Some items redirects to Item informatrion page instead of adding the item to the cart - Apple Cinema 30" |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## Tablets

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | PASS | N/A |
| Verify that the product detail section and related Products are accurately displayed and accessible | FAIL | No details/ nformation about section etc. |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | FAIL | No Refined Search functionality found |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## Softwares

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | PASS | N/A |
| Verify that the product detail section and related Products are accurately displayed and accessible | FAIL | No details/ nformation about section etc. |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | PASS | N/A |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | PASS | N/A |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## Phones & PDAs

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | PASS | N/A |
| Verify that the product detail section and related Products are accurately displayed and accessible | FAIL | No details/ nformation about section etc. |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | PASS | N/A |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## Cameras

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | PASS | N/A |
| Verify that the product detail section and related Products are accurately displayed and accessible | FAIL | No details/ nformation about section etc. |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | PASS | N/A |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | FAIL | Some items redirects to Item informatrion page instead of adding the item to the cart -  Canon EOS 5D  |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

## MP3 players

| Test Case | Status | Defects |
|---|---|---|
| Verify that the product names with number of available products are visible accurately in the list | PASS | N/A |
| Verify that the product detail section and related Products are accurately displayed and accessible | PASS | N/A |
| Verify that the product 'List' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the product 'Grid' view layout functionality is visible and performs accurately | PASS | N/A |
| Verify that the 'Compare Product' hyperlink is clearly visible and accessible  | PASS | N/A |
| Verify that the 'Compare Product' hyperlink always displays the number of product selected for comparison | PASS | N/A |
| Verify that the 'Compare products' hyperlink displays Product comparison page on click | PASS | N/A |
| Verify that the product Sort DropDown is visible clearly and functions accurately. | FAIL | Ratings sort doesn't shows any ratings for any item while sorting |
| Verify that the number of product displayed is accurate from 'show' drop down functionality | PASS | N/A |
| Verify that the 'Refine Search' functionality is available , visible and completely functional | FAIL | Irregular number of refined searches sections and unnumbered searches. |
| Verify that the 'add to cart' button option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to cart' button options adds selected product, once into the cart when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view ' cart' tab after every product is carted from 'add to cart' button | PASS | N/A |
| Verify that the Product Carted message is displayed successfully for each selected product - Includes (Product Name hyperlink and Shopping cart hyperlink) | PASS | N/A |
| Verify that the product Carted message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Shopping cart hyperlink redicrects to Shopping cart page | PASS | N/A |
| Verify that the 'add to Wishlist' button  and it's 'logo' option is visible and accessible for all the products displayed | PASS | N/A |
| Verify that the 'add to wishlist' button options adds selected product, once into the wishlist when clicked | PASS | N/A |
| Verify that the screen scrolls upwards to view 'Wishlist' hyperlink from Nav bar, after every product is wishlisted from 'add to wishlist' button | PASS | N/A |
| Verify that the Product Wishlisting message is displayed succesfully for each selected product - Includes (Product name and Product Wishlist page hyperlink)  | PASS | N/A |
| Verify that the Product Wishlisting message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - Product wishlist hyperlink redicrects to product wishlist page | PASS | N/A |
| Verify that the 'Compare Product' button and it's 'logo' is clearly visible and accessible. | PASS | N/A |
| Verify that the Screen is scrolled to the top to view 'Product Comparison' hyerlink in Products page | PASS | N/A |
| Verify that the Product Comparison message is displayed successfully for each selected product - Includes (Product Name and Compare product Hyperlink) | PASS | N/A |
| Verify that the product Comparison message Hyperlinks performs properly:  - Product name hyperlink redirects to product information page - SCompare product hyperlink redicrects to Product comparison page | PASS | N/A |
| Verify that the 'Showing item' and 'number of page' is mentioned at the bottom of product page accurately  | PASS | N/A |

# Sidebar Menu


## Guest User

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Login shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the Register shortcut is visible and redirects to Registration page for any unregistered / logged out user | PASS | N/A |
| Verify that the forgotten password shortcut is visible and redirects to forgotten password page for any unregistered / logged out user | PASS | N/A |
| Verify that the 'my account' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Address Book' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Wishlist' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Order history' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Downloads' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Recurring payments' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the '  Reward points' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Returns ' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Transaction ' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |
| Verify that the ' Newsletter' shortcut is visible and redirects to Login page for any unregistered / logged out user | PASS | N/A |

# Contact Us Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the headings and texts on the webpages are clearly visible and accurate | PASS | N/A |
| Verify that the Address , Telephone , Name and Mail id is clearliy visible and accurate as per user's inputs while registration | PASS | N/A |

## TextFields

| Test Case | Status | Defects |
|---|---|---|
| Verify that the textFields are auto fillied but editable | PASS | N/A |
| Verify that the name and email fields accepts valid input format | FAIL | Numbers are accepted in Name field |
| Verify that the enquiry Editible text area is compulsory | PASS | N/A |

## Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the submit button is visibile and accessible | PASS | N/A |
| Verify that the Submit button redirects to Confirmation page. | PASS | N/A |

## Confirmation Page

| Test Case | Status | Defects |
|---|---|---|
| Verify that the confirmation page is loaded properly | PASS | N/A |
| Verify that the confirmation is clearly visible  | FAIL | Page is empty. No Confirmation message is visible |
| Verify that the continue button is visible and accessible | PASS | N/A |
| Verify that the continue button redirects to home page | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# My Account Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the labels and texts for the webpage visible and clear | PASS | N/A |
| Verify that the headers are visible and clear | PASS | N/A |

## My Account Hyperlink section

| Test Case | Status | Defects |
|---|---|---|
| Verify that the hyperlink for edit details page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for edit details page redirects to 'Details Edit page'   | PASS | N/A |
| Verify that the hyperlink for change password page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for change password page redirects to 'Change Password' page | PASS | N/A |
| Verify that the hyperlink for Address Book page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Address Book page redirects to the Address Book Page | PASS | N/A |
| Verify that the hyperlink for wishlist page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Wishlist page is redirects to the Wish list Page | PASS | N/A |

## My Orders hyperlink Section

| Test Case | Status | Defects |
|---|---|---|
| Verify that the hyperlink for Order Hstory page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Order History page redirects to Order History page | PASS | N/A |
| Verify that the hyperlink for Down history page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Download history page redirects to the Account Downloads page | PASS | N/A |
| Verify that the hyperlink forReward points page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Reward points page redirects to the Reward points page | PASS | N/A |
| Verify that the hyperlink for Returns is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Returns page redirects to the Product returns Page | PASS | N/A |
| Verify that the hyperlink for Transaction page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for Transaction page redirects to the Your Transaction page | PASS | N/A |
| Verify that the hyperlink for recurring payments page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for recurring payments page redirects to the Recurring payments | PASS | N/A |

## My Affiliates Accounts hyperlink section

| Test Case | Status | Defects |
|---|---|---|
| Verify that the hyperlink for Register Affiliates Accounts page is visible and accessible | FAIL | After has registered once, this Hyperlink never re-occurs for user to add more affilaites |
| Verify that the hyperlink for Affiliates Accounts page redirects to Add-Affiliates page | PASS | N/A |
| Verify that the hyperlink for Edit Affiliates Accounts page is visible and accessible only when user has added an affiliate | PASS | N/A |
| Verify that the hyperlink for Edit Affiliates Accounts page redirects to Edit-Affiliates page | PASS | N/A |
| Verify that the hyperlink for  Custom affiliates tracking code Affiliates Accounts page is visible and accessible only after the user has registered it's affilaites | PASS | N/A |
| Verify that the hyperlink for Custom Affiliates tracking code Accounts page redirects to Custom Affiliates account page -Affiliates page | PASS | N/A |

## Newsletters hyperlink Sections

| Test Case | Status | Defects |
|---|---|---|
| Verify that the hyperlink for Newsletter subcription page is visible and accessible | PASS | N/A |
| Verify that the hyperlink for news letter subscription page redirects to newsletter subcription page | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Details Edit Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the header and texts related to the page is clearly visible  | PASS | N/A |

## TextFields

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the fields are marked compulsory | PASS | N/A |
| Verify that the fields hold user's previously input details accurately | PASS | N/A |
| Verify that the fields contains accurate placeholders  | PASS | N/A |

## Form

| Test Case | Status | Defects |
|---|---|---|
| Verify that the form submits only when all the compulsory fields are filled with Valid inputs as per valid format | FAIL | Form submits even if the Name fields are filled with Numeral and special Characters |
| Verify that the form restricts the submission if fields are filled with only Null values | PASS | N/A |
| Verify that the form displays error message when registered email is being replaced with another email which is already registered with another account  | PASS | N/A |
| Form displays confirmation message when valid inputs are submitted. | PASS | N/A |

## Buttons

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Back and Continue buttons are visible and acessible | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always access , though submission isn't possible when fields are empty or null |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Change Password Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the header and texts related to the page is clearly visible  | PASS | N/A |

## TextFields

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the fields are marked compulsory | PASS | N/A |
| Verify that the fields restrict autofill functionalities | PASS | N/A |
| Verify that the fields contains accurate placeholders  | PASS | N/A |

## Form

| Test Case | Status | Defects |
|---|---|---|
| Verify that the form submits only when all the compulsory fields are filled with Valid inputs as per valid format | PASS | N/A |
| Verify that the form only submits if the input Confirm password field matches the prior password field | PASS | N/A |
| Verify that the form checks the condition of  password must not the same the previous one. | FAIL | Even if passwords that were previously saved are overwritten  Ex:   Password yesterday : 1234  Password today : 1234   Status : Accepted and overwritten, System should have displayed error message like password can not be same as the previous password |
| Verify that the system displays change update confirmation message  | PASS | N/A |

## Buttons

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Back and Continue buttons are visible and acessible | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always access , though submission isn't possible when fields are empty or null |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Address Book Page


## Empty book

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays no address message when no address has been added yet | PASS | N/A |

## Buttons

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Back and Add New Address buttons are visible and acessible | PASS | N/A |
| Verify that the Back redirects to previous webpage while Add New Address button redirects to add New Address page | PASS | N/A |

## New Address Page

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the compulsory fields are marked with star | PASS | N/A |
| Verify that all the fields only submits when filled with valid input formats | FAIL | Name fields accepts numerical and special Values |
| Verify that the form restricts submission of Empty values/fields | PASS | N/A |
| Verify that the fields contains placeholders | PASS | N/A |
| Verify that the Address confirmation message is displayed after successful submission | PASS | N/A |
| Verify that the Back and Continue buttons are visible and acessible | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always access , though submission isn't possible when fields are empty or null |

## Updated Address Book

| Test Case | Status | Defects |
|---|---|---|
| Verify that the books displays detailed Address input by the user accurately | PASS | N/A |
| Verify that the Edit and Delete buttons and thier functionalities are as expected | FAIL | Once an address is selected Default it's not being updated to not default by edit option |
| Verify that the default addresses can not be Deleted | PASS | N/A |
| Verify that there can be a default address | FAIL | There are more than one default address addable, there can only be one default address |
| Verify alert messages displays while trying to delete default address | PASS | N/A |
| Verify that the confirmation messages is displayed after the updates of address | PASS | N/A |
| Verify that the updates inputs are reflected on the address book | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Wish List Page


## Empty list

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays no empty wishlist message when no product has been added yet | PASS | N/A |

## Updated List

| Test Case | Status | Defects |
|---|---|---|
| Verfy that the system displays all the Wishlisted Products  along with their details  -  Image -  Product Name -  Model name / Number -  Availability in Stocks  -  Individual Prices (along with discounted prices)  | FAIL  | A typo error with respect to stocks detail.. Instead of showing '2-3 items' , it displays '2-3 days' |
| Verify that the product can be deleted using the delete button  | PASS | N/A |
| Verify that the item can be carted using the cart button and message is displayed  | FAIL |  Few Items aren't getting carted , Instead they redirect to product detail page |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Order History Page


## Empty History

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays no order history message when no product has been ordered yet | PASS | N/A |

## Updated List

| Test Case | Status | Defects |
|---|---|---|
| Verify that the labels and table / text is visible | PASS | N/A |
| Verify that the table include order's details :   - Order ID  - Customer Name  - Product Qunatity  - Status of Order (Pending / Delivered)  - Order charge  - Delivary date selected by the user   - Order Information Icon button | PASS | Improvement: There should have been Product name in the table and Adding Customer name is not sensible |

## Pagination

| Test Case | Status | Defects |
|---|---|---|
| Verify that the orders history is properly paginated and user is able to paginate between multiple pages to view brief history of orders   - NUmber of orders per page - 10  - Next page  - Previous page   - First page  - Last page | PASS | N/A |

## Order Information Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the order information button redirects to Order information page for that specified order | PASS | N/A |

# Order Information Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the headings and texts are visible and accurate | PASS | N/A |

## Order Information Table

| Test Case | Status | Defects |
|---|---|---|
| Verify that the table include order's details :   - Order ID  - Payment Method  - Order Date  - Shipment method  - Billing address  - Shipping address  - Product Name  - Product Qunatity  - Status of Order (Pending / Delivered)  - Order charge  - Delivary date selected by the user    | PASS | N/A |
| Verify that the Reorder Button is visible and functional | PASS | N/A |
| Verify that the same item is carted upon clicking Reorder button  | PASS | N/A |
| Verify that the product carted confrimation message is displayed. | PASS | N/A |
| Verify that the Return Button is visible and functional | PASS | N/A |
| Verify that the Returns Button redirects to the Product returns Page | PASS | N/A |
| Verify that the Submit/Continue button redirects to Order History Page | PASS | N/A |

# Product returns page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the headings and texts are visible and accurate | PASS | N/A |

## Order Information

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the compulsory fields are marked | PASS | N/A |
| Verify that the fields are autofilled with usual customer and Order details:   - First Name - Last Name - Email - Telephone - Order ID - Order Date | PASS | N/A |
| Verify that the fields contains accurate placeholders  | PASS | N/A |
| Verify that the form only accepts valid input formats | FAIL | Telephones field accepts spaces , Alphabets and special characters |
| Verfiy that the messages for invalid input formats are displayed  | PASS | N/A |

## Product Information 

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the compulsory fields are marked | PASS | N/A |
| Verify that the fields are autofilled with Product details:   - Product Name - Product Model  - Product Qunatity  | FAIL | Label for Product model is instead written as 'Product Code' |
| Verify that the Radio buttons for reason of return is diplsyaed and accessible  - Damaged on Arrival - Wrong order /order error - Order Error - Wrong Item Recieved - Other reasons | PASS | NOTE : Dead on Arrival sounds rude and innaceptible |
| Verify that the user must select atleast one reason before submitting the return request | PASS | N/A |
| Verify that the user must select if the box of order has been opened or not | PASS | N/A |
| Verify that the More Information text area is visible and accessible | PASS | N/A |

## Submit Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Back and Continue buttons are visible and acessible | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always access , though submission isn't possible when fields are empty or null |

## Product Return confirmation

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system redirects to prodcut returned confirmation webpage after retrun has been sucessfully requested | PASS | N/A |
| Verify that the heading and texts are visible and accurate | PASS | N/A |
| Verify that the Details about product return is sent to the user's registered telephone/email upon request  | FAIL | SMS/Mail service not functional  |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Download History Page


## Empty Downloadable order

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays ' No downloadable Orders placed yet' message when no product has been downloadable ordered yet | PASS | N/A |

## Updated Downloadable History page

| Test Case | Status | Defects |
|---|---|---|
| Verify that the downloadable history page reflects the downloadable order's history | FAIL | No products that can downloaded |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Reward Points Page


## Empty Rewards point page

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays ' No Rewards points ' message when no product has been ordered yet | PASS | N/A |

## Updated Rewards Point Page

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays reward points as per the ordered products accurately | FAIL | Even though orders have been placed, No reward points are being given to the user nor reflected in rewards points page |

## Continue Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the continue button is visible and redirects to Accounts page | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Transaction Page


## Empty transaction History

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays 'No transactions yet' message when no transactions have been made yet | PASS | N/A |

## Balance

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system correctly displays proper balance in the account for the user | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# Recurring Payments Page


## Empty Payments page

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays 'No Recurring payments yet' message when no payements have been made yet | PASS | N/A |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

## Continue Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the continue button is visible and redirects to Accounts page | PASS | N/A |

# Add Affiliates Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the heading and the detailing texts are visible and clear | FAIL | The Hyper link for Agreement is labeled and redrects to About us page pop up |
| verify that the radio buttons are visible and accessible | PASS | N/A |

## My Affiliates Account Module

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Company textFields accepts proper inputs  | FAIL | Accepts only Spaces values and Empty field as well with NO error Message Displayed |
| Verify that the Website textFields accepts proper inputs  | FAIL | Accepts only Spaces values and Empty field as well with NO error Message Displayed |

## Payments Information Module

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Tax ID textFields accepts proper inputs  | FAIL | Accepts only Spaces values and Empty field as well with NO error Message Displayed |
| Verify that the radio buttons for Payment mode informations are visible and reversiblely accessible |  |  |
| Verify that the Cheque Payee Name (Compulsory field) is displayed and is accessible when CHEQUE payment option on radio button is selected | PASS | Improvement: Field is not marked even though is it compulsory field |
| Verify that the Paypal Email Account (Compulsory field) is displayed and is accessible when PAYPAL payment option on radio button is selected | PASS |  |
| Verify that the Compulsory fields are displayed and is accessible when BANK TRANSFER payment option on radio button is selected  - Bank Name  - Branch Number - SWIFT code - Account Name - Account Number | FAIL | Improvement: Fields are not marked even though is it compulsory fields |

## Agreement checker module

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Agreement Check box is visible with it's lables and hyperlinks and accessible | PASS | N/A |
| Verify that the system displays error notifications when Form is beng submitted without chec box being checked | PASS | N/A |

## Submit Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that the Continue buttons are visible and acessible | PASS | N/A |
| Verify that the button for submission is only accessible when all the compulsory field are filled | FAIL | Button is always accessable |

## Side Bar Menu

| Test Case | Status | Defects |
|---|---|---|
| Verify that the sidebar menu and it's components are visible | PASS | N/A |

# News Letter Subscription Page


## Labels

| Test Case | Status | Defects |
|---|---|---|
| Verify that the heading and the detailing texts are visible and clear | PASS | N/A |
| verify that the radio buttons are visible and accessible | PASS | N/A |

## Radio button

| Test Case | Status | Defects |
|---|---|---|
| Verify that radio buttons can only be selected one at a time. | PASS | N/A |

## Submission button

| Test Case | Status | Defects |
|---|---|---|
| Verify Submission button is visible and accessible | PASS | N/A |

## Message

| Test Case | Status | Defects |
|---|---|---|
| Verify that the system displays alert messages of successful update | PASS | N/A |

## Update

| Test Case | Status | Defects |
|---|---|---|
| System should hold the updates made unless changed  | PASS | N/A |

# Logout Module 


## Update

| Test Case | Status | Defects |
|---|---|---|
| Verify that the logout functionality is functional | PASS | N/A |
| Verify that the user will not be able to place order of access My Account Modules without being Logged In | PASS | N/A |