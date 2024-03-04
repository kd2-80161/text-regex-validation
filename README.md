# text-regex-validation  ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-green.svg)
## Introduction
This package includes the following functionalities

- **Text Validation:** This could include checks for length, presence of certain characters, format requirements (like email addresses or phone numbers), or any other rules you need.

- **Log Analysis:** For analyzing logs, you might want to create functions that parse log files and extract relevant data.

- **Search and Replace:** Implement functions that perform search and replace operations on strings..

- **URL Parsing:** Create functions that parse URLs into their component parts. Regular expressions can help with this by matching different parts of the URL (protocol, domain, path, query parameters, etc.) and extracting them into separate variables or objects.

## Installation

```bash
npm install text-regex-validation
```

OR

```bash
npm i text-regex-validation
```

## Usage Guidelines

### **Text Validation:**

To validate string you have to Call below function

```.js
validateString(inputString, regexType) //string and regextype from table
```

__regexType name must be same__

it will return **true or false(Boolean)**.

### TABLE

| regexType name | Input String Example | Description |
|:------:|:------:|:--:|
| email | `abc121@xyz.com` | This is for validation of E-mail pattern like {abc121@xyz.com} |
| URL | `https://chat.openai.com` | This is for validation of URL pattern like {https://chat.openai.com} |
| Date | `2024-03-04` | This is for validation of Date in pattern like {YYYY-MM-DD} |
| Username | `username_123` | This is for validation of Username (Alphanumeric with underscores, hyphens, or periods) |
| Time | `14:30` | This is for validation of Time (HH:MM 24-hour format) |
| IPv4 | `192.168.1.1` | This is for validation of IPv4 Address |
| IPv6 | `2001:0db8:85a3:0000:0000:8a2e:0370:7334` | This is for validation of IPv6 Address |
| CreditCard | `4111111111111111` | This is for validation of Credit Card Number (Visa, MasterCard, American Express, Discover) |
| HTML | `<tag>content</tag>` | This is for validation of HTML Tags|
| ZIP | `12345` or `12345-6789` | This is for validation of ZIP Code (U.S.) |
| Phone | `+911234567890` | This is for validation of Phone number like {+91{6 - 14 digits are allowed}} |
| Pin | `123456` | This is for validation of pin code |
| name | `John Doe` | This is for validation of name |
| password | `P@ssw0rd` | This is for validation of password |
| aadhar | `1234 5678 9101` | This is for validation of aadhar |
| userName | `username123` | This is for validation of userName |

<!--
```.js
import {validateString,analyzeLog, searchAndReplace,parseUrl} from 'text-regex-validation'
validateString(inputString, regexType)
analyzeLog(YourLogText)
// Log Example :- // let logTexts = '[2024-03-03 10:15:30] ERROR: Failed to connect to database'\
searchAndReplace(fullText, SearchText, replaceText) 
parseUrl(YourURL)
```
-->

### **Log Analysis:**

### **Search and Replace:**

### **URL Parsing:**

# Example

```.js
import {validateString,analyzeLog, searchAndReplace,parseUrl} from 'text-regex-validation'

validateString("example@example.com", 'email')

analyzeLog('[2024-03-03 10:17:20] ERROR: Invalid username or password')

searchAndReplace('This is sample data', 'is', 'not')

parseUrl('https://www.example.com:8080/path/to/page?param1=value1&param2=value2#section1')
```

# Usage
`node`

```js
return regexPatterns[regexType].test(inputString);
```

# Build
```bash
npm run build
```

# Contribute

If you would like to contribute your most welcome. Clone the repository.
