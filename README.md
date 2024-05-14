**TK905 SMS Commands List (Version 1.0)**

| Item                        | SMS format for setting                    | Reply           | Example                     | Description                                                    |
|-----------------------------|-------------------------------------------|-----------------|-----------------------------|----------------------------------------------------------------|
| **GPRS ON**                 | GPRS+123456                               | GPRS ok         | GPRS123456                  | Open GPRS                                                      |
| **GPRS OFF**                | noGPRS+123456                             | no GPRS ok      | noGPRS123456                | Shut GPRS                                                      |
| **Set APN**                 | apn+123456+apn content                    | apn ok          | apn123456 apn               | Set APN (old one will be replaced)                             |
| **APN user**                | apnuser+123456+space+content              | apnuser ok      | apnuser123456 user          | Set APN username (if without, please ignore)                   |
| **APN password**            | apnpasswd+123456+space+content            | apnpasswd ok    | apnpasswd123456 password    | Set APN password (if without, please ignore)                   |
| **Set authorized number**   | admin+123456+space+number                 | admin ok        | admin123456 13417411616     | Set authorized number; only these numbers can control the unit |
| **NO authorized number**    | noadmin+123456+space+number               | noadmin ok      | noadmin123456 13417411616   |                                                               |
| **Set password**            | password+old 123456+space+new 123456      | password ok     | password 123456 666888      | Set password                                                   |
| **Retrieve password**       | cpwd                                      | old pwd:123456  | cpwd                        |                                                               |
| **Timezone**                | timezone+123456+space+GMT No.             | time ok         | timezone123456 -4           | Set GMT time zone number. (default: 0)                         |
| **Monitor mode**            | monitor123456                             | monitor ok      | monitor123456               | Switch to the monitor mode. You will hear sounds near the unit after you call it|
| **Tracking mode**           | tracker123456                             | tracker ok      | tracker123456               | Switch to the tracking mode, you will get geo-info after you call it|
| **SMS Tracker**             | G+123456                                  |                 | G123456#                    | Latitude & longitude query                                     |
| **Sleep mode by time**      | sleep+123456+space+time(10)<br>(Change interval time)| sleep time ok  | sleep123456 10              | Enter mode-sleep much power, tracker will fall asleep in 5 minutes (default: 5 minutes)|
| **Sleep mode by shock**     | sleep+123456+space+shock<br>(Change interval time)| sleep shock ok | sleep123456 shock           | Tracker will enter sleep mode after detect no shock in 5 minutes|
| **Sleep mode OFF**          | sleep+123456+space+off                    | sleep off ok    | sleep123456 off             | Tracker will continue working                                 |
| **Upload command**          | upload+123456+space+15<br>(Range:10-43200)| upload ok       | upload123456 15             | Upload information every 15 seconds (default: 120 seconds)    |
| **Shock alert ON**          | shock+password                            | shock ok        | shock123456                 | Arm                                                           |
| **Shock alert OFF**         | noshock+password                          | noshock ok      | noshock123456               | Unarm                                                         |
| **Vibrator sms alarm on/off**| vibalarm+password                        | vibalarm ok     | vibalarm123456              | Defaulted: ON                                                 |
| **Vibrator sms alarm on/off**| novibalarm+password                      | novibalarm ok   | novibalarm123456            | Alarm set OK                                                  |
| **Query parameters**        | check123456                               |                 | check123456                 | Version, ID, IP, port, domain name, APN, GPS, GSM signal, center number...|
| **AdminIP**                 | adminip+123456+space+ip+space+port        | adminip ok      | adminip123456 119.145.44.170 7700 | Set Home IP and Port of the server, and update IPs into by cell id|
| **NO AdminIP**              | noadminip+123456+space+ip+space+port      | noadminip ok    | noadminip123456             |                                                               |
| **Restore to factory**      | begin+123456                              | begin ok        | begin123456                 | Restore to factory                                             |
