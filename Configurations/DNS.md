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
|burn._domainkey.burn.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; p=" "MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAtF/2vp1JjuJUQHnjKAa" "TZ0MLytVbp7/K/xvKGh5GRf8ZWYXe9Yyg34s4RNiL6AABBp4+9FoJTkqZibGzPK" "oYbprbdSoZJj8xD6FoD6Yyl2l5Edd3ozB3lx+KPjlsYCOj/+EZW0mksD6k7kz4+" "eQD2scaZ3grYSwj2ah9KmRzSwYaTtLys2paw8Qd3WPbwQSB/kPYRJsLSiaVhMNT" "sMP+u8JQMS4C22tMFGsoVYPbaxJokcW4cKa2pJ7LeijRz6h2RlClj4YC2KY0+eb" "mVL9PGVq2PlmNtYA6CBRkxaZ/yUYUR0GaRZSEXxlO7yRmK547jRObIkvVZZW03q" "fP0SufbhfuOqcpjY0YhFTvivly/2DtJlhFaKqVm5sbqLkpn537jYmVwr4A+Km6e" "1KI3hHvQmggBNJqPyHn/2X2mmTajbIe/bgkP/At/zhMnmwUrYLcVk1XyMC6qitw" "aF3O5cDHg1Q7iTX25LdadX8sh7bjG67JuIBb9QmYgdbO08hvLMSelM7MzzQsCSl" "BH8pckiqHWzLvqD7zGBNrRBvlPuMo8jOpgA6L5mCyycGSldvC83O7QTMgz9UJD2" "7iZ86UrYDqXlIOVvrsBkHnMF8ORCv4nuCTZ1X0ALoevbHN2UbqdHMK2ywOGBsy6" "AG4DimUDUfCI4GvwhsJhvmMCAwEAAQ=="|3600|No|Simple||
|fwd.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.fwd.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|fwd._domainkey.fwd.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; p=" "MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAmt083QIhR7IE2tgDfla" "rjVNg3dPwP2XTxTQafsW/aIcWa0uCfm+bsz3ezlXPqil5s27rG5Cza7vxBi7P3S" "iS4EBpWfbPM/KxE+3s5X/xxCKqqZifAcvyeeFZC3DjL5pfoxvrHqztIYL1QaLuX" "SnLF60T1uN3dl2kVYBtgJqwmQSpTOu2jqPAO56DoOtyon0zi7e+T/Qlxeod+1Sh" "+uO5fnenN/1bzj1LBUZhfTzf3VhaSRAbmSBWujoFZEKrvBCja35B96notSLgHnP" "yFol738bjf0scy1vbmCjAHuVmMJDkWre0WSYWIpp7BCfpHzT0j4S7K2mQf4tezr" "lfEx+/vi6vEKVoCqWwpARYNDihIv6IENz5it2wGpVqPdGf2+fjvut4YSlM03Axx" "rg06IrD500HcPdM02O3dKk0wfLLNoUfMma1oOZ4LDI5Pjvws6sUZhAbNECu66Ba" "PpBttvQa+eODbT8+BzJfHMNhaZ/T2FZN2HRghgDPcvI+6yVTW/eJSK+xc7G+pqZ" "lPbAz4fvy4J7LQKpovFJ8MSdHM+7wTv0xhFe7NHBow/FjXf9w9qUOdSyauWwhT3" "4s1ziEcpqGnrX6p8bbRGsZWePpfPYEawfa1Zk+bDvvZQlwTym7pKwvkaNB7NmSz" "w8RZb6tuurLIyR2rvDoSQ10CAwEAAQ=="|3600|No|Simple||
|noreply.priveasy.org|TXT|"v=spf1 mx ip4:144.91.77.173/32 ip4:51.79.87.85/32 a:webserver0.priveasy.org a:webserver1.priveasy.org -all"|10800|No|Simple||
|_dmarc.noreply.priveasy.org|TXT|"v=DMARC1; p=reject; pct=100"|10800|No|Simple||
|noreply._domainkey.noreply.priveasy.org|TXT|"v=DKIM1; h=sha256; k=rsa; p=" "MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAu/yluGOKbtL6oxZ1rVz" "7BbFeJR1Q6N2ZmqL3WS28ps6Gqj1MGPQZ+2vMMVVGjZRm5M1AiMTnUtSASdUCX9" "2B+QyPsNsz3Y8V7/nvXJkrVlU7HYBS4GQg9k3Mbmr/37rnJDLuAK4yHmDAzfmAP" "y5It9m3T1+fMG/kE7CFc4+DxxLLRZJA3E33Af/ah8hQpW/v1l4saj2dciamdxbW" "wD8Cf+gHuWpFfmM9lquuTLcT11LedWzJcWG/mVWfen5Cb/AtLCyRQ2FUU70Xccy" "7z3mJ+SAQI2bvzZW2XM0L9TA1b5PrJFFJEiY0oosUyF1+8mJkGmT50xC/7a2+25" "v20DBzImorz5qJ0Rsw8aMBGI+Uo4hxByCxZPFPRLz/Mq2CQjLaRDi942uTQYNWC" "QoNjmmGBSN1pnwbFhAx9e8bo4LWnhpgWfhvkiWAXX54rbQ589pWJkQkCWnFBUYw" "lgtcjrf1frOXOAmlC4zVWWNJ9smEDB6q/AQuH+luUY6MMOn2XteoGT+WNObzJsx" "oCoM2KfzDzdIw20IOlGhb1RlHaabPs5K5c6rTIiOIR1mLa8ypX8EhtMl8Rg9hGE" "HEOB+3/6FzISnSEltfPvVBUzkPNzy9QJx6MwI/pD9dbkjSOq5wS/oNsedB4y0eX" "hC/k0mstm7yK+kHcp8msqb8CAwEAAQ=="|3600|No|Simple||

## Reverse DNS

|Server|Pointer Record|
| :------------ | :------------ |
|webserver0|webserver0.priveasy.org|
|webserver1|webserver1.priveasy.org|
|database0|database0.p5.vc|
|database1|database1.p5.vc|
|records0|mail.priveasy.org|
