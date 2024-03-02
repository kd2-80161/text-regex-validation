# Introduction

Javascript library to validate texts

# Installation

```npm i text-regex-validation```

## How It work
Call below function and pass your String and regexType (From below TABLE regexType must be same as name in the table accordin to requirment) it will return true or false(Boolean).

```  validateString(inputString, regexType) ```

| Name | Description 
| ------ | ------ |
| email | This is for validation of E-mail pattern like {abc121@xyz.com} |
| URL | This is for validation of URL pattern like {https://chat.openai.com}|
|Date |This is for validation of Date in pattern like {YYYY-MM-DD} |
| Username | This is for validation of Username (Alphanumeric with underscores, hyphens, or periods) |
| Time | This is for validation of Time (HH:MM 24-hour format) |
| IPv4 | This is for validation of IPv4 Address |
| IPv6 | This is for validation of IPv6 Address |
| CreditCard | This is for validation of Credit Card Number (Visa, MasterCard, American Express, Discover) |
| HTML | This is for validation of HTML Tags|
| ZIP | This is for validation of ZIP Code (U.S.) |
| Phone | This is for validation of Phone number like {+91{6 - 14 digits are allowed}} |
| Pin | This is for validation of pin code |
| name | This is for validation of name |
| password |This is for validation of password|
| aadhar | This is for validation of aadhar |
| userName | This is for validation of userName |


And Call it as function with parameter

```validateString(text, regextType)```


# Example

```validateString("example@example.com", 'email')```

# Usage

`node`

```js
       return regexPatterns[regexType].test(inputString);
```

# Build

```npm run build```

# Contribute

If you would like to contribute your most welcome. clone the repository.