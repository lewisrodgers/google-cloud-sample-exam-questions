# security-engineer-16

You need to perform a vulnerability scan for an App Engine app using Web Security Scanner. Upon completion of the scan, the report is not producing the expected number of webpage results. The pages in the app with mouseover menus are missing from the report. Which action should you take to make sure the scan completes and captures the menu?

A. Verify the Excluded URLs.

B. Modify the scan schedule to return new results.

C. Change the scan to include additional Starting URLs.

D. Adjust the Google account on which the scan is running.

## Feedback

A is not correct because the missing webpages in mouseover menu are unlikely to be explicitly excluded since they’re expected to be scanned.

B is not correct because changing the scan schedule will not result in scanning of more webpages.

C is correct because Web Security Scanner may not be able to navigate through complex JavaScript such as a mouseover-driven multilevel menu. Specifying additional starting URLs can increase scan coverage in this scenario.

D is not correct because changing the Google account will not result in scanning of more webpages.

https://cloud.google.com/security-scanner/docs/scanning