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
|dkim._domainkey.p5.vc|TXT|"v=DKIM1; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAoLgiU64/" "JQcKeUgaJMT07RQuA3zC4ZDDU26hVQHGVwHI4AbuTkZUEe3DOWoP52iw5lCK+sB" "h6tjqx7JtLjsXWJjwQ2VMLC23llG9+AAdLGlsi9vYPfvwWkW/zkndnD2FynD/R8" "j0rh0c37EFOIvQ39dNJVj0AcjkQMcKZPBj0a5Sl1NHpZHKgVK+0z+ucR7fJRPwi" "Gj9Mvk1qTwUhbOSXeoz5ak4BMTgM4vZC0/seE0LvAGF46yZyny+rrc6rGXhyeUf" "91K+CXfF1CT0eeNq3XuEM6Fse9p8b0OQquetO8RITaO6kGFr3iradNgpJkpr79f" "h4XreNoznvD0QIDAQAB"|3600|No|Simple||

## Hosted Zone 2 (Priveasy.org)

|Record Name|Record Type|Record Value|TTL|Alias|Routing Policy|Differentiator|
| :------------ | :------------ | :------------ | :------------ | :------------ | :------------ | :------------ |
|priveasy.org|A|webserver0.priveasy.org||Yes|Weighted|200|
|priveasy.org|A|webserver1.priveasy.org||Yes|Weighted|50|
|docs.priveasy.org|A|95.111.228.106|10800|No|Simple||
|mail.priveasy.org|A|95.111.228.106|10800|No|Simple||
|webserver0.priveasy.org|A|144.91.77.173|10800|No|Simple||
|webserver1.priveasy.org|A|51.79.87.85|10800|No|Simple||
|www.priveasy.org|A|priveasy.org||Yes|Simple||
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
|dkim._domainkey.priveasy.org|TXT|"v=DKIM1; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAwigNdV1j" "CPvZ5UraLd1Fj/WZn1378Yk2lriJivVqNTYlKoBesk3Quoqw3r72CGlHXxT188A" "HrLGgoFaqaFw3NB5r5acOGE7RgeNE5Hm+pQZEwbDME0cx242RA8P1yrQrMNGf/l" "Z4Xa44MTjeKAWtyyUUQEpIUjtllCdWeTqrwtz8qHR8jQivJWzqWExIQQ+VwzVQK" "piYcOwaRtEP5SeHw0VUG1gQKWw5eZ2k4YkHrn3gNXVG3+YyvGGCYJU1rWQQ1uqh" "hWDWy5TPtfKY9AogXNoir+1i8V3uq6HnHu6PiM8CB6NCDIkUVeqQax3DbEirUku" "V5IO8zWYis9vwIDAQAB"|3600|No|Simple||
|burn.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.burn.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|burn._domainkey.burn.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMII" "CgKCAQEA2EwRx5xTfkQO0igRVVSjh7/pdFJDQ7IdXIcX3pfkjmIW2q78VQwf/Fz" "xGeJ4TkZs3TBRaHOrldt5hgUtbUhurSowXfU4c3Yr5E2TlnB5SLaYN2NxOlqR2L" "XpHkE9TIEa3zpwk/QeGbDOTQubq2tj08LzJNid9+1K2PVLGGD564dFVbegb3K0I" "gXTANlJD9WyI+pBWqNvMtHT7eyxAv375knu0pV2Qyv8n50DrAKvqLtpPQ8j8Y7J" "UUanxxwpceyT68RugJ2lJs6Fh1/AedqgGRldXF4yOxY3Ne5oBDVL4RjBDKcce9q" "gUTmeDZvq/qJPVfdlJOXckmbGG7tPwIDAQAB"|3600|No|Simple||
|fwd.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.fwd.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|fwd._domainkey.fwd.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMII" "CgKCAQEAugLdZu/F+bqsGpnHyM+CLrvrcljRpJ4CdU+9s/XTGH5PoBrA5WUbs5F" "1e20D5zHJcSrvxXAu0iE9GC9HwNCy94TTY4qnszbdXamqCeUokQioNGIWEGvU5F" "/q/gZ0RjFBFBAdFunpujExdVDAouW8o9ELqQ86EmCR/9Aiwm6ikAOWTANT/wbKj" "4bhaa+g5HNEomHFJdst+4FoEDBg4odE1rd5QBCyoC6P8vsMF67nu7SkUs6CtjtV" "iNGhrjaqbU2o21sKlVlAdKMkr0t4vvaoAdXW1x1hsvZanZ5Gv0reJk7Ugi0B3Af" "itIpdeUDpPECG6mZJyReBepGoO0EBwIDAQAB"|3600|No|Simple||
|noreply.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.noreply.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|noreply._domainkey.noreply.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMII" "CgKCAQEAs95tfINY8HwGjcoX+VBlmQHroL+mn5mtDvtd9z18ipRDlW4ElsIhJQx" "muJI37sWmiASzZh2oYEwE5nQoj0mCxxXUxhotF5UMUINF/rwD/O1c5u/2JvP38A" "6uxj6XV4Mp+DE5iFA/VOVeuJ0jcpAsA09QshqDf3JYo4IzG76bFSxPAI2CDnBXF" "yLuVVO2nmvtjtcm3iOYEIhjJGia1mv2hkHOp6h3trkLkzkfrGNybzSIlE8Zqrix" "OloxDu/XywihoP4N0NEj9u6cfTsSi9fFTTtnF1UZ/gPTnI02v6o0vswL9c5Cp/J" "5OXwA2AEavnyJut1NJ0D59gVeeCb8QIDAQAB"|3600|No|Simple||

## Reverse DNS

|Server|Pointer Record|
| :------------ | :------------ |
|webserver0|webserver0.priveasy.org|
|webserver1|webserver1.priveasy.org|
|database0|database0.p5.vc|
|database1|database1.p5.vc|
|records0|mail.priveasy.org|
