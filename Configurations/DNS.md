# Priveasy DNS Configuration

Priveasy operates its own authoritative nameserver. This means that we host all of the DNS records associated with our domains and services, and can guarantee that zero logs are kept.

## Zone 1 (P5.vc)

|Record Name|Record Type|Record Value|TTL|
| :------------ | :------------ | :------------ | :------------ |
|@|A|144.91.77.173|10800|
|badapplews0|A|213.108.105.170|10800|
|database0|A|161.97.95.155|10800|
|database1|A|51.79.86.89|10800|
|docs|A|95.111.228.106|10800|
|records0|A|95.111.228.106|10800|
|relay1-1|A|209.126.12.189|10800|
|relay2-1|A|185.145.129.25|10800|
|webserver0|A|144.91.77.173|10800|
|webserver1|A|51.79.87.85|10800|
|ba|CNAME|badapplews0|10800|
|badapple|CNAME|badapplews0|10800|
|@|MX|10 @|10800|
|@|NS|dns0.p5.vc.|86400|
|@|SOA|p5.vc. admin.priveasy.org.|86400|
|@|TXT|"v=spf1 mx a ip4:95.111.228.106/32 include:mail.priveasy.org -all"<br>"keybase-site-verification=DHramCRdMolyxSdp0eFGBrcEHqTWhi4QPKDlV5vH85U"|10800|
|_dmarc.p5.vc|TXT|"v=DMARC1; p=reject; pct=100"|10800|
|dkim._domainkey.p5.vc|TXT|"v=DKIM1; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAoLgiU64/" "JQcKeUgaJMT07RQuA3zC4ZDDU26hVQHGVwHI4AbuTkZUEe3DOWoP52iw5lCK+sB" "h6tjqx7JtLjsXWJjwQ2VMLC23llG9+AAdLGlsi9vYPfvwWkW/zkndnD2FynD/R8" "j0rh0c37EFOIvQ39dNJVj0AcjkQMcKZPBj0a5Sl1NHpZHKgVK+0z+ucR7fJRPwi" "Gj9Mvk1qTwUhbOSXeoz5ak4BMTgM4vZC0/seE0LvAGF46yZyny+rrc6rGXhyeUf" "91K+CXfF1CT0eeNq3XuEM6Fse9p8b0OQquetO8RITaO6kGFr3iradNgpJkpr79f" "h4XreNoznvD0QIDAQAB"|10800|

## Zone 2 (Priveasy.org)

|Record Name|Record Type|Record Value|TTL|
| :------------ | :------------ | :------------ | :------------ |
|@|A|144.91.77.173|10800|
|badapplews0|A|213.108.105.170|10800|
|docs|A|95.111.228.106|10800|
|mail|A|95.111.228.106|10800|
|webserver0|A|144.91.77.173|10800|
|webserver1|A|51.79.87.85|10800|
|autoconfig|CNAME|mail|10800|
|autodiscover|CNAME|mail|10800|
|badapple|CNAME|badapplews0|10800|
|www|CNAME|@|10800|
|@|MX|10 mail|10800|
|burn|MX|10 webserver0|10800|
|fwd|MX|10 webserver0|10800|
|noreply|MX|10 webserver0|10800|
|@|NS|dns0.priveasy.org.|86400|
|@|SOA|priveasy.org. admin.priveasy.org.|86400|
|@|TXT|"v=spf1 mx ip4:95.111.228.106/32 a:mail.priveasy.org -all"<br>"keybase-site-verification=7vntSggoXZyNZ19HY6KmnpbjsxcyrYmo2zD7nyqFoBI"|10800|
|_dmarc|TXT|"v=DMARC1; p=reject; pct=100"|10800|
|dkim._domainkey|TXT|"v=DKIM1; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAwigNdV1j" "CPvZ5UraLd1Fj/WZn1378Yk2lriJivVqNTYlKoBesk3Quoqw3r72CGlHXxT188A" "HrLGgoFaqaFw3NB5r5acOGE7RgeNE5Hm+pQZEwbDME0cx242RA8P1yrQrMNGf/l" "Z4Xa44MTjeKAWtyyUUQEpIUjtllCdWeTqrwtz8qHR8jQivJWzqWExIQQ+VwzVQK" "piYcOwaRtEP5SeHw0VUG1gQKWw5eZ2k4YkHrn3gNXVG3+YyvGGCYJU1rWQQ1uqh" "hWDWy5TPtfKY9AogXNoir+1i8V3uq6HnHu6PiM8CB6NCDIkUVeqQax3DbEirUku" "V5IO8zWYis9vwIDAQAB"|10800|
|burn|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|
|_dmarc.burn|TXT|"v=DMARC1; p=reject; pct=100"|10800|
|burn._domainkey.burn|TXT|"v=DKIM1; h=sha256; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMII" "CgKCAQEA2EwRx5xTfkQO0igRVVSjh7/pdFJDQ7IdXIcX3pfkjmIW2q78VQwf/Fz" "xGeJ4TkZs3TBRaHOrldt5hgUtbUhurSowXfU4c3Yr5E2TlnB5SLaYN2NxOlqR2L" "XpHkE9TIEa3zpwk/QeGbDOTQubq2tj08LzJNid9+1K2PVLGGD564dFVbegb3K0I" "gXTANlJD9WyI+pBWqNvMtHT7eyxAv375knu0pV2Qyv8n50DrAKvqLtpPQ8j8Y7J" "UUanxxwpceyT68RugJ2lJs6Fh1/AedqgGRldXF4yOxY3Ne5oBDVL4RjBDKcce9q" "gUTmeDZvq/qJPVfdlJOXckmbGG7tPwIDAQAB"|10800|
|fwd|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|
|_dmarc.fwd|TXT|"v=DMARC1; p=reject; pct=100"|10800|
|fwd._domainkey.fwd|TXT|"v=DKIM1; h=sha256; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMII" "CgKCAQEAugLdZu/F+bqsGpnHyM+CLrvrcljRpJ4CdU+9s/XTGH5PoBrA5WUbs5F" "1e20D5zHJcSrvxXAu0iE9GC9HwNCy94TTY4qnszbdXamqCeUokQioNGIWEGvU5F" "/q/gZ0RjFBFBAdFunpujExdVDAouW8o9ELqQ86EmCR/9Aiwm6ikAOWTANT/wbKj" "4bhaa+g5HNEomHFJdst+4FoEDBg4odE1rd5QBCyoC6P8vsMF67nu7SkUs6CtjtV" "iNGhrjaqbU2o21sKlVlAdKMkr0t4vvaoAdXW1x1hsvZanZ5Gv0reJk7Ugi0B3Af" "itIpdeUDpPECG6mZJyReBepGoO0EBwIDAQAB"|10800|
|noreply|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|
|_dmarc.noreply|TXT|"v=DMARC1; p=reject; pct=100"|10800|
|noreply._domainkey.noreply|TXT|"v=DKIM1; h=sha256; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMII" "CgKCAQEAs95tfINY8HwGjcoX+VBlmQHroL+mn5mtDvtd9z18ipRDlW4ElsIhJQx" "muJI37sWmiASzZh2oYEwE5nQoj0mCxxXUxhotF5UMUINF/rwD/O1c5u/2JvP38A" "6uxj6XV4Mp+DE5iFA/VOVeuJ0jcpAsA09QshqDf3JYo4IzG76bFSxPAI2CDnBXF" "yLuVVO2nmvtjtcm3iOYEIhjJGia1mv2hkHOp6h3trkLkzkfrGNybzSIlE8Zqrix" "OloxDu/XywihoP4N0NEj9u6cfTsSi9fFTTtnF1UZ/gPTnI02v6o0vswL9c5Cp/J" "5OXwA2AEavnyJut1NJ0D59gVeeCb8QIDAQAB"|10800|

## PTR Records (Reverse DNS)

|Server|Pointer Record|
| :------------ | :------------ |
|badapplews0|badapplews0.p5.vc|
|database0|database0.p5.vc|
|database1|database1.p5.vc|
|dns0|dns0.p5.vc|
|records0|mail.priveasy.org|
|relay1-1|relay1-1.p5.vc|
|relay2-1|relay2-1.p5.vc|
|webserver0|webserver0.priveasy.org|
|webserver1|webserver1.priveasy.org|

## DNSSEC (DS Records)

|Zone|Key Tag|Algorithm|Digest Type|Digest|
| :------------ | :------------ | :------------ | :------------ | :------------ |
|priveasy.org.|13517|ECDSA Curve P-256 with SHA-256 (13)|SHA-256 (2)|F2ECDB794FE78598C0BB96E8432DC50BD9B7287F184FB37F704B5C9B3974D663|
|p5.vc.|8171|ECDSA Curve P-256 with SHA-256 (13)|SHA-256 (2)|F09C505E651B01A53621A3EAD40A05AA4DD9BBE8E04283566305CE3479BA4733|
