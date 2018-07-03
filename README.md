# JavaScript Technical Test

The brief is simple. Create a multi-step form used to submit your CV and details to a provided endpoint via Ajax. The technology you employ is completely up to you, as long as the form submits successfully. 

The aim of this test is to assess the decisions you make along the way, including but not limited to choice of tech, engineering, and general care to user experience.

## Instructions

Create a multi-step form to allow users (yourself) to submit your CV and details

### Form fields

Details of the form fields required and any validation rules are provided below, and should be submitted using the associated field names.

| Label         | Field name    | Data type | Required? |
| ------------- |:-------------:|:---------:|:---------:|
| First name | first_name | string | :white_check_mark: |
| Last name | last_name | string | :white_check_mark: |
| Email | email | string | :white_check_mark: |
| Phone number | phone_number | string | :white_check_mark: |
| Do you live in the uk? | live_in_uk | boolean | :white_check_mark: |
| Git profile | git_profile | string | :white_check_mark: |
| Upload CV | file | string | :white_check_mark: |
| About you | about_you | string | :white_check_mark: |

### Endpoint

You should submit all of your data to the following endpoint as a `POST` request:

```
https://technical-tests.netsells.co.uk/vacancies/javascript-developer/submissions
```

This endpoint will either return a success (200) or a validation error (422) if the data provided is incorrect.

## Requirements

- Use JavaScript
- Make it work

## Bonus points

- Use of newer javascript standards (ES6+)
- Use of a javascript bundler
- An eye for design/detail
- Use of a JavaScript framework
- Tests

## FAQ

### Do I need to submit my details?

We will purely use the submitted details to ensure that the forn successfully submits, so we don't care about the legitimacy of data, however it would be helpful to see which requests came from you.

### What happens to the details I submit?

All data is deleted after 7 days.

### Are there preferences on x, y, z?

Our code standards are available [here](here) and our 
