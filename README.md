# bb-app
Backbase App - Make a transaction

## Table of contents
  1. Technologies
  2. Data load
  3. Validation and flow
  4. Color
  5. Task duration

# 1. Technologies
  - HTML5
  - CSS3 (SASS)
  	- normalize.css v7.0.0 / reset.css v2.0.0
  - jQuery v3.2.1
  - Bootstrap v4.0.0
  - Bootstrap Datatables v1.10.15
  - Google Fonts
  - Font awesome v4.7.0

  This application was developed following the 'Mobile first' approach, to achieve this and provide basic styling i made use of Bootstrap v4 framework. 

  In order to provide custom styles i made use of SASS pre-processor in order to create css modules along with clean and reusable code. Reset.css and normalize.css were used as well to initial UI set up.

  jQuery was chosen since it's needed with Bootstrap plugins, such as Bootstrap datatables, because of this and the application requirements i believe the use of jQuery provided a quick and simple solution.

  Google Fonts were used as required in specifications.

  Font Awesome was used instead of the icons provided in the design, this provides a better experience for the user, it's easier to control and customize as well as it follows the Retina ready approach. Font awesome was needed since Bootstrap 4 does not provide integrated icon pack.

# 2. Data load
  - When page loads, all data related to past transactions is presented in the datatable.

# 3. Validation and flow
  - User can only confirm a transaction if the Beneficiary input and amount input are filled (amount must be higher than 0).
  - If user wants to transfer an amount that will end in a balance below 500, warning message will be displayed and transaction must be canceled.
  - After a transacion is placed, the balance is updated, the form goes to it's initial state and the info is displayed in the datatable.
  - User can search for transaction by typing in the search field, which also has the 'clear' button on the right side. Sorting is also a feature.

# 4. Colors
  	- Depending on the transfer amount, a different color is set for each transacion (visible in te left side of each transfer row). 
  	values : > 0 , > 25 , > 60 , > 1000

# 5. Task duration
  - To complete this assignment between 4-5 hours of work were required.