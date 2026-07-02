# Test Cases Examples : GreenKart

GreenKart is one of the simplest e-commerce websites for aspiring QA professionals to begin their testing journey. It features a straightforward design and basic functionalities, making it ideal for beginners to understand application workflows, practice writing test cases, and identify defects with ease.


**Website:** [ GreenKart Groceries ](https://rahulshettyacademy.com/seleniumPractise/#/)

## Page Landing

| Test Case | Status | Defects |
|---|---|---|
| The homepage should load successfully when the website URL is accessed. | PASS | N/A |

# Home Page


## Visuals

| Test Case | Status | Defects |
|---|---|---|
| GreenKart Logo should be Visible | PASS | N/A |
| Search Button , next to search bar must be visible and accessible | PASS | N/A |
| Search Bar with text field must be visible and accessible | PASS | N/A |
| HyperLink 'Top Deals' Must be visible and accessible. | PASS | N/A |
| Labels for 'Items' and 'price' must be visible. | PASS | N/A |
| The "Flight Booking" hyperlink Visible.   | FAIL | Displays an unrelated hyperlink for "Flight Booking."  |
| Logo for Cart must be visible and accessible. | PASS | N/A |
| Copyright claim for Website visible and inaccessible. | PASS | N/A |
| List of products should be visible | PASS | N/A |

## Search Bar

| Test Case | Status | Defects |
|---|---|---|
| Text field should show placeholder. | PASS | N/A |
| Must be interactive and search for correct products, with correct spellings. | PASS | N/A |
| Must Show error message when incorrect or unavailable product name is added on product page. | PASS | N/A |

## Product page

| Test Case | Status | Defects |
|---|---|---|
| Must show products in Highlighted format when cursor is  Hovered upon | PASS | N/A |
| Must show Name ,Weight and price per unit of Products. | FAIL | The Spelling of product 'Broccolli' isn't mentioned. |
| Must show highlight /zoom the product Images when cursor is hovered upon | PASS | N/A |
| Must allow user to Increase or decrease the selected Number of Products using buttons | PASS | N/A |
| Must allow user to type the number of  selected Product using text field | PASS | N/A |
| Allows integers in  text field | FAIL | It allows to type Alphabets (e) |
| Must not allow Null Value. | FAIL | It allows null values after deleting integeral values or typing '0' in text field, Instead of getting it back to '1'. |
| Must allow to Add the selected Number of Products in the cart. | PASS | N/A |
| Must open a product specification page when clicked on a product. | FAIL | Product page doesn't loads |

## Cart Pop-up

| Test Case | Status | Defects |
|---|---|---|
| Must show Empty Cart message popup on click, When Nothing is Stored in the cart. | PASS | N/A |
| Check Out Button must be visible and accessible | PASS | N/A |
| Check Out Button must be unclickable when cart is empty | PASS | N/A |
| Products information (Number of Items , Per Unit Charge , Total Charge of individual Units) must be visible | PASS | N/A |
| Product information must remain visible in cart and Items tab after pages are switched | FAIL | Cart data disappears when the user clicks the browser's "Back" button.  |
| Must redirect on Check -Out Page when clicked on yellow colored Checkout Button | PASS | N/A |

# Top - Deal Page


## Page - Landing 

| Test Case | Status | Defects |
|---|---|---|
| Should locate 'Top Deal' Webpage  | PASS | N/A |

## Page Size Tab

| Test Case | Status | Defects |
|---|---|---|
| Page Size function tab must be visible | PASS | N/A |
| Must Allow to interaction and choose number of products to be displayed in 'Page Size'. | PASS | N/A |
| Must allow user to choose the number of pages using Numbers , First , Previous , Next and Last buttons | PASS | N/A |
| Must Not Allow user to click First , previous , Next or Last buttons if the products are no more available on those page. | PASS | N/A |

## Product Table

| Test Case | Status | Defects |
|---|---|---|
| Actual price per unit and Discounted Price should be visible | FAIL | Prices do not match those on the homepage product page.  |
| Must Allow user to Surf through the Product list in Ascending / Desending Alphabetic order. | PASS | N/A |
| Must allow user to Search for the Products through search bar, | PASS | N/A |
| Add - to - Cart Functionality visible | FAIL | Buttons of add to cart are missing for products. |
| Delivary Dates Functionality visible and accessible | FAIL | Delivary dates before the present date is accepted which shouldn't be possible. |

# Check Out Page


## Page - Landing 

| Test Case | Status | Defects |
|---|---|---|
| Should locate 'Top Deal' Webpage  | PASS | N/A |

## Product Table

| Test Case | Status | Defects |
|---|---|---|
| Must show Product Image , Name , Quantity , Individual Price , Total price of items respectively.  | FAIL | Warning : The 'Quantity' Spelling incorrect |

## PromoCodes

| Test Case | Status | Defects |
|---|---|---|
| Must allow user to type in 'Promocode' text field. | PASS | N/A |
| Must Verify the Promocodes, on clicking 'Apply' button | PASS | N/A |
| Must Show error in red when invalid code is entered. | PASS | N/A |

## Total Charges

| Test Case | Status | Defects |
|---|---|---|
| Must Show total number of Items selected , Total Amount , Discount , Cost after discount  | PASS | N/A |

## Place Order

| Test Case | Status | Defects |
|---|---|---|
| Must redirect to 'Country Selection'. | PASS | N/A |

# Country Selection Build


## Page - Landing 

| Test Case | Status | Defects |
|---|---|---|
| Should locate to 'Country Selection' Webpage.  | PASS | N/A |

## Order Placement page

| Test Case | Status | Defects |
|---|---|---|
| Must allow user to select country from drop down. | PASS | N/A |
| Must allow user to skip search the Country from drop down by typing their Name. | PASS | N/A |
| Must allow user to check the box in Agreement of terms and conditions. | PASS | N/A |
| Must have sections which redirects user to 'Delivary Address' Page | FAIL | Delivary date selection absent here and is placed in 'Top Deals ' build instead. |
| Must Not allow user to proceed without marking Country or Agreement  | PASS | N/A |
| Must redirect to terms and conditions page by clicking on hyperlink underlined in blue | PASS | N/A |

# Terms and Condition Page


## Order Placement page

| Test Case | Status | Defects |
|---|---|---|
| Must hold Information about company's terms and conditions | PASS | N/A |
| Must allow user to go back home page by clicking 'Return home' hyper link | PASS | Warning: spelling of 'go' on the page is incorrect |

# Order Verification Page


## Order Placement page

| Test Case | Status | Defects |
|---|---|---|
| Must provide order confirm with a message and a hyper link to return back to  the home page. | PASS | N/A |