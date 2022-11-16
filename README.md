# :rocket: Amazon list scraper :rocket:

Scrapes Amazon product data from a list of ASINs using chromium headless browser with python.

## Running locally

### Setup

Create a virtual environment and install the requirements:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Now you can run the application:

```bash
$ python src/scraper.py
+--------------------------------------------------------------+----+----------------+-------+-----------+-----------+-----------+
|                             list                             | #  |      item      | price | requested | purchased | fulfilled |
+--------------------------------------------------------------+----+----------------+-------+-----------+-----------+-----------+
| AWS Professional Services North East Toys for Tots Wish List | 1  | I2GOV6NR7XN6WK | 21.59 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 2  | IBX93S3LT7USQ  | 22.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 3  | I1758VCPK07C5N | 28.92 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 4  | IL8XP5F9NMEIM  | 20.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 5  | I37L0Q8R07NW7W | 3.59  |    100    |    13     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 6  | I13OPRH8MMLSTC | 34.99 |    100    |     3     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 7  | I1IICFE250N7VJ | 24.99 |    100    |     4     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 8  | I3TESHSGHW6TQJ | 16.95 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 9  | IB1RSVUP6OKL3  | 32.99 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 10 | I3T6SEHSKB0LUZ | 29.99 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 11 | IPJ1HJCG0NMKB  | 20.99 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 12 | IJZNTUV171TMU  | 21.99 |    10     |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 13 | IWFVC541PCRE8  | 24.99 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 14 | I30WNUP7OVR5SO | 29.99 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 15 | I19ZZGSCZYVELU | 20.99 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 16 | IXH1ZUTIDKTYS  | 11.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 17 | I1F4Q76AYBF8VS | 29.95 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 18 | IN1KGDFHZBBZC  | 34.99 |    100    |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 19 | I4I4G5EGPCZ26  | 11.99 |    100    |     7     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 20 | I6NDWUM5F7M95  | 14.95 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 21 | I2N5341HM6NF0Z |  n/a  |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 22 | IVRWTH5II5JPV  | 29.99 |    10     |     0     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 23 | II66QXA5U43KC  | 45.95 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 24 | I7MZSQ664VNEF  | 18.6  |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 25 | IHVP6TPSU5IZ1  | 19.89 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 26 | I1MYCIRN4GWV6O | 9.99  |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 27 | IZNVE2N4FY11Y  | 21.99 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 28 | IKGEPCL0TUX78  | 22.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 29 | I1F2S7Q5654ITY | 34.99 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 30 | I3EWE5TAI3MAE5 | 19.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 31 | IGJNA1NTQ37M9  | 22.99 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 32 | I1ZCLZVK0VYUW0 | 34.99 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 33 | I17VYMBFB8CCMJ | 7.99  |    100    |     3     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 34 | I3VH7NT8IWFF3P | 22.55 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 35 | I3SBOEYUIZLKOF | 26.85 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 36 | I2O53X1BHNKICM | 8.37  |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 37 | I1XU6D1683MM53 | 12.89 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 38 | I2PFZP083U9S0S | 17.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 39 | I2SF9VK35USH9M | 11.99 |    100    |     2     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 40 | ISFH0E4IDJVQG  | 22.85 |    100    |     1     |    NO     |
| AWS Professional Services North East Toys for Tots Wish List | 41 | I2JGHJC35CUSC  | 13.13 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 1  | ISKSTF46G7MVQ  | 34.99 |    100    |     5     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 2  | I1O8BKFDRW2MCI | 29.95 |    100    |     4     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 3  | INOJ3FHO7D0AA  | 11.99 |    100    |     2     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 4  | I21U0Q1Q3AOO3X | 20.99 |    100    |     4     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 5  | IAGDP7ZWA2Q8X  | 29.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 6  | I3N07YST3YFVB8 | 24.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 7  | I3JZEDNTI3T5L  | 21.99 |    100    |     4     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 8  | I3NU5OY4DQQ6NG | 20.99 |    100    |     5     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 9  | I1JOF798FBM21E | 29.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 10 | I10VPDID6XLC6W | 32.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 11 | I2QXS327CELRLC | 16.95 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 12 | I1MR1WGAV44JGH | 16.95 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 13 | I1VVHMHJ1KM2RK | 24.99 |    100    |     2     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 14 | IGNOAFKSR05T5  | 34.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 15 | IK2QEUBRQMBAJ  | 11.69 |    100    |    13     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 16 | I2MRO5G51YDGHC | 3.59  |    100    |     8     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 17 | I318E30KRZXLP0 | 20.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 18 | I1QKFQFQ6OOFV7 | 28.92 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 19 | I3OTV3N1OCS87R | 22.99 |    100    |     2     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 20 | I2MKF418MJAW1D | 21.59 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 21 | I3DORAV5ZPKO3L | 11.99 |    10     |     4     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 22 | IVZ33U1KN89RC  | 14.95 |    10     |     2     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 23 | I1WXG6AHNPBV4O |  n/a  |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 24 | I3VKEFOBDQFG4L | 22.55 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 25 | I1LDTWZVI2M4AN | 13.13 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 26 | I1MTSW6ISRWO2Z | 29.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 27 | IGRRJCOAT280Q  | 45.95 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 28 | IAZSPXB976E80  | 18.6  |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 29 | I1KBWH6PPW99ZK | 19.89 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 30 | I3I2IYAYOHOQHZ | 9.99  |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 31 | I3999W1Y37CFVT | 21.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 32 | I2ONXWJ9DNGZTN | 22.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 33 | I12OC2LQ8KFIKG | 34.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 34 | I1CMFPFSMA8QVB | 19.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 35 | I3UPFV3FWLQ3Q7 | 22.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 36 | I6AF2UFG5LQ5V  | 34.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 37 | I2ULAYMNIH426I | 7.99  |    100    |     5     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 38 | IPV28N6IENZCK  | 26.85 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 39 | IWLYJHNP68B57  | 8.37  |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 40 | I2GYEMSVORL865 | 12.89 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 41 | I1YG129MZWSB8G | 17.99 |    100    |     1     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 42 | I3C728NHI5OVF  | 11.99 |    100    |     0     |    NO     |
| AWS Professional Services North West Toys for Tots Wish List | 43 | I2W1MJ3GPGI7TN | 22.85 |    100    |     0     |    NO     |
+--------------------------------------------------------------+----+----------------+-------+-----------+-----------+-----------+
total scraped: 84
```
