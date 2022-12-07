# security-engineer-10

An application log’s data, including customer identifiers such as email addresses, needs to be redacted. However, these logs also include the email addresses of internal developers from company.com, and these should NOT be redacted. Which solution should you use to meet these requirements?

A. Create a regular custom dictionary detector that lists a subset of the developers' email addresses.

B. Create a regular expression (regex) custom infoType detector to match on @company.com.

C. Create a regular custom dictionary detector to match all email addresses listed in Cloud Identity.

D. Create a custom infoType called COMPANY_EMAIL to match @company.com.

## Feedback

A is not correct because as all company.com email addresses are sensitive and should be filtered. A static list is hard to maintain and can easily miss sensitive data.

B is correct because the regex will detect all company.com email addresses that need to be protected and written to the log file.

C is not correct because as the user base in Cloud Identity might only be a subset of all emails that need to be protected.

D is not correct because you need to specify a detector within the custom infoType and the detector should be a regular expression to match all @comapny.com email addresses.

https://cloud.google.com/dlp/docs/infotypes-reference

https://cloud.google.com/dlp/docs/creating-custom-infotypes