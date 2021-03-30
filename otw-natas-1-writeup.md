# OverTheWire Natas Project Part #1

## Student Information

* Student name: **Michael Cox**
* NetId: **mcox59**


## Project Description

In this project, you will be complete the Natas challenges at <https://overthewire.org/wargames/natas/>. In this part of the lab, you will complete challenges Natas 0–Natas 13. For each challenge, you will complete the following worksheet describing:
1. The credentials found in the challenge.
2. How you solved the challenge. Include any JavaScript or other scripts necessary to retrieve the credentials.
3. What sins (as found in the *24 Deadly Sins* book) are evidenced in the challenge.
4. How those sins should be addressed to address your exploit.

In the workshop, the challenges are named based on the username used to login to the shell for that challenge. For example, the challenge labeled "Natas 10" will be logged into with the username natas10, and the solution will be the credentials for the user Natas11.

You can find a basic guide for markdown formatting [here](https://www.markdownguide.org/basic-syntax/). In particular, note the [code section](https://www.markdownguide.org/basic-syntax/#code) which should be used to annotate any code or commands used in your writeup.


## Hints
* Natas 11: `plaintext ^ key` gives the ciphertext. What does `plaintext ^ ciphertext` equal?


## Challenges

---
### Natas 00

#### Credentials
`natas1:gtVrDuiDfck831PqWsLEZy5gyDz1clto`

#### How you passed the challenge
* The password is stored in a comment in the html page

#### What sins are evidenced in this challenge
* [CWE-312: Cleartext Storage of Sensitive Information](https://cwe.mitre.org/data/definitions/312.html)
* [CWE-319: Cleartext Transmission of Sensitive Information](https://cwe.mitre.org/data/definitions/319.html)
* [CWE-540: Inclusion of Sensitive Information in Source Code](https://cwe.mitre.org/data/definitions/540.html)


#### How could those sins be mitigated
* Remove the password from the HTML (do not store sensitive information in any publicly accessible files)
* Use HTTPS (securely encrypt any sensitive information going through public channels)
* Securely hash passwords



---
### Natas 01

#### Credentials
`natas2:ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi`

#### How you passed the challenge
* The password is stored in a comment in the html page
  * Use browser dev tools

#### What sins are evidenced in this challenge
* [CWE-312: Cleartext Storage of Sensitive Information](https://cwe.mitre.org/data/definitions/312.html)
* [CWE-319: Cleartext Transmission of Sensitive Information](https://cwe.mitre.org/data/definitions/319.html)
* [CWE-540: Inclusion of Sensitive Information in Source Code](https://cwe.mitre.org/data/definitions/540.html)
* [CWE-656: Reliance on Security Through Obscurity](https://cwe.mitre.org/data/definitions/656.html)

#### How could those sins be mitigated
* Remove the password from the HTML (do not store sensitive information in any publicly accessible files)
* Use HTTPS (securely encrypt any sensitive information going through public channels)
* Securely hash passwords
* Use these mitigations rather than attempting to hide the vulnerability by removing functionality


---
### Natas 02

#### Credentials
`natas3:sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14`

#### How you passed the challenge
* Note that there is an `<img>` tag including a relative path to `files`
* Visit `/files`
* Notice the directory index includes `users.txt`
* View `users.txt`

#### What sins are evidenced in this challenge
* [CWE-312: Cleartext Storage of Sensitive Information](https://cwe.mitre.org/data/definitions/312.html)
* [CWE-319: Cleartext Transmission of Sensitive Information](https://cwe.mitre.org/data/definitions/319.html)
* [CWE-548: Exposure of Information Through Directory Listing](https://cwe.mitre.org/data/definitions/548.html)
* [CWE-552: Files or Directories Accessible to External Parties](https://cwe.mitre.org/data/definitions/552.html)
* [CWE-732: Incorrect Permission Assignment for Critical Resource](https://cwe.mitre.org/data/definitions/732.html)

#### How could those sins be mitigated
* Use HTTPS (securely encrypt any sensitive information going through public channels)
* Securely hash passwords
* Disable automatic directory listings and hide directory listings
* Reconfigure permissions on `files` and `users.txt` so that they are not accessible by the public



---
### Natas 03

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 04

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 05

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 06

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 07

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 08

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 09

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 10

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 11

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 12

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **



---
### Natas 13

#### Credentials
** Credentials here **

#### How you passed the challenge
** Steps here **

#### What sins are evidenced in this challenge
** Sins here **

#### How could those sins be mitigated
** Mitigations here **


