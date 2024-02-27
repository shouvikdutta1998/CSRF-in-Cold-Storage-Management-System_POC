# Exploit Title: Simple Cold Storage Management System v1.0 - Stored XSS in "Storage List Page" 
# Exploit Author: Shouvik Dutta
# Vendor Name: oretnom23 
# Vendor Homepage: https://www.sourcecodester.com/php/15088/simple-cold-storage-management-system-using-phpoop-source-code.html
# Software Link: https://www.sourcecodester.com/php/15088/simple-cold-storage-management-system-using-phpoop-source-code.html
# Version: v1.0
# Tested on: Windows 11, Apache


## A stored Cross-Site Scripting (XSS) vulnerability has been identified in SourceCodester Simple Cold Storage Management System 1.0, specifically occurring post-admin login during the "add new storage" process. This vulnerability allows improper input at the "Name of the Storage parameter" parameter, resulting in a Cross-Site Scripting vulnerability.

## Vulnerable Parameters:  Name of Storage

##Steps:
1. Access the admin portal by logging in.
2. Go to the Storage List section.
3. Select "Add New Storage."
4. Inject an XSS payload (</script>alert(1)</script>) into the "Name of Storage" parameter.
5. The stored XSS will trigger, displaying the input provided by the attacker.
