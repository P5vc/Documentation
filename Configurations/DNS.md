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
|dkim._domainkey.p5.vc|TXT|"v=DKIM1; p=" "MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAoLgiU64/jJQcKeUgaJMT" "07RQuA3zC4ZDDU26hVQHGVwHI4AbuTkZUEe3DOWoP52iw5lCK+sB0h6tjqx7JtLj" "sXWJjwQ2VMLC23llG9+AAdLGlsi9vYPfvwWkW/zkndnD2FynD/R8ej0rh0c37EFO" "IvQ39dNJVj0AcjkQMcKZPBj0a5Sl1NHpZHKgVK+0z+ucR7fJRPwilGj9Mvk1qTwU" "hbOSXeoz5ak4BMTgM4vZC0/seE0LvAGF46yZyny+rrc6rGXhyeUfW91K+CXfF1CT" "0eeNq3XuEM6Fse9p8b0OQquetO8RITaO6kGFr3iradNgpJkpr79fmh4XreNoznvD" "0QIDAQAB"|3600|No|Simple||

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
|dkim._domainkey.priveasy.org|TXT|"v=DKIM1; p=" "MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAwigNdV1jHCPvZ5UraLd1" "Fj/WZn1378Yk2lriJivVqNTYlKoBesk3Quoqw3r72CGlHXxT188AfHrLGgoFaqaF" "w3NB5r5acOGE7RgeNE5Hm+pQZEwbDME0cx242RA8P1yrQrMNGf/lmZ4Xa44MTjeK" "AWtyyUUQEpIUjtllCdWeTqrwtz8qHR8jQivJWzqWExIQQ+VwzVQKZpiYcOwaRtEP" "5SeHw0VUG1gQKWw5eZ2k4YkHrn3gNXVG3+YyvGGCYJU1rWQQ1uqhXhWDWy5TPtfK" "Y9AogXNoir+1i8V3uq6HnHu6PiM8CB6NCDIkUVeqQax3DbEirUkuPV5IO8zWYis9" "vwIDAQAB"|3600|No|Simple||
|burn.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.burn.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|burn._domainkey.burn.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; " "p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAtmiRDQJZ/KlQR4K2zEjFfuwPfiOtjilRAaHQWk8GNTpJjimvD2FGgBYWxFvBecQdQaoSOEVo5QBt/B78K+Y+XBr6bQpV5vgnZvVWL0zDqAKhL4wcDZY+tloj8YL2EyeLEJqc8QB5Lke0+uOIPb7XlhGQuHFebjVSBZiKvhCtE4tMcDQbZMkSq42hFBBDk086V827qmStLEnIaL" "6k3WCxCr7XKK8///dSB+JOHbm1DPKbhXjJrzGQPA1Ousxphjlxe2oaf3YkjB4+2ov4zsCG82HLn5r0rv5J87ULqZMf/NkDPsU6wYPFvF/VYwm6DXMvJqU2kkbXghHJXKMgKP4QTQIDAQAB"|3600|No|Simple||
|fwd.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.fwd.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|fwd._domainkey.fwd.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; " "p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA3BKefZHmhxDkr0dZuFLq4Bc7+CgV+20zdzhHtHJlsnIsOP13uXvJpyGYMnML4lyiJM6Xlb3aF/urDLR5k7LJluL1gc+T5rcGTjeiUUx4bHYGXbZ1o3rRbb48A8E1RONt7MZ9mJ9/S2FbQn1Sq8PDnaUnpzZweFUumooPxG5LDlofKwu54soJBxYhmyQdw1V5PtaFQpHa9a8SFr" "MgzbpQmZR8FVgPqaELa416rPdmw/UzPNh5tGQrdusYVOcKuQX52UEYmj1AKcuyY1KZ2HP/lF97q7rJU3I1JgXYQyZ/pffRX6QAIBQSMDrKS9mNeJr+L8mxxT2DEmO/eyprdI3UjwIDAQAB"|3600|No|Simple||
|noreply.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.noreply.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|noreply._domainkey.noreply.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; " "p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA+LmqHQxD/SaB3cxVasZlPqEJbnyqARy1/OpbFH9V6KfSX+rGVEQqV0gHDjGH22hCkd0PgzWSOjRnpDhR/AfT1EyFqf3PFtdUxuZFwr6uDg1hzcZP10wV/h5YqLr07L/avPZ/KdvL2Kdi1DYL9n+BEZQ2VouDLDl4iQxZSUKMZF1L9BXtReHMTlrFhRdGsjjTBJekWVAhnMcLE2" "KJVls4WHCWsOni6TljcnxAxLqEdRnL1rNrIrxDQwsBxqvqNGKL8L6KudyfK6Z9TKNnq4PMFStkIb50QVX9jc9IE8xu4Is3AJYlSNVkNZw7Yczc4hL7wSXS7DKX0EP3C3pg7p3CYQIDAQAB"|3600|No|Simple||

## Reverse DNS

|Server|Pointer Record|
| :------------ | :------------ |
|webserver0|webserver0.priveasy.org|
|webserver1|webserver1.priveasy.org|
|database0|database0.p5.vc|
|database1|database1.p5.vc|
|records0|mail.priveasy.org|
