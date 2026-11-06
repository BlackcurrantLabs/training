# Testing Challenges

Testing Challenges are a collection of hands-on exercises designed to help beginners build confidence in software testing by practicing a wide variety of testing techniques and validating different types of input and edge cases.

Before learning how to write formal test cases, it is important to understand how to think like a tester. These challenges focus on developing that mindset by encouraging you to explore application behavior, identify defects, validate expected outcomes, and investigate unusual or boundary conditions.

By completing these challenges, you will:

- Develop a practical testing mindset.
- Improve your ability to identify functional and non-functional defects.
- Learn to think beyond happy-path scenarios by exploring boundary values, invalid inputs, security vulnerabilities, and edge cases.
- Build confidence in performing exploratory and manual testing.
- Strengthen your analytical and observation skills.
- Gain practical experience before moving on to formal test case design and documentation.

Once you are comfortable identifying scenarios and defects through these exercises, writing structured test cases will become significantly easier and more meaningful.

*Note: Use Horizontal scroll (Shift+scroll) wherever required*

<style>
.challenge{margin-bottom:40px}
.table-wrap{overflow-x:auto;margin:12px 0}
.sheet{border-collapse:collapse;table-layout:fixed}
.sheet td{
border:1px solid #999;
padding:6px;
vertical-align:top;
white-space:pre-wrap;
overflow-wrap:break-word;
}
</style>

<div class='challenge'>

<h2>Testing Challenge #1 - web testing </h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/index.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 1 - web testing <b> </td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">Category</td>
<td  style="font-weight:bold;text-align:center;">Defects / Out-comes</td>
<td  style="font-weight:bold;text-align:center;">Input </td>
<td rowspan='16' style="background-color:#F4CCCC;text-align:center;">15 out of 18 Found</td>
</tr>
<tr>
<td rowspan='8' style="background-color:#FFFFFF;">Functional Tests</td>
<td  style="background-color:#FFFFFF;">Minimum Value</td>
<td  style="background-color:#FFFFFF;">Single character (e.g., &quot;A&quot;)</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">Space Values at the End</td>
<td  style="background-color:#FFFFFF;">&quot;John &quot;</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">Space Values at the Beginning</td>
<td  style="background-color:#FFFFFF;">&quot; John&quot;</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">Space in the Middle</td>
<td  style="background-color:#FFFFFF;">&quot;John Doe&quot;</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">More than Maximum Values</td>
<td  style="background-color:#FFFFFF;">&quot;ARHTRBEHFBEDSHFUVHVVEVURVHEVIRJJH&quot;</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">Empty Value</td>
<td  style="background-color:#FFFFFF;">(No input)</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">Average Value</td>
<td  style="background-color:#FFFFFF;">&quot;Michael&quot;</td>
</tr>
<tr>
<td  style="background-color:#FFFFFF;">Only Space</td>
<td  style="background-color:#FFFFFF;">&quot;            &quot; </td>
</tr>
<tr>
<td rowspan='3' style="background-color:#EFEFEF;">Security Tests</td>
<td  style="background-color:#EFEFEF;">HTML Tags</td>
<td  style="background-color:#EFEFEF;">&quot;&lt;b&gt;John&lt;/b&gt;&quot;</td>
</tr>
<tr>
<td  style="background-color:#EFEFEF;">Basic XSS</td>
<td  style="background-color:#EFEFEF;">&quot;&lt;script&gt;alert(&#x27;XSS&#x27;)&lt;/script&gt;&quot;</td>
</tr>
<tr>
<td  style="background-color:#EFEFEF;">Basic SQL Injection</td>
<td  style="background-color:#EFEFEF;">&quot;&#x27; OR &#x27;1&#x27;=&#x27;1&quot;</td>
</tr>
<tr>
<td rowspan='4' style="">Input Character Tests</td>
<td  style="">Non-ASCII Characters</td>
<td  style="">&quot;José&quot; or &quot;Åqsa&quot;</td>
</tr>
<tr>
<td  style="">Other Characters Than Alphabetic</td>
<td  style="">&quot;John123&quot; or &quot;John@Wick&quot;</td>
</tr>
<tr>
<td  style="">Maximum Values</td>
<td  style="">&quot;AETDHKGHIQKLMPONQRSTUVIXBZAQ&quot;</td>
</tr>
<tr>
<td  style="">Basic Valid Input</td>
<td  style="">&quot;John&quot;</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #2 - bypass html 5 validations</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge2.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 2 - bypass html 5 validations<b> </td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">Step</td>
<td  style="font-weight:bold;text-align:center;">Action Taken</td>
<td  style="font-weight:bold;text-align:center;">Result</td>
<td rowspan='7' style="background-color:#B6D7A8;text-align:center;">Challenge Successful !! </td>
</tr>
<tr>
<td  style="">1. Opened the webpage with the form</td>
<td  style="">Opened the form in the browser</td>
<td  style="">Form loaded successfully</td>
</tr>
<tr>
<td  style="">2. Identified the input field with numeric validation</td>
<td  style="">Noticed the HTML5 validation (type=&#x27;number&#x27;)</td>
<td  style="">HTML5 validation was visible</td>
</tr>
<tr>
<td  style="">3. Opened Developer Tools in the browser using Inspect</td>
<td  style="">Right-clicked the page, selected &#x27;Inspect&#x27;</td>
<td  style="">Developer Tools opened correctly</td>
</tr>
<tr>
<td  style="">4. Modified the input field validation</td>
<td  style="">Changed the type attribute to &#x27;text&#x27; to bypass validation</td>
<td  style="">Validation was bypassed</td>
</tr>
<tr>
<td  style="">5. Entered invalid data in the input field</td>
<td  style="">Entered a non-integer value (e.g., &#x27;hello&#x27; or &#x27;123.456&#x27;)</td>
<td  style="">Form accepted invalid input</td>
</tr>
<tr>
<td  style="">6. Submitted the form successfully with invalid data</td>
<td  style="">Successfully submitted the form with invalid data</td>
<td  style="">Form was submitted without any errors</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #4 - generate testing data</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge4.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
<col style='width:168px'>
<col style='width:126px'>
<col style='width:140px'>
<col style='width:193px'>
<col style='width:202px'>
<col style='width:193px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 4 - generate testing data<b></td>
<td  style="background-color:#B6D7A8;text-align:center;">Challenge Successful !!</td>
<td  style=""></td>
<td  style=""></td>
<td  style=""></td>
<td  style=""></td>
<td  style=""></td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">CNP</td>
<td  style="font-weight:bold;text-align:center;">Details of CNP</td>
<td  style="font-weight:bold;text-align:center;">Control Number Calculations</td>
<td rowspan='7' style="">1st Digit  (Gender and Time Period)<br><br>This digit give info about the gender and when the person was born<br><br>1 - Male, born between 1900 - 1999.<br>2 - Female, born between 1900 - 1999.<br>3 - Male, born between 1800 - 1899.<br>4 - Female, born between 1800 - 1899.<br>5 - Male, born between 2000 - 2099.<br>6 - Female, born between 2000 - 2099.<br>7 - Foreigner, male.<br>8 - Foreigner, female.<br>9 - Unknown gender, Not- Resident.</td>
<td rowspan='7' style="">2nd and 3rd Digits (Year of Birth)<br><br>These two digits give info about the last two digits of the year of birth:<br><br>Ex: If born in 1985, it will be 85.<br>Ex: If born in 2003, it will be 03.</td>
<td rowspan='7' style="">4th and 5th Digits ( Month of Birth )<br><br>These digits tgive info about the month of birth :<br><br>Ex:<br>01 - January<br>02  - February<br>12 - December</td>
<td rowspan='7' style="">6th and 7th Digits - Day of Birth<br><br>These two digits give info about the day of birth:<br><br>Ex:<br>01 - 1st day of  month.<br>15  - 15th day of month.</td>
<td rowspan='7' style="">8th and 9th Digits - Area Code<br><br>These digits give info about pincode of place of birth<br><br>Ex:<br><br>01 – Bucharest<br>02 – Arad<br><br>The exact area codes can be range from 01 to 52.</td>
<td rowspan='7' style="">10th to 12th Digits - Order Number<br><br>These three digits give infoabout number of order per DAY<br><br>Ex: <br>001 is the first person registered that day.<br><br>456 could be the 456th person registered that day.</td>
<td rowspan='7' style="">13th Digit – Control Number<br><br>This is a number to ensure the CNP is valid and calculated using the first 12 digits and the following formula:<br><br>Multiply each of the first 12 digits by a specific sequence:<br><br>2x Digit 1 + ,  7x Digit 2 + ,  9, 1, 4, 6, 3, 5, 8, 2, 7, 9. wagera wagera<br><br>Then Mod by 11, remainder is Control Number.</td>
</tr>
<tr>
<td  style="text-align:center;">1850415010013</td>
<td  style="">1 - Male born between 1900 -1999.<br>85 -  Born in 1985.<br>04 -April.<br>15 - 15th day.<br>01 - Bucharest area.<br>001 - First record for that day.<br>3 - Control digit .</td>
<td  style="text-align:left;">(1×2) + (8×7) + (5×9) + (0×1) + (4×4) + (1×6) + (5×3) + (0×5) + (1×8) + (0×2) + (0×7) + (1×9)<br>= 2 + 56 + 45 + 0 + 16 + 6 + 15 + 0 + 8 + 0 + 0 + 9 = 157 Mod 11 = 3</td>
</tr>
<tr>
<td  style="text-align:center;">2990621010024</td>
<td  style="">2 - Female born between 1900 -1999.<br>99 -  Born in 1999.<br>06 -  June.<br>21 -  21st day.<br>01 -  Bucharest area.<br>002 -  Second record for that day.<br>4 -  Control digit.</td>
<td  style="">(2×2) + (9×7) + (9×9) + (0×1) + (6×4) + (2×6) + (1×3) + (0×5) + (1×8) + (0×2) + (0×7) + (2×9)<br>= 4 + 63 + 81 + 0 + 24 + 12 + 3 + 0 + 8 + 0 + 0 + 18 = 213 Mod 11 =4</td>
</tr>
<tr>
<td  style="text-align:center;">1980324010013</td>
<td  style="">1 - Male born between 1900 - 1999.<br>98 -  Born in 1998.<br>03 - March.<br>24 - 24th day.<br>01 - Bucharest area.<br>001 - First record for that day.<br>3 - Correct control digit (calculated).</td>
<td  style="">(1×2) + (9×7) + (8×9) + (0×1) + (3×4) + (2×6) + (4×3) + (0×5) + (1×8) + (0×2) + (0×7) + (1×9)<br>= 2 + 63 + 72 + 0 + 12 + 12 + 12 + 0 + 8 + 0 + 0 + 9 = 190 Mod 11 = 3</td>
</tr>
<tr>
<td  style="text-align:center;">3030415010044</td>
<td  style="">3 - Male born between 1800 -1899.<br>03 - Born in 1803.<br>04 - April.<br>15 - 15th day.<br>01 - Bucharest area.<br>004 - Fourth record for that day.<br>4 - Correct control digit (calculated).</td>
<td  style="">(3×2) + (0×7) + (3×9) + (0×1) + (4×4) + (1×6) + (5×3) + (0×5) + (1×8) + (0×2) + (0×7) + (4×9) = 6 + 0 + 27 + 0 + 16 + 6 + 15 + 0 + 8 + 0 + 0 + 36 = 114 Mod 11 = 4</td>
</tr>
<tr>
<td  style="text-align:center;">2991223010053</td>
<td  style="">2 - Female born between 1900 -1999.<br>99 - Born in 1999.<br>12 - December.<br>23 - 23rd day.<br>01 - Bucharest area.<br>005 - Fifth record for that day.<br>3 - Control digit (calculated).</td>
<td  style="">(2×2) + (9×7) + (9×9) + (1×1) + (2×4) + (2×6) + (3×3) + (2×5) + (3×8) + (0×2) + (0×7) + (5×9)<br>= 4 + 63 + 81 + 1 + 8 + 12 + 9 + 10 + 24 + 0 + 0 + 45 = 157 Mod 11 = 3</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #5 - using a web analytics engine</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge5.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:168px'>
</colgroup>
<tr>
<td  style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 5 - using a web analytics engine<b></td>
<td rowspan='3' style="background-color:#FFD966;text-align:center;">Challenge Incomplete !!</td>
</tr>
<tr>
<td rowspan='2' style="">NEED TO BE DONE BY SELF, Consider following question before solving.<br>- What is this asking for?<br>- What am supposed to expect<br>- How am I supposed to do this?</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #6 - Boundary testing</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge6.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
<col style='width:168px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 6 - Boundary testing<b> </td>
<td  style=""></td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;"></td>
<td  style="font-weight:bold;text-align:center;">Input</td>
<td  style="font-weight:bold;text-align:center;">Issue</td>
<td  style="font-weight:bold;text-align:center;">Challenge&#x27;s Test &#x27;s Response</td>
<td rowspan='17' style="background-color:#FFE599;text-align:center;">Challenge Incomplete !!</td>
</tr>
<tr>
<td  style="text-align:left;">1</td>
<td  style="text-align:left;">2016-12-31 23:59:00</td>
<td  style="text-align:left;">Below the minimum year range</td>
<td  style="background-color:#FFFFFF;">First date before 2017, December 2016 23:59</td>
</tr>
<tr>
<td  style="text-align:left;">2</td>
<td  style="text-align:left;">2018-01-01 00:00:00</td>
<td  style="text-align:left;">Above the maximum year range</td>
<td  style="text-align:left;">First date after 2017, January 2018 00:00<br></td>
</tr>
<tr>
<td  style="text-align:left;">3</td>
<td  style="text-align:left;">2017-01-20 14:20:00</td>
<td  style="text-align:left;">Exactly 1-hour advance</td>
<td  style="text-align:left;">Date less than 1 hour<br></td>
</tr>
<tr>
<td  style="text-align:left;">4</td>
<td  style="text-align:left;">29/02/2017 12:00</td>
<td  style="text-align:left;">Invalid leap year date</td>
<td  style="text-align:left;">Inexistent date 29 for February 2017<br></td>
</tr>
<tr>
<td  style="text-align:left;">5</td>
<td  style="text-align:left;">31/04/2017 12:00</td>
<td  style="text-align:left;">Invalid day for April</td>
<td  style="text-align:left;">31 days for 30 days months<br></td>
</tr>
<tr>
<td  style="text-align:left;">6</td>
<td  style="text-align:left;">32/01/2017 12:00</td>
<td  style="text-align:left;">Non - existent day</td>
<td  style="text-align:left;">32 days for 31 days months<br></td>
</tr>
<tr>
<td  style="text-align:left;">7</td>
<td  style="text-align:left;">20/13/2017 12:00</td>
<td  style="text-align:left;">Invalid month</td>
<td  style="text-align:left;">Higher limit for the month 13<br></td>
</tr>
<tr>
<td  style="text-align:left;">8</td>
<td  style="text-align:left;">00/01/2017 12:00</td>
<td  style="text-align:left;">Zero as a day</td>
<td  style="text-align:left;">Date with day = zero<br></td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #7 - Scenario Testing</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge7.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:259px'>
</colgroup>
<tr>
<td colspan='2' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 7 - Scenario Testing<b></td>
</tr>
<tr>
<td  style="">Danish Masood, a passionate QA intern at blackcurrant, was tasked with testing a new administrator portal for an online E-Turf booking and management platform. He followed agile testing practices, while working closely with developers to ensure each sprint is delivered promptly and accurately. Inspired by the principles of software craftsmanship, Danish suggested his teams of focusing on unit testing for critical features like user management and permissions.  His active approach caught several bugs early in the development phase, saving the team from last-minute chaos and time vulnerability.<br><br>By the end of the project, Danish’s efforts impressed the team, and the administrator portal was launched successfully, showcasing his growing expertise in QA.</td>
<td  style="background-color:#B6D7A8;text-align:center;">Challenge Successful !!</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #8 - State Transition</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge8.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
<col style='width:168px'>
<col style='width:126px'>
<col style='width:140px'>
<col style='width:193px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 8 - State Transition<b></td>
<td  style=""></td>
<td  style=""></td>
<td  style=""></td>
<td  style=""></td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">State</td>
<td  style="font-weight:bold;text-align:center;">Selling</td>
<td  style="font-weight:bold;text-align:center;">Description</td>
<td  style="font-weight:bold;text-align:center;">Start Date</td>
<td  style="font-weight:bold;text-align:center;">End Date</td>
<td  style="font-weight:bold;text-align:center;">Action</td>
<td  style="font-weight:bold;text-align:center;">Result</td>
<td rowspan='5' style="background-color:#B6D7A8;text-align:center;">Challenge Sucessful !!</td>
</tr>
<tr>
<td  style="">Saved</td>
<td  style="">Potato</td>
<td  style="">A highly fibrous vegetable root that grows under the ground.</td>
<td  style="">11:00:00</td>
<td  style="">12:00:00</td>
<td  style="">Delete</td>
<td  style="">Successfully deleted.</td>
</tr>
<tr>
<td  style="">In Progress</td>
<td  style="">Sweet Potato</td>
<td  style="">A highly glutenous vegetable root that grows under the ground.</td>
<td  style="">09:45:00</td>
<td  style="">11:00:00</td>
<td  style="">Delete</td>
<td  style="">Deletion not allowed (as expected).</td>
</tr>
<tr>
<td  style="">In Progress</td>
<td  style="">Sweet Potato</td>
<td  style="">A highly glutenous vegetable root that grows under the ground.</td>
<td  style="">09:45:00</td>
<td  style="">11:00:00</td>
<td  style="">Archive</td>
<td  style="">Archiving not allowed (as expected).</td>
</tr>
<tr>
<td  style="">Finished</td>
<td  style="">Bad Potato</td>
<td  style="">A highly venomous vegetable root that grows under the ground.</td>
<td  style="">09:48:00</td>
<td  style="">09:49:00</td>
<td  style="">Archive</td>
<td  style="">Successfully archived.</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #9 - Know your testing techniques</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge9.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
<col style='width:168px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 9 - Know your testing techniques<b></td>
<td  style=""></td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">Words</td>
<td  style="font-weight:bold;text-align:center;">Direction</td>
<td  style="font-weight:bold;text-align:center;">Letters</td>
<td  style="font-weight:bold;text-align:center;">Answer</td>
<td  style="font-weight:bold;text-align:center;">Description</td>
</tr>
<tr>
<td  style="text-align:center;">COMPLIANCETESTING</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">17</td>
<td  style="text-align:center;">Compliance Testing</td>
<td  style="">Testing techniques used to assess if the product meets certain standards.</td>
</tr>
<tr>
<td  style="text-align:center;">GLOBALIZATIONTESTING</td>
<td  style="text-align:center;">Across</td>
<td  style="text-align:center;">20</td>
<td  style="text-align:center;">Globalization Testing</td>
<td  style="">Testing technique used when a product has customers all over the world.</td>
</tr>
<tr>
<td  style="text-align:center;">PERFORMANCETESTING</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">18</td>
<td  style="text-align:center;">Performance Testing</td>
<td  style="">Testing technique used to evaluate if software and hardware are in tune.</td>
</tr>
<tr>
<td  style="text-align:center;">USABILITYTESTING</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">16</td>
<td  style="text-align:center;">Usability Testing</td>
<td  style="">Technique concerned with the ease of use for a product.</td>
</tr>
<tr>
<td  style="text-align:center;">SECURITYTESTING</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">15</td>
<td  style="text-align:center;">Security Testing</td>
<td  style="">Testing technique investigating threats such as viruses.</td>
</tr>
<tr>
<td  style="text-align:center;">PORTABILITYTESTING</td>
<td  style="text-align:center;">Across</td>
<td  style="text-align:center;">18</td>
<td  style="text-align:center;">Portability Testing</td>
<td  style="">Ensures the application can function on different platforms.</td>
</tr>
<tr>
<td  style="text-align:center;">SMOKETESTING</td>
<td  style="text-align:center;">Across</td>
<td  style="text-align:center;">12</td>
<td  style="text-align:center;">Smoke Testing</td>
<td  style="">Testing technique named after testing pipelines or electronic circuits.</td>
</tr>
<tr>
<td  style="text-align:center;">BOUNDARYVALUEANALYSIS</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">21</td>
<td  style="text-align:center;">Boundary Value Analysis</td>
<td  style="">Focuses on testing valid and invalid limits.</td>
</tr>
<tr>
<td  style="text-align:center;">MONKEYTESTING</td>
<td  style="text-align:center;">Across</td>
<td  style="text-align:center;">13</td>
<td  style="text-align:center;">Monkey Testing</td>
<td  style="">Testing technique related to randomness, inspired by the animal.</td>
</tr>
<tr>
<td  style="text-align:center;">STATETRANSITION</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">15</td>
<td  style="text-align:center;">State Transition Testing</td>
<td  style="">Focuses on checking how objects change their state during application operation.</td>
</tr>
<tr>
<td  style="text-align:center;">USEREXPERIENCE</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">14</td>
<td  style="text-align:center;">User Experience Testing</td>
<td  style="">Concerned with all aspects of how a product is experienced by a user.</td>
</tr>
<tr>
<td  style="text-align:center;">GUITESTING</td>
<td  style="text-align:center;">Down</td>
<td  style="text-align:center;">10</td>
<td  style="text-align:center;">GUI Testing</td>
<td  style="">Testing that focuses only on the end result visible to the user.</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #10 - BUG HUNT - Part 01</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge10.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 10 - BUG HUNT - Part 01<b></td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">Defect Numbers </td>
<td  style="font-weight:bold;text-align:center;">Input</td>
<td  style="font-weight:bold;text-align:center;">Defect information</td>
<td  style="font-weight:bold;text-align:center;">Advices from GPT (Got these with GPTs assistances)</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">1</td>
<td  style="">&lt;script&gt;alert(&#x27;XSS&#x27;)&lt;/script&gt; or &#x27;; DROP TABLE users;--</td>
<td  style="">Special characters like &lt;, &gt;, /, ; are allowed in the form fields.</td>
<td  style="">Check if characters like &lt; or ; cause any issues (like breaking the form).</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">2</td>
<td  style="">John (space) or Wick (space)</td>
<td  style="">The form doesn’t remove spaces before or after the input.</td>
<td  style="">See if spaces at the start or end of the text are causing issues when entering data.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">3</td>
<td  style="">😀😆 or ñ (Unicode or non-ASCII characters)</td>
<td  style="">The form lets you enter emojis or other non-standard characters.</td>
<td  style="">Test if the form should reject things like emojis or weird symbols.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">4</td>
<td  style="">user@example.com (already registered email)</td>
<td  style="">The form lets you register with a username or email that’s already registerd.</td>
<td  style="">Try registering with a username or email that’s already in the system and see if it stops you.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">5</td>
<td  style=""> OR &#x27;1&#x27;=&#x27;1</td>
<td  style="">The form accepts SQL commands, which can cause security issues.</td>
<td  style="">Try entering SQL commands like &#x27; OR &#x27;1&#x27;=&#x27;1 in the username and password fields to check for security holes.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">6</td>
<td  style="">password123 (check for plaintext)</td>
<td  style="">The form sends or stores passwords without encryption.</td>
<td  style="">Check if the password is visible or sent in a way that could be easily intercepted.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">7</td>
<td  style="">Submit with invalid input empty, incorrect format</td>
<td  style="">The system shows too much error info, like internal messages or technical details.</td>
<td  style="">Try submitting incorrect info and see if it reveals any sensitive server information.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">8</td>
<td  style="">john.wick@kalakhatta.com, password123</td>
<td  style="">The form doesn’t store or show input correctly in the database.</td>
<td  style="">Check if the data entered (name, email, password) shows up correctly in the database.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">9</td>
<td  style="">NULL, empty fields, or missing values</td>
<td  style="">The form or database doesn’t handle missing or incomplete data properly.</td>
<td  style="">Test by leaving out some details (like the last name or email) and see how the system reacts.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">10</td>
<td  style="">created_on  and last_updated  = non</td>
<td  style="">Dates and times (created_on, last_updated) are missing or wrong in the database.</td>
<td  style="">Test if the timestamps are saved and displayed right in the database.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">11</td>
<td  style="">Refresh page after registration</td>
<td  style="">After registering, refreshing the page causes the user to disappear from the system.</td>
<td  style="">Check if the data is still there after refreshing or restarting the app.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">12</td>
<td  style="">Leave required fields blank and click &quot;Submit&quot;</td>
<td  style="">The &quot;Submit&quot; button stays active even when fields are missing.</td>
<td  style="">Make sure the &quot;Submit&quot; button only works when all the fields are filled correctly.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">13</td>
<td  style="">invalid email or leave a field blank</td>
<td  style="">The form doesn’t show proper error messages for invalid or incomplete fields.</td>
<td  style="">Try submitting wrong info (like an email without @) and see if the right message shows up.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">14</td>
<td  style="">Resize browser window</td>
<td  style="">The screen layout doesn’t adjust correctly when the screen is resized.</td>
<td  style="">Test how the form looks on different screen sizes by resizing the browser or using mobile mode.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">15</td>
<td  style="">john.wick@example.com, password123 (registered user)</td>
<td  style="">Registered users can’t log in properly.</td>
<td  style="">Try logging in with a user that’s already registered to see if login works as expected.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">16</td>
<td  style="">Keep the session idle for an extended time (15 minutes)</td>
<td  style="">The session doesn’t automatically log out after a certain time.</td>
<td  style="">Leave the app idle for a while and see if it logs you out after a period of inactivity.</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">17</td>
<td rowspan='5' colspan='3' style="font-weight:bold;text-align:center;">Not able to get anything about these five. </td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">18</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">19</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">21</td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">20</td>
</tr>
</table></div></div>
<div class='challenge'>

<h2>Testing Challenge #10 - BUG HUNT - Part Two</h2>

<p><strong>Website:</strong> <a href="http://testingchallenges.thetestingmap.org/challenge10submitreport.php" target="_blank">testingchallenges.thetestingmap.org</a></p>
 

<div class='table-wrap'><table class='sheet'><colgroup>
<col style='width:200px'>
<col style='width:269px'>
<col style='width:318px'>
<col style='width:259px'>
</colgroup>
<tr>
<td colspan='4' style="background-color:#D0E0E3;text-align:center;"><b>Testing Challenge 10 - BUG HUNT - Part Two<b></td>
</tr>
<tr>
<td  style="font-weight:bold;text-align:center;">Category</td>
<td  style="font-weight:bold;text-align:center;">Number</td>
<td  style="font-weight:bold;text-align:center;">Description</td>
<td  style="font-weight:bold;text-align:center;">Notes</td>
</tr>
<tr>
<td  style="font-weight:bold;">Top 5 Bugs</td>
<td  style="text-align:center;">1</td>
<td  style="text-align:left;">SQL Injection Vulnerability</td>
<td  style="">Fields accept SQL injection queries in passwords and other fields, creating a major security issue</td>
</tr>
<tr>
<td  style="font-weight:bold;"></td>
<td  style="text-align:center;">2</td>
<td  style="text-align:left;">Duplicate User Registrations</td>
<td  style="">The form allows already registered values to be registered again, indicating a lack of uniqueness validation.</td>
</tr>
<tr>
<td  style="font-weight:bold;"></td>
<td  style="text-align:center;">3</td>
<td  style="text-align:left;">No Error Messages</td>
<td  style="">Missing error feedback for duplicate registrations, incomplete fields, and invalid input formats creates confusion.</td>
</tr>
<tr>
<td  style="font-weight:bold;"></td>
<td  style="text-align:center;">4</td>
<td  style="text-align:left;">&quot;Only-Space&quot; Input Accepted</td>
<td  style="">Fields for First Name, Last Name, and Username accept inputs consisting of only spaces, which is invalid.</td>
</tr>
<tr>
<td  style="font-weight:bold;"></td>
<td  style="text-align:center;">5</td>
<td  style="text-align:left;">Database Data Missing</td>
<td  style="">Database does not show values in the :active, created_on, and created_by_id fields, impacting tracking and auditability.</td>
</tr>
<tr>
<td  style="font-weight:bold;">Top 5 Issues</td>
<td  style="text-align:center;">1</td>
<td  style="text-align:left;">Form Validation Inadequacies</td>
<td  style="">First Name accepts numbers and special characters, violating typical input standards for this field.</td>
</tr>
<tr>
<td  style=""></td>
<td  style="text-align:center;">2</td>
<td  style="text-align:left;">Password Field Design</td>
<td  style="">The password text field is poorly bordered, impacting user experience and usability.</td>
</tr>
<tr>
<td  style=""></td>
<td  style="text-align:center;">3</td>
<td  style="text-align:left;">Non-ASCII Input Acceptance</td>
<td  style="">The form accepts non-ASCII values, which might need improvement depending on localization and character set requirements.</td>
</tr>
<tr>
<td  style=""></td>
<td  style="text-align:center;">4</td>
<td  style="text-align:left;">Whitespace Handling</td>
<td  style="">Leading/trailing spaces are not trimmed in input fields, allowing for potential inconsistencies in the database.</td>
</tr>
<tr>
<td  style=""></td>
<td  style="text-align:center;">5</td>
<td  style="text-align:left;">Localization Missing/Error Messages</td>
<td  style="">If the form is expected to support multiple languages, it lacks necessary translations for error feedback.</td>
</tr>
</table></div></div>