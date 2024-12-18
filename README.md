# Date-Picker

Test Name: Date Picker Navigation and Selection Test
Objective:
To verify the correct functioning of a jQuery UI date picker widget, focusing on the ability to navigate and select specific dates in the past or the future.

Preconditions:
Selenium WebDriver and ChromeDriver are installed and configured correctly.
Chrome browser is available on the test machine.
The target website (jQuery UI date picker demo page) is accessible.
Test Steps:
Setup WebDriver:

Initialize a ChromeDriver instance.
Set implicit wait for handling dynamic elements.
Maximize the browser window.
Open Target URL:

Navigate to the jQuery UI date picker demo page (https://jqueryui.com/datepicker/).
Switch to iFrame:

Switch context to the iframe containing the date picker widget.
Open Date Picker:

Click on the date picker input field to display the calendar.
Select Past Date:

Define the target date parameters (year = 2022, month = May, date = 30).
Use the Selectpastdate method:
Navigate through the calendar using the "Previous" arrow until the target year and month are displayed.
Select the specified date from the calendar grid.
Validate Date Selection:

Confirm that the selected date is correctly displayed in the date picker input field.
(Optional) Select Future Date:

If desired, define a future date (year = 2028, month = May, date = 12).
Use the Selectfuturedate method:
Navigate through the calendar using the "Next" arrow until the target year and month are displayed.
Select the specified date from the calendar grid.
Validate the selected date in the input field.
Close Browser:

Quit the WebDriver to close the browser.
Expected Results:
The calendar navigates correctly to the specified past or future year and month.
The date picker selects the specified date, and it is accurately displayed in the input field.
Additional Notes:
The Selectfuturedate and Selectpastdate methods rely on XPath locators and expect the calendar widget structure to remain consistent.
The test does not include assertions or error handling for invalid dates.
Enhance the test by adding validation steps, such as checking the actual value in the input field post-selection.
