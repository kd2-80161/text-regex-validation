# Introduction

Text Validation: This could include checks for length, presence of certain characters, format requirements (like email addresses or phone numbers), or any other rules you need.

Log Analysis: For analyzing logs, you might want to create functions that parse log files and extract relevant data.

 Search and Replace: Implement functions that perform search and replace operations on strings..

URL Parsing: Create functions that parse URLs into their component parts. Regular expressions can help with this by matching different parts of the URL (protocol, domain, path, query parameters, etc.) and extracting them into separate variables or objects.

# Installation

```npm install npm i text-regex-validation```

## How It work
Call below function and pass your String and regexType (From below TABLE regexType must be same as name in the table accordin to requirment) it will return true or false(Boolean).
``` import {validateString,analyzeLog, searchAndReplace,parseUrl} from 'text-regex-validation' ```

```  validateString(inputString, regexType) ```

``` analyzeLog(YorLogText) ```
 Log Example :- // let logTexts = '[2024-03-03 10:15:30] ERROR: Failed to connect to database'\
 
 ``` searchAndReplace(fullText, SearchText, replaceText) ```
 
``` parseUrl(YourURL) ```
 
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


# Example
```validateString("example@example.com", 'email')```
```analyzeLog('[2024-03-03 10:17:20] ERROR: Invalid username or password')```
```searchAndReplace('This is sample data', 'is', 'not')```
```parseUrl('https://www.example.com:8080/path/to/page?param1=value1&param2=value2#section1')```

# Usage
`node`

```js
return regexPatterns[regexType].test(inputString);
```

# Build
```npm run build```

# Contribute

If you would like to contribute your most welcome. Clone the repository.