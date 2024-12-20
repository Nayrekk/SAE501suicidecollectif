# Fichier Client OpenVPN
***
***Configuration d’un fichier client pour un VPN utilisant OpenVPN***
```
persist-tun
persist-key
data-ciphers AES-256-GCM:AES-128-GCM:CHACHA20-POLY1305:AES-256-CBC
data-ciphers-fallback AES-256-CBC
auth SHA256
tls-client
client
remote 217.5.160.1 4443 udp4
nobind
verify-x509-name "VPNSERVER" name
auth-user-pass
remote-cert-tls server
explicit-exit-notify

<ca>
-----BEGIN CERTIFICATE-----
MIIFhTCCA22gAwIBAgIQHlJspl6z8r9CdvnAFs0mQTANBgkqhkiG9w0BAQ0FADBJ
MRMwEQYKCZImiZPyLGQBGRYDb3JnMRcwFQYKCZImiZPyLGQBGRYHd3NsMjAyNDEZ
MBcGA1UEAxMQV1NGUi1JTlQtUk9PVC1DQTAeFw0yNDEyMTExMzU0MzFaFw0yOTEy
MTExNDA0MzBaMEkxEzARBgoJkiaJk/IsZAEZFgNvcmcxFzAVBgoJkiaJk/IsZAEZ
Fgd3c2wyMDI0MRkwFwYDVQQDExBXU0ZSLUlOVC1ST09ULUNBMIICIjANBgkqhkiG
9w0BAQEFAAOCAg8AMIICCgKCAgEAqv0AMR0/GNP1O8y+pfrJKxORb5iZlMmJnRs7
9NaHD+vepgS8tAEONFkvHzZrhtaD9vnIqfpMbWI3xJV9w40eN8E7onIbRlJ0loXZ
UuV7g+KJ6aA0CFqeilUTC11IYECKDMKoovdRPK9Pz/RG9RXkeL4+LD0aBQBJHe+H
rwJ/xgRNPSn5p8J1Qiyr6SE8/RmTfMulD9K2on5yvieLNzF/3LJzTjiNFWgdIJCv
NItegF34RcGRsdoZrdVejX66+dHnazz/titgTm286qls1l4XhXFCU0rApmfk1zop
V6cN/JubLeZVTGjztWWbUxqJ21o/7xg3T9aqgHOID1FLj0S6jzpL9Uf/kssC7ghv
fflK3/cwhQsXXyuhsOrRu+3bO3mze4O9gyGCqnbA3c5b+YP41tHKG1KytU4pefkc
d4uJfJgElxQqprPa6Z2kQVxpSzGad/WbijQCZp+6emXx1aeAUm8XUuSvlIKIpbZh
Ube12HCZ+rTRYo7KVrJuSp4sgn6jA5MVxfbmwz4V548o27iqpTe3szBTaKPC7HUT
v1UTmvJgEy69BbEZ0xoQCYLXpTuanywJ3EUMl2OoRfm/L/OTZLXYaBXpIZV+Y17t
UNW26H9m8ksBNU6J9uc2EKnXqoypAcNRCfUwlshyzzgKfi9kuF+sg/WdkY2GnahS
ZxWmJhkCAwEAAaNpMGcwEwYJKwYBBAGCNxQCBAYeBABDAEEwDgYDVR0PAQH/BAQD
AgGGMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFLocut49AOKX6SO52ojCCHKv
YvBZMBAGCSsGAQQBgjcVAQQDAgEAMA0GCSqGSIb3DQEBDQUAA4ICAQCOHs0CWgHH
3T2ZSxPu1m03etVSsu29rgdHNlG1Fwdmva6gU06xOp/LKK/vsp1xwnntJKO5ZvpF
LqzTcGGv4KxH21U+e+EvVqdGJOU//Q7zUuXHCHLe0f9vzdEEogLe5xzuJKK8wIsF
vpjSNBCTPvixIE9K9Ui8u7kdoOxIuJXJ8xBU1g9a3zCU4UrTaKKNT+FOU2+OmKMV
jMghrYhCigLuY4XMqxHFCByPPGKl8omGZOSncm/WToW7X+07D7jARSvr4hTEQ9We
2Fu9ux7KD6LtPNutRLayejgAPzMbS+pz+14nFBjZIv1nPfBIqLDtssUu4r6/Q7zo
sbr6kXyWhSeG/5at665aNy+eNXKcw3fhUDB7eGpcpga3QBbwdLudNIlQhhzRnMAF
A/FiSInICvtv1wcZ7rVjIH9Oq+eRcCmKLba8GOHBzi5TLp6LfElRRHHzLTgeUBRA
fkug6I43wGLCcnrvNyP1278DjQgHP384wZ1un+hl30Nn4xk/o0f2g5HS8+JDD11L
GHgBs1a2DD0BEsbdoKUdf6HaZKvXjVs3yNoA60aVhsFfqwixTHYwzBwZ9Zqo/BhO
AvN9YSq5eln7OvcTze4RX1SUqNx3u17Onc/gxmnItXfD5XmzxCUqXCTqZW1aBpTU
I8eMP68OGglqcBkKLNkm4kFh6PBPe4pyCA==
-----END CERTIFICATE-----
</ca>
<cert>
-----BEGIN CERTIFICATE-----
MIIHKjCCBRKgAwIBAgITTgAAAArhW6cEtA8R3wAAAAAACjANBgkqhkiG9w0BAQ0F
ADBJMRMwEQYKCZImiZPyLGQBGRYDb3JnMRcwFQYKCZImiZPyLGQBGRYHd3NsMjAy
NDEZMBcGA1UEAxMQV1NGUi1JTlQtUk9PVC1DQTAeFw0yNDEyMTUwMzMxMDJaFw0y
NTEyMTUwMzMxMDJaMFcxEzARBgoJkiaJk/IsZAEZFgNvcmcxFzAVBgoJkiaJk/Is
ZAEZFgd3c2wyMDI0MQ4wDAYDVQQDEwVVc2VyczEXMBUGA1UEAxMOQWRtaW5pc3Ry
YXRldXIwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDPSTTEBpWpjWki
R83mLSFN2diCBnL/8wb1uKjuQSkTVByWL5cJHMCOJucg4QRuG7OewEY1ClHyRhcP
VJFXUmIJ+9QH/kEnT1bsWB2SB17xiI00UwONIGz9IV2q0gS3IYzR329BC1Yr6lVS
2Zk2+lfGJDx0xsfkYypt9Io2BZOL5OYmLwZ85TlsGV3flnTXZLQfcO98V1y4eNLU
HNVPw5ICzwf5KHGVIx+ZHhEvx15QI1VKPsQ/La8s2UuM3yQI67wSc0Bt8/ovgJQJ
SkZLSQHh/eD47advccpJEZGp98C9zsAksRS6SxcSqWPwXkR0hxwH6+nBqA938l8e
vgdu2+8JAgMBAAGjggL7MIIC9zAOBgNVHQ8BAf8EBAMCBaAwHQYDVR0OBBYEFEMw
crl9J8IGZFcY2ATUHrTCd05lMCkGA1UdJQQiMCAGCisGAQQBgjcKAwQGCCsGAQUF
BwMEBggrBgEFBQcDAjA1BgNVHREELjAsoCoGCisGAQQBgjcUAgOgHAwaQWRtaW5p
c3RyYXRldXJAd3NsMjAyNC5vcmcwHwYDVR0jBBgwFoAUuhy63j0A4pfpI7naiMII
cq9i8Fkwgc4GA1UdHwSBxjCBwzCBwKCBvaCBuoaBt2xkYXA6Ly8vQ049V1NGUi1J
TlQtUk9PVC1DQSxDTj1IUURDU1JWLENOPUNEUCxDTj1QdWJsaWMlMjBLZXklMjBT
ZXJ2aWNlcyxDTj1TZXJ2aWNlcyxDTj1Db25maWd1cmF0aW9uLERDPXdzbDIwMjQs
REM9b3JnP2NlcnRpZmljYXRlUmV2b2NhdGlvbkxpc3Q/YmFzZT9vYmplY3RDbGFz
cz1jUkxEaXN0cmlidXRpb25Qb2ludDCBwgYIKwYBBQUHAQEEgbUwgbIwga8GCCsG
AQUFBzAChoGibGRhcDovLy9DTj1XU0ZSLUlOVC1ST09ULUNBLENOPUFJQSxDTj1Q
dWJsaWMlMjBLZXklMjBTZXJ2aWNlcyxDTj1TZXJ2aWNlcyxDTj1Db25maWd1cmF0
aW9uLERDPXdzbDIwMjQsREM9b3JnP2NBQ2VydGlmaWNhdGU/YmFzZT9vYmplY3RD
bGFzcz1jZXJ0aWZpY2F0aW9uQXV0aG9yaXR5MBcGCSsGAQQBgjcUAgQKHggAVQBz
AGUAcjBOBgkrBgEEAYI3GQIEQTA/oD0GCisGAQQBgjcZAgGgLwQtUy0xLTUtMjEt
NDAzMzE4NzkxMS0zNDg1Nzc5OTc1LTM3NTQ5MTU5MjItNTAwMEQGCSqGSIb3DQEJ
DwQ3MDUwDgYIKoZIhvcNAwICAgCAMA4GCCqGSIb3DQMEAgIAgDAHBgUrDgMCBzAK
BggqhkiG9w0DBzANBgkqhkiG9w0BAQ0FAAOCAgEAEk9FpG6d9fWHrYHxrlNEG08N
Xwv6OOKlK/zutf44hHe/AioVO4rzr7Ho4AlaaX6nonMh64GuXJp7RuyV4UchgRM2
+HByhDHv3xY684PWsRPy8Vf5fVior/AVL46yiDeJjbFIpZA++s6xyuo6lbRm4l7i
zq0ydP4lPImHypHAe1+OkY4a5r5bk0qjRtVViSGxHl1M1wPO83SGtCK0OogEA2KJ
VusOPsEA6xPmqjElxR/MRuMUJSG/Oi+g/FWPq6MTVEPIHwwlPr62y9i73iu+mbZD
31Q5CXSPurM81YqdumR30SAfbOF1AL6B7xveS86Oago2UDrDmsV68iQCduREl2PI
BDnwmySZMPK2QGf+NXr3jbllYN5tCn+moh7LB8o4DWh2wFmmeUJ05Mx1/V1u8Qoo
dmCbwzBLX4t1ojGgq1X3peFgQp2ezBFFd5b8E+1w1LB7Gw3PvT1EVqjjedMW1YUl
f0ngdZNV4K3ROddQiwOBF/7NQ8U1Qo6sqgvL56epOCOU87zl6DqnKCs2wNx4M1SB
v85s+qZfEl4ENiX3j2J+0geBDIAV6NhkbaBq/NDgrcmiiySFsBtRtB0oDzFN1fwp
UIZlLK8Aec5yfmXb+qS0vu2yw6cukjrQ09svpdHdyczAJZC6Sd0w8Zw4RH/CQGK9
e2iuhfQmVi/69eWhnQE=
-----END CERTIFICATE-----
</cert>
<key>
-----BEGIN PRIVATE KEY-----
MIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQDPSTTEBpWpjWki
R83mLSFN2diCBnL/8wb1uKjuQSkTVByWL5cJHMCOJucg4QRuG7OewEY1ClHyRhcP
VJFXUmIJ+9QH/kEnT1bsWB2SB17xiI00UwONIGz9IV2q0gS3IYzR329BC1Yr6lVS
2Zk2+lfGJDx0xsfkYypt9Io2BZOL5OYmLwZ85TlsGV3flnTXZLQfcO98V1y4eNLU
HNVPw5ICzwf5KHGVIx+ZHhEvx15QI1VKPsQ/La8s2UuM3yQI67wSc0Bt8/ovgJQJ
SkZLSQHh/eD47advccpJEZGp98C9zsAksRS6SxcSqWPwXkR0hxwH6+nBqA938l8e
vgdu2+8JAgMBAAECggEAIPiziHTFrJUeQoIqabEHCaObsT8GXtkQ49gOIuvBdV4d
N/R08VGd/V6JyCySsFL+tMM/x6MPGtr0Qw+AGOQ1TQI+HVFfmrmfiXOQrJA4lXHT
iB2mRHYCcBc1F31Vm62eASopv65mdBDPpqCPIvQaLx3HcgnGdPkjIB9UNriXWhpy
viw76HDfTDuixe2RVGuVcvkfu94FTNt3fbGzENsAyZPeI9RwSS+vboKpERxZSm88
hTouLddbUoNWWb374vDTWvVIgXSkYJ8EvuQiOo5K672Ut4x7cf2niB1HehI2c2Zs
Hk1WEYCO1H6tskBZY4ZHTJHYWn3noh7X6NXrDWA0KwKBgQD8Hfp3Zzr2jX30Q+Hn
imK+juqnO4zyOFk4vMOskRKyPyzDC0c/AaZb+iHEUywxQ/nNuDPogjeGPViaD7AP
GQKIAI5deSfbRrqtQwgV4pJshGWBUum2UOTHm+KRGEapqzymQh/iAoBMEeD8gWEC
iiY+dARpa8OeVzwXy2cgaJBFjwKBgQDSenjZ9/GO4oNrb6pOHVTRzrCs/QFyAXxo
l2+JdqAJUEVjJ5mom9y4RUlyIie4nQB7lljqsXF1kg6wNcZQ8gFiouQA3IfnbWYI
OVmzMqMStNkbu0C1qo0FrZ41cfVyCwwEO2e5P4GadruBsxYRxgqZaOaIfhx6p823
0bd9bqil5wKBgQD1W6d5tLkpYSIHKlkboQ3gLe4nuki9IiGSmgJEWxs65UiGuN8p
bk2cjZ13FwqXF3RwxKefy7qFpgYoSMQqrUhNW10xkss7F2ZtYCLqSYn+mgq/BRX2
HFvJ9udUFbAPR1rK4udsaMq7PVsb4j2q3w/BD9+LSRkja/pLneRLIffl+QKBgQCn
q8j6WvqjyO7Id3xEHjmjqfQ02ph8KZLh/0FrUITM5pVgF/vgxclfQlLwCSV7fBcW
XP8Yd6La9i+dUDlb4m4YFYts5EGfqxbNFmLOzlf6XvdVkCZMkkEldNnD2bSd1Q8N
kAVhHaYxVsSo3fGG1y06aMa9lTk6vNK0zOxPkAfpoQKBgFJbdq8U2n0X9/0+L0Y6
WMGpbEdqzszOVtNRqxzWwQXU67pZuViErv+5tEK204CWtFcbQFyws7WhJmMphXKd
te6kEeH+Im8QdlRQrAD043IkVs6Ir5YL9mnkqfJRYweNQ5qO8r34sJ6mRhzXUn9X
FMFCTPvIDghKw0na9FRim67g
-----END PRIVATE KEY-----
</key>
key-direction 1
<tls-auth>
#
# 2048 bit OpenVPN static key
#
-----BEGIN OpenVPN Static key V1-----
2126ae0575d7a1f0ff134f5dfd5aa52b
fd14d72df08f350afe02aeb4f8af1d13
ef7ef4f95618e4369f6379596124b5c7
fcdf650fd214e776ff18719e98407e3d
ff735d1c5e26863bc9784d0350fb7909
2f5a2980ff672a2a4e7ac187f6024d3d
9873ed8af0deb0b9afb4b93369e780d6
ba2f58986714849650b8a467ab5bc2a4
fd610c65fb9b4b913becac198f568c71
32fb85e207f9295b16e32158e7697f6b
381cc3601144774ad31d4bffd729c883
c8c0e20dafa9d6ddd7609a98c919e672
4fb66b2ff9efb495ca30d8f3dd011b8f
d2d3d96e412c86835f0b7b0b0612bfa4
a8f06c3484bb19a0a181b6ac06a6382c
d5d97374a7b3362ecaadffe6774969fa
-----END OpenVPN Static key V1-----
</tls-auth>
```
# Configuration d'un serveur VPN
***
![[Jalon28.1.png]]
***
![[Jalon28.2.png]]
***
![[Jalon28.3.png]]
***
![[Jalon28.4.png]]
***
![[Jalon28.5.png]]
***
![[Jalon28.6.png]]
***
![[Jalon28.7.png]]