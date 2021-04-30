# BackbaseAssignment

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.2.9.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Components

1. `Logo Component` - Used to display the logo on the top header of the page.
2. `Make Transfer Component` - Used to display the Make Transfer section. It follow the below criteria:
    ```shell
    a. "From account" field should be prefilled with my account details and disabled
    b. There should not be any validations on "To account" input field except it is a mandatory field.
    c. Following field validations should exist on "Amount" input field
        i.  It is a mandatory field
        ii. Negative numbers are not allowed
        iii. Decimals are permitted ( 2 places )
        iv. It should not allow amount below the total balance of -€500  
    ```
3. `Submit Button Component` - Used to submit the transaction.  
4. `Transaction Item Component` - Transactions list should be sorted by date in descending order. 
5. `Filter Component` - Used to filter the transaction list on the basis of merchant name.
6. `Footer Component` - Used to display the footer at the bottom of the page.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running lint

Run `ng lint` to execute the lint.

## Assumptions

1. `Make transfer form validation` - Best practice is to manage validation inside template but as mentioned into the user story that do not make any changes in provided UI Component, so not able to do any changes in Submit button, due to which move validation from template to ts.
2. `Frontend Technical Assignment` - Not showing, assuming this is only for showing purpose.
3. `Transactions List Data` - Implementation is like first hit the provided transaction url and if that url is not providing the result, so fetch data from json file.  