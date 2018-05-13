# GST waf - Web Application Firewall
Original Free Web Application Firewall, Open-Source.

# Features

- [x] XSS Vulns Fixed.
- [x] SQL Injection Fixed.
- [x] Anti-Cookie-Steal Method.
- [x] HTML Malicious Code's Vulns Fixed.
- [x] CSRF Easy to use, and validation.
- [x] Block HTML Upgraded.
- [x] Lightweight.
- [x] Array Support, All Bypass fixed.
- [x] Advanced Bot validation, Browser Validation.
- [x] Most Poc's SQLi and XSS.
- [x] Security upgraded.
- [x] Errors supression.
- [x] Cloudflare and BlazingFast Support.

# Sample Usage
```php
// Before all your code starts.
require('gwaf.php');
$gwaf = new gwaf();
$gwaf->start();
// Your code below.
```
# Advanced Usage
```php
// Before of all your CODE.
require('gwaf.php');
$gwaf = new gwaf();
// Cloudflare Mode [Optional]
$gwaf->useCloudflare();
// BlazingFast Mode [Optional]
$gwaf->useBlazingfast();
// Use Own IP Header [Optional]
$gwaf->customIPHeader('IP-Header');
// Anti-Cookie-Steal Method [Optional]
$gwaf->antiCookieSteal('username'); // For trigger if on PHPSESSID is logged.

// Check separated types.
$gwaf->checkGET();
$gwaf->checkPOST();
$gwaf->checkCOOKIE();
// Your code below.
```
# CSRF Validation Example
Please read test.php

# Requirements

- [x] Min: PHP5.3 (With common functions)
