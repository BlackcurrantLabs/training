# Test Cases Examples : Tools.com

Tool.com is another sample e-commerce website that differs in its composition and layout from conventional online shopping platforms. Its distinct interface and page structure provide QA professionals with a fresh testing experience, offering a different environment and a variety of UI components to validate and explore.


**Website:** [ Tools.com E-Commerce Website](https://with-bugs.practicesoftwaretesting.com/#/)

# Home Page

## Site Logo

| Test Case | Status | Defects |
|---|---|---|
| Verify that website logo is visible and accessible. | FAIL | Logo image is broken |
| Verify that website logo redirects to home page from anyone page on click | PASS | N/A |

## Navigation Bar

| Test Case | Status | Defects |
|---|---|---|
| Verify that Navigation bar is visible and hold components of hyperlink / drop down accurately  - Home page hyperlink - Categories drop down - Contacts hyperlink - Sign in hyperlink | FAIL | Contacts hyperlink have incorrect typo error. Spelled Contakt instead of Contact |
| Verify hyperlink Home redirects to specified webpage | FAIL | Link redirects to contacts page instead |
| Verify hyperlink Contacts redirects to specified webpage | PASS | NA |
| Verify hyperlink Sign in redirects to specified webpage | PASS | N/A |
| Verify Categories drop down includes sub tabs :  - Hand tools  - Power tools  - chain saws - Rentals  - unclassified tools  Redirects respectively to   - Hand tools product page - Power tools product page - chainsaws product page - rentals machine product page - unclassfied tools product page | FAIL | Unclassified tools page lacks the product page. No products are displayed. |

## Product page

| Test Case | Status | Defects |
|---|---|---|
| Verify that all the availanle product are displayed accurately, with proper following criteria   - Accurate labels  - Accurate Images  - Accurate price tags  | FAIL | Products have improperly aligned labels. Some are aligned to left while some are liged to right. |
| Verify that pagination functionality works accurately   - Previous page  - Next page  - Page 1,2,3 etc - Previous or Next page disabled depending of current page  | PASS | N/A |

## Sort functionality

| Test Case | Status | Defects |
|---|---|---|
| Verify that sort labels and it's functionality is accurate:   - Labels  - dropdown functionality  - Dropdown components      - Name (A-Z , Z-A)    - Price (Low -  High, High -  Low)   | FAIL | Typo error: 'Sort' written as 'sorth' |

## Price sort functionality

| Test Case | Status | Defects |
|---|---|---|
| Verify that price range sorts functionality is properly functioning.  - Slider bar (1 - 200) - Slider pivot (Displays the range number it's present at ) - Properlt placed hr (horizontal ruling) line  | FAIL | Prince range sort is disfunctional. Doesn't sorts anything |

## Search bar functionality

| Test Case | Status | Defects |
|---|---|---|
| Verify that the search bar functionality is functional properly.  - Labels are clearly visible - Placeholders with instructions are visible - Search bar is clearly visible and accessible - Search logo is visible  - Cross button to cancel the search - No searches until search button is clicked - Search button is visible and completes search functionality on click - Correct products displays on the page depending on correctly searched words. - Prompt erro displays on the page depending on incorrectly searched words.  | FAIL | The Logo image is broken |

## Filter

| Test Case | Status | Defects |
|---|---|---|
| Verify that the BY CATEGORY sections is accurate with the following criterias :   - Labels  - Hand tools check boxes sections are visible and accessible :    - Hammer    - Handsaw    - Wrench    - Screw drivers    - Pliers - User can check multiple checkboxes - Power tools check boxes sections are visible and accessible :    - Grainder    - Sander    - Saw   - Drill - Others    - Rental Machines. - Product page is filtered accurately according to the selected checkboxes  | FAIL | Grinder checkbox displays empty product page |
| Verify that the BY BRAND sections is accurate with the following criterias :   - Labels  - Brands check boxes sections are visible and accessible :    - Brand 01   - Brand 02 - Product page is filtered accurately according to the selected checkboxes  | PASS | N/A |
| Verify that the sorts resonates with each other well.  | PASS | N/A |