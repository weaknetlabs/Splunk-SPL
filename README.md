# Splunk> SPL Cheat Sheets
Welcome to my set of cheat sheets for Splunk> SPL. In these sheets, you will find commonly used SPL queries and syntax.
* [common-spl.md](https://github.com/weaknetlabs/Splunk-SPL/blob/master/common-spl.md) - This file contains commonly used SPL Syntax and Commands.
* [web-security-spl.md](https://github.com/weaknetlabs/Splunk-SPL/blob/master/web-security-spl.md) - This file contains commonly used SPL for incident detection and response of the [OWASP Top 10 Web Application Attacks](https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project).

# How to fetch only top 10 records and stops query execution as soon as we get 10 records

index="xyz" | streamstats count as total | search total<=10 | head 10
