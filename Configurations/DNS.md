# Priveasy's DNS Configuration

> Does something look off (outdated, incorrect, could be improved, etc.)? Please let us know! We do our best to keep these records as efficient and up-to-date as possible, but we make mistakes!

## Hosted Zone 1 (P5.vc)

|Record Name|Record Type|Record Value|TTL|Alias|Routing Policy|Differentiator|
| :------------ | :------------ | :------------ | :------------ | :------------ | :------------ | :------------ |
|p5.vc|A|webserver0.p5.vc||Yes|Weighted|200|
|p5.vc|A|webserver1.p5.vc||Yes|Weighted|50|
|database0.p5.vc|A|161.97.95.155|10800|No|Simple||
|database1.p5.vc|A|51.79.86.89|10800|No|Simple||
|docs.p5.vc|A|95.111.228.106|10800|No|Simple||
|records0.p5.vc|A|95.111.228.106|10800|No|Simple||
|webserver0.p5.vc|A|144.91.77.173|10800|No|Simple||
|webserver1.p5.vc|A|51.79.87.85|10800|No|Simple||
|p5.vc|MX|10 p5.vc|10800|No|Simple||
|p5.vc|NS|ns-1203.awsdns-22.org.<br>ns-543.awsdns-03.net.<br>ns-1779.awsdns-30.co.uk.<br>ns-80.awsdns-10.com.|172800|No|Simple||
|p5.vc|SOA|ns-1203.awsdns-22.org.<br>awsdns-hostmaster.amazon.com.<br>1 7200 900 1209600 86400|900|No|Simple||
|p5.vc|TXT|"v=spf1 mx a ip4:95.111.228.106/32 include:mail.priveasy.org -all"|10800|No|Simple||
|_dmarc.p5.vc|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|dkim._domainkey.p5.vc|TXT|"v=DKIM1; p=" "MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAv9R4IlEitEo4pyyir8G2" "IpTaRR3pxjkeo6DNU0eg/3S9rDZrblhCE43N9nBPrMLAuK5HvkCHS339ZCAe0JJm" "CCL9sdwuZGq+y+NU8hXf8NMQaj0LdtDXcpD7op21/nYtdV9vPGNhmKib2lEcEv4I" "JAMIGzsJa+OXvNYr/uycnmvpSUB1pBnkhmFcBRv542Si3XAG2oSUKSpxvgTnVHb+" "YLJBPS1W9QPbKtjJ3SVSOAdtHTHLyi567FX1pnJ83lUQPmeoeyx9eFb15t2Qpcb+" "kJTjFyXbgsWEjefLKR/CHSZa+IOctWm6pKCcnjz7Gs3F3Nh6om78XxvqY41Hiiz4" "BwIDAQAB"|3600|No|Simple||

## Hosted Zone 2 (Priveasy.org)

|Record Name|Record Type|Record Value|TTL|Alias|Routing Policy|Differentiator|
| :------------ | :------------ | :------------ | :------------ | :------------ | :------------ | :------------ |
|priveasy.org|A|webserver0.priveasy.org||Yes|Weighted|200|
|priveasy.org|A|webserver1.priveasy.org||Yes|Weighted|50|
|docs.priveasy.org|A|95.111.228.106|10800|No|Simple||
|mail.priveasy.org|A|95.111.228.106|10800|No|Simple||
|webserver0.priveasy.org|A|144.91.77.173|10800|No|Simple||
|webserver1.priveasy.org|A|51.79.87.85|10800|No|Simple||
|autoconfig.priveasy.org|CNAME|mail.priveasy.org|172800|No|Simple||
|autodiscover.priveasy.org|CNAME|mail.priveasy.org|172800|No|Simple||
|priveasy.org|MX|10 mail.priveasy.org|10800|No|Simple||
|burn.priveasy.org|MX|10 webserver0.priveasy.org<br>20 webserver1.priveasy.org|10800|No|Simple||
|fwd.priveasy.org|MX|10 webserver0.priveasy.org<br>20 webserver1.priveasy.org|10800|No|Simple||
|noreply.priveasy.org|MX|10 webserver0.priveasy.org<br>20 webserver1.priveasy.org|10800|No|Simple||
|priveasy.org|NS|ns-464.awsdns-58.com.<br>ns-1196.awsdns-21.org.<br>ns-666.awsdns-19.net.<br>ns-1771.awsdns-29.co.uk.|172800|No|Simple||
|priveasy.org|SOA|ns-464.awsdns-58.com.<br>awsdns-hostmaster.amazon.com.<br>1 7200 900 1209600 86400|900|No|Simple||
|priveasy.org|TXT|"v=spf1 mx ip4:95.111.228.106/32 a:mail.priveasy.org -all"|10800|No|Simple||
|_dmarc.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|dkim._domainkey.priveasy.org|TXT|"v=DKIM1; p=" "MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA5ZkEOUmGaca90Sp7vR+i" "phizRphdgBIX2hjFahEyMZUx/2wmMWTi6KQ+3ZZxZ84D2J102s2KZpgqgfS/aCw6" "gVQIe1SPD1Uey0NWBXzr3EeLobHKQU5Ojj2TDfGJi8lg3N8ldAyFZXdaB9ZQlXXT" "DLMkCWEgpL9xv0HoRvzIp/PHuIPAWLIvaVPYe3PiLjrD9iGYqSFnWsIBEY4ZwDDL" "XC2WBzIfDEWNuHB6YPuE2aLKOtI9b6obzp6/bt26HzPuuc6tDSi7P4WUaEHbMRte" "l20b4K8s8E6N7CW/kGn8WAZuNvFl9l3RFTyN75OslwEncyD+UyP1YF/+BjITT+0c" "DwIDAQAB"|3600|No|Simple||
|burn.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.burn.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|fwd.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.fwd.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|noreply.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.noreply.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||

## Reverse DNS

|Server|Pointer Record|
| :------------ | :------------ |
|webserver0|webserver0.priveasy.org|
|webserver1|webserver1.priveasy.org|
|database0|database0.p5.vc|
|database1|database1.p5.vc|
|records0|mail.priveasy.org|
