# GoAutoDial-CE-3.3 - Authentication-Bypass-Command-Injection Exploit.
This script exploits a SQL injection flaw in the login functionality for GoAutoDial version 3.3-1406088000 and below, and attempts to perform command injection. This also attempts to retrieve the admin user details, including the cleartext password stored in the underlying database. Command injection will be performed with root privileges. The default pre-packaged ISO builds are available from goautodial.org. Currently, the hardcoded command injection payload is an encoded reverse-tcp bash one-liner and the handler should be setup to receive it appropriately.

- Affected software: GoAutoDial
- Affected version: 3.3-1406088000 (GoAdmin) and previous releases of GoAutodial 3.3
- Associated CVEs: CVE-2015-2842, CVE-2015-2843, CVE-2015-2844, CVE-2015-2845
- Vendor advisory: http://goautodial.org/news/21

```bash
Usage: ./goautodial_rce_exploit.sh -u <target-url> -r <lhost> -p <lport>
```
![image](https://user-images.githubusercontent.com/81138950/186477675-dd82bdd8-6632-4e47-8d29-7f7debcb7718.png)

Note:
This is just a script created from the origial exploit which automates the process of exploitation.
