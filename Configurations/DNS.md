# Priveasy's DNS Configuration

> Does something look off (outdated, incorrect, could be improved, etc.)? Please let us know! We do our best to keep these records as efficient and up-to-date as possible, but we make mistakes!

## Hosted Zone 1 (P5.vc)

|Record Name|Record Type|Record Value|TTL|Alias|Routing Policy|Differentiator|
| :------------ | :------------ | :------------ | :------------ | :------------ | :------------ | :------------ |
|p5.vc|NS|ns-1203.awsdns-22.org.<br>ns-543.awsdns-03.net.<br>ns-1779.awsdns-30.co.uk.<br>ns-80.awsdns-10.com.|172800|No|Simple||
|p5.vc|SOA|ns-1203.awsdns-22.org.<br>awsdns-hostmaster.amazon.com.<br>1 7200 900 1209600 86400|900|No|Simple||
|dkim._domainkey.p5.vc|TXT|"("<br>"v=DKIM1; p="<br>"MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAtI+xkY2rzRAkSlmnSgv3"<br>"nB8Ad/EGnfgaIhjq9Kbre4Pri5P748QxLQFKXKAcMPiPeyc/+/vi7E5P2JDRy9+C"<br>"1AQoAUjcg/yh8E6L7r4Q2UdT9pd3vb8cb1pmy6ZfNGqZjAe85F+igqdYsGCExW7q"<br>"U4I+qGoS9A6kTrqAfIA7QhthLAnn+p8pda5Ztm2G8XiwoAH2Qlz3OTkeEgTa8xK2"<br>"rm1+qEd9m6LYm4d4tuzJKC6PN3+BaTrbgKf3wWLUmaa2izgfIUp5IwoXpcbTsm+y"<br>"1kCXenizFK3CXsph60cIEdXP7QERgQvjU1EBjoo7VtaqGOC+4YOoekm4VO2HY+Ge"<br>"\"bwIDAQAB\")"|3600|No|Simple||

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
|dkim._domainkey.priveasy.org|TXT|"("<br>"v=DKIM1; p="<br>"MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA84tCGLxM37GJm2LY9NWX"<br>"CdrCSsy3Mm2AlXdVUvuNbY5wgcXdABkvaK375pAJjkxIcEU4djQ7mCsmHUKpPbcV"<br>"QD43tv9qyCx9gK06UJ3Rl3Qk19eNwSG/IrvYQ8fQi5JazKmie++GWTbDiF+aVh8h"<br>"s0vhJCv0FheXzENEVzx9A1WYWwfkL1VDYYa8M1SJs/HdIWI/I1C2MXxUcbR4kdeC"<br>"zQtEu1BqqL+Z7ny4YobxY0t3IpmRWKyLG34txUifbciA15DfKQxR/BTgg0h0lia2"<br>"pZujedK57ZEKJ/kEHeEfwH6g9hhSsTDjyNf1ke5NewNM1FgW07H2Gc0X8Wr4Q3ag"<br>"  \"CwIDAQAB\")"|3600|No|Simple||
|priveasy.org|TXT|v=spf1 mx ip4:95.111.228.106/32 a:mail.priveasy.org -all|10800|No|Simple||
|burn.priveasy.org|TXT|v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all|10800|No|Simple||
|fwd.priveasy.org|TXT|v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all|10800|No|Simple||
|noreply.priveasy.org|TXT|v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all|10800|No|Simple||

## Reverse DNS

|Server|Pointer Record|
| :------------ | :------------ |
|webserver0|webserver0.priveasy.org|
|webserver1|webserver1.priveasy.org|
|database0|database0.p5.vc|
|database1|database1.p5.vc|
|records0|mail.priveasy.org|
