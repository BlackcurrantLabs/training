# Test Cases Examples : Browser Stack

BrowserStack is another sample e-commerce website with a standard layout and user interface. Unlike basic practice websites, it contains several subtle defects that are not immediately visible and cannot be identified through casual exploration. Many of these issues require specific user actions or a sequence of steps to reproduce, making it an excellent platform for practicing exploratory and scenario-based testing.

**Website:** [Browser Stack E-Commerce Website](https://www.bstackdemo.com/)

**Note:** Although this document includes only the test cases and a few sample defects, you are expected to thoroughly explore the entire website and identify at least three additional defects (major or minor) that require specific steps to reproduce. At present, the website contains eight known defects intentionally included for testing practice.


# Home Page 

## Website Logo

| Test Case | Status | Defects |
|---|---|---|
| Verify that logo is visible and accessible | PASS | N/A |
| Verify that user is redirected to the home page when clicked on Logo | PASS | N/A |

## Nagivation Bar 

| Test Case | Status | Defects |
|---|---|---|
| Verify that nav bar is visible and includes intended navbar components :   - Logo  - Offers page hyperlink - Orders page hyperlink - Searchbar  - Search button  - Favorites page hyperlink  - sign in / log-out / Account holder's name in visible hyperlink. | PASS | N/A |
| Verify that guest user is rediredted to log in page upon interacting with hyperlinks :  - Offer page hyperlink - Orders page hyperlink - favorites page hyperlink  - sign in page hyperlink | PASS | N/A |
| Verify that the Account holder's name hyperlink is visible and accessible , redirecting uset to accounts / uer information page. | FAIL | Hyperlink is visible but not accessible. |
| verify that logout hyperlink functionality properly functions , making logged in user log out  | PASS | N/A |
| Verify that cart button icon is is visible and accessible  | PASS | N/A |
| Verify that a slide window opens displaying cart details when user interacts with the cart button icon. | PASS | N/A |
| Verify that cart icon moves along with the nav bar when the page is scrolled. | PASS | N/A |

## Search Bar and Button

| Test Case | Status | Defects |
|---|---|---|
| Verify that search bar and button are visible and accessible. | PASS | N/A |
| Verify that search bar is accessible and accepts valid inputs. | PASS | N/A |
| Verify that the products are displayed accurately as per searched items names when the search button is clicked. | FAIL | Search functionality doesn't works. (product page displays same products even  if a particular product is searched for) |

## Information page

| Test Case | Status | Defects |
|---|---|---|
| Verify that information related to the website is displayed properly. | PASS | N/A |

## Product page

| Test Case | Status | Defects |
|---|---|---|
| Verify that all available products are visible properly. | PASS | N/A |
| Verify that all products are interactive, redirecting to the individual product details page. | FAIL | Interacting with product image / Name on product page yeilds no distinguishable results. |
| Verify that all product cards contains visible and interactive components :   - Favorites icon  - Add to cart button | PASS | N/A |
| Verify that for each product, the Favorites icon component adds the product to the favorites page . | PASS | N/A |
| Verify that for each product, the Add to Cart button component adds the product by 01 count to the cart everytime the button is clicked. | PASS | N/A |
| Verify that cart slide window opens automatically displaying the selected product in cart window. | PASS | N/A |
| Verify that bundle deal functionality is accurately functional and is reflected in the cart upon adding bundle deal's item count . | FAIL | the bundle price for the items is not function and reflected in the cart.  example :  Product A 's individual cost is 399$  while it's  bundle deal is 3 x  133,   thus when the user adds three of that product, the cost should be 399 as per bundle deal,  however, in the cart it displays 1197  which is 399 x 3.  |

## Item  price sort 

| Test Case | Status | Defects |
|---|---|---|
| Verify that item price sort is visible and drop down is accessible  | PASS | N/A |
| Verify that sort functionality is accurate for ' Low- High ' sort - Verify that products in the product page are sorted ascendingly according to their prices. | PASS | N/A |
| Verify that sort functionality is accurate for ' High - Low ' sort - Verify that products in the product page are sorted descendingly according to their prices. | PASS | N/A |

## Item brand sort

| Test Case | Status | Defects |
|---|---|---|
| Verify that item brand sort buttons are visible clearly and are accessible. | PASS | N/A |
| Verify that the Item brand sort functionality works properly when buttons realted to the brands are clicked - Verify that product chosen in the sort is accurately displayed | PASS | N/A |
| Verify that multiple buttons can selected in the sort. | PASS | N/A |
| Verify that products of cross / invalid / Different brands are not displayed upon sorts. | PASS | N/A |
|  Verify that product count is accurately displayed upon the sorts. | PASS | N/A |

# Log in Page


## Log in / Sign in

| Test Case | Status | Defects |
|---|---|---|
| Verify that credentials fileds are visible and accessible. | PASS | N/A |
| Verify submit button is visible and redirect to the home page after user logs in. | PASS | N/A |
| Verify that BrowserStack Logo is visible and inaccessible | PASS | N/A |

# Cart 


## Cart Slide window

| Test Case | Status | Defects |
|---|---|---|
| Verify that every carted product from product page is visible with accurate individual prices. | PASS | N/A |
| Verify that the item count is visible from the cart icon. | PASS | N/A |
| Verify that the a sub total and total cost for all the products combined is visible and is displayed accurately. | PASS | N/A |
| Verify that user is able to add or subtract an item count with '+' and '-' icons. | FAIL | The icons are barely visible, must increase the icon size. |
| Verify that addition and subtraction functionality is accurate. | PASS | N/A |
| Verify that the user can remove an individual item from the cart using the 'remove' functionality iconized as  X | PASS | N/A |
| Verify that the cart accurately reflects changes in prices due to item addition , subtraction or removal. | PASS | N/A |
| Verify that slide window can be closed properly with Cross button at the top corner of window | PASS | N/A |
| Verify that cart page is scrollable. | PASS | N/A |
| Verify that the user can not alter the product data in the cart of a registered user. | FAIL | Once user logs out , the data in the cart doesn't goes null but remains there, which allows the guest user to alter the data |
| Verify that products remains holded even if user logs out and re-logs in. | FAIL | The the cart slide page data is lost once user logs out |

# Offers page


## Product page

| Test Case | Status | Defects |
|---|---|---|
| Verify that headers and labels are visible and accurate. | PASS | N/A |
| Verify that products in offer / discount at the moment is displayed. | PASS | N/A |
| Verify that product image on interaction redirects to product detail page / product page from home.  | FAIL | No such functionality is visible or accessible |
| Verify that products have options to cart or added to the favorites.  | FAIL | No such functionality is visible or accessible |
| Verify that the offered prices are also displayed in Product of home page | FAIL | No such functionality is visible or accessible |

# Favorites page


## Product page

| Test Case | Status | Defects |
|---|---|---|
| Verify that the header and labels / texts are visible and accurate. | FAIL | Website details seems unnecessary to be displayed in Favorite page |
| Verify that the products marked as favorite are clearly displayed. | PASS | N/A |
| Verify that product card contains interactive compoments   - Unfavorite - Cart button | PASS | N/A |
| Verify that upon interacting with the favorite button , the product is remvoed from the page and favorite list. | PASS | N/A |
| Verify that product can be carted as usual using the add to cart button | PASS | N/A |
| Verify that the user can not alter the product data in the favorites page of a registered user. | FAIL | Once user logs out , the data in the Favorites slide page doesn't goes null but remains there, which allows the guest user to alter the data |
| Verify that products remains holded even if user logs out and re-logs in. | FAIL | The the favorite page data is lost once user logs out |

# Check Out page


## Checkout button

| Test Case | Status | Defects |
|---|---|---|
| Verify that checkbutton is visible and accessible in the cart. | PASS | N/A |
| Verify that checkout button redirects to checkout page properly. | PASS | N/A |

## User details 

| Test Case | Status | Defects |
|---|---|---|
| Verify that  form doesn't submits unless all the fields are filled with valid inputs. | PASS | N/A |
| Verify that the system displays an error prompt if the user tries to submit an empty form. | PASS | N/A |
| Verify that Name fields (first name + Last name) accepts valid inputs. | PASS | N/A |
| Verify that Name fields prevents invalid input formats . | FAIL | Alphanumeric + Special characters are accpeted in these fields. |
| Verify that Address field accepts valid inputs. | PASS | N/A |
| Verify that State / province field accepets valid inputs. | PASS | N/A |
| Verify that the State / Province fields prevents invalid input formats | FAIL | Alphanumberic + Special characters are accepted in these fields |
| Verify that the postal code field accepts valid inputs | PASS | N/A |
| Verify that the postal code field prevents invalid input formats. | FAIL | Alphnumeric + Special characters are accepted here |
| Verify that the form prompts error notification for any invalid inpt format. | FAIL | No prompt notifications are displayed |
| Verify that submit button is visible and accesible. | PASS | N/A |
| Verify that order summery table is visible and contains accurate information about the chosen carted items  - Product image  - Product Name  - Product brand - Product Individual cost  - Total cost | PASS | N/A |
| Verify that the total cost summs up accurately. | PASS | N/A |

## Submit

| Test Case | Status | Defects |
|---|---|---|
| Verify that, clicking on Submit buttons is visible and redirect to order confirmation page. | PASS | N/A |

# Order confirmation Page


## Order Confirmation

| Test Case | Status | Defects |
|---|---|---|
| Verify that header and text displays correctly verifying the successfull placement of the order. | PASS | N/A |
| Verify that a table of order summery is dispayed . | PASS | N/A |
| Verify that the order summery perfectly matches with the order summery in the cart and checkout page. | PASS | N/A |
| Verify that continue button is visible, that redirects to the home page towards product page section | PASS | N/A |

## Order Bill/receipt 

| Test Case | Status | Defects |
|---|---|---|
| Verify that hyperlink for downloading Order receipt is visible and accessible. | PASS | N/A |
| Verify that an order ID / number is displayed to the user. | PASS | N/A |
| Verify the order receipt is properly downloaded upon interacting with the hyperlink | PASS | N/A |
| Verify that bill is downloaded in PDF / readble format | PASS | N/A |
| Verify that the bill contents are visible and accurate   - Header (Site name) - Structured ordered products data     - Product Brand     - Product Name     - Product Count     - Product Individual price  - Total sum of prices.   | PASS | N/A |