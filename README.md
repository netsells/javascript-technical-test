# JavaScript Technical Test

The brief is simple. Create a multi-step form used to submit your CV and details to a provided endpoint via Ajax. The technology you employ is completely up to you, as long as the form submits successfully. 

The aim of this test is to assess the decisions you make along the way, including but not limited to choice of tech, engineering, and general care to user experience.

Don't worry about over-engineering, we want to see the technology you can make use of. Try and wow us.

## Instructions

Create a multi-step form to allow users (yourself) to submit your CV and details to via Ajax. All the backend work is done for you, you simply need to hit the endpoint with the data required. By "multi-step" we mean that the form should be a "flow". You complete step 1, then step 2 etc and finally submit all data collected.

### Form fields

Details of the form fields required and any validation rules are provided below, and should be submitted using the associated field names. Any other validation rules will be returned in the 422 response so be sure to handle them appropriately.

| Label         | Field name    | Data type | Required? |
| ------------- |:-------------:|:---------:|:---------:|
| First name | first_name | string | :white_check_mark: |
| Last name | last_name | string |  |
| Email | email | string | :white_check_mark: |
| Phone number | phone_number | string |  |
| Do you live in the uk? | live_in_uk | boolean | :white_check_mark: |
| Git profile | git_profile | string | :white_check_mark: |
| Upload CV | cv | string | :white_check_mark: |
| Upload Cover Letter | cover_letter | string |  |
| About you | about_you | string | :white_check_mark: |

### Endpoint

You should submit all of your data to the following endpoint as a `POST` request:

```
https://technical-tests.netsells.co.uk/vacancies/javascript-developer/submissions
```

This endpoint will either return a success (`200`) or a validation error (`422`) if the data provided is incorrect.

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

### What is this?

This is the technical test for the "frontend javascript developer" role at [Netsells](http://netsells.co.uk), a digital agency based in York, UK. If you came across this technical test in the wild, why not see if you're the [person we're looking for?](./JOB_SPEC.md)

### Do I need to submit my details?

We will purely use the submitted details to ensure that the forn successfully submits, so we don't care about the legitimacy of data, however it would be helpful to see which requests came from you.

### What happens to the details I submit?

All data is deleted after 7 days.

### Are there preferences on x, y, z?

Use whatever you like, and as said, don't worry if you feel like you're over-engineering it. Our code standards are available [here](https://netsells.github.io/code-standards/) and our linters are available [here](https://github.com/netsells/eslint-config-netsells/) and [here](https://github.com/netsells/stylelint-config-netsells/). Bonus points if you follow these.
