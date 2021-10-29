# Magento EOL

EOQ: End of Quality Fixes.  
EOL: End of Security Fixes/End of Software Support

| Magento Minor Version | Release | <attr title="End of Quality Fixes">EOQ</attr> | <attr title="End of Security Fixes/End of Software Support">EOL</attr> |
|:---|---|---|---|
|2.0|November 2015|**March 2018**|**March 2018**|
|2.1|June 2016|**June 2019**|**July 1, 2019**|
|2.2|September 2017|**December 2019**|**December 2019**|
|2.3|November 2018|July 2021|April 28, 2022|
|2.4|July 2020|||

Notes:
1. Information taken regularly from the [Magento Software Lifecycle Policy document](https://magento.com/sites/default/files/magento-software-lifecycle-policy.pdf)

# Supported Software

## PHP

| Magento Minor Version | PHP 5.5 | PHP 5.6 | PHP 7.0 | PHP 7.1 | PHP 7.2 | PHP 7.3 | PHP 7.4 | PHP 8.0 | PHP 8.1
|:---|---|---|---|---|---|---|---|---|---|
|2.0|✓|✓|✓|✗|✗|✗|✗|✗|✗|
|2.1|✗|✓|✓<sup>[1]</sup>|2.1.16+|✗|✗|✗|✗|✗|
|2.2|✗|✗|✓<sup>[2]</sup>|✓|2.2.10+|✗|✗|✗|✗|✗|
|2.3|✗|✗|✗|✓<sup>[3]</sup>|Until 2.3.6-p1|2.3.3 - 2.3.6<sup>[4]</sup>|2.3.7+|✗|✗|
|2.4|✗|✗|✗|✗|✗|Until 2.4.1<sup>[4]</sup>|Until 2.4.5|✗|2.4.5+|

Notes:
1. Only 7.0.2 and ~7.0.6 for 2.1.0-2.1.1.  Starting with 2.1.2 that was expanded to include 7.0.4.
2. 7.0.2, 7.0.4, and ~7.0.6 for 2.2.0-2.2.4.  Starting with 2.2.5 7.0 support was limited to ~7.0.13
3. Supports ~7.1.3
4. The composer.json in 2.3.7, 2.4.1, and 2.4.2 appears to support 7.3, however the [System Requirements](https://devdocs.magento.com/guides/v2.3/install-gde/system-requirements.html) does not list it as a supported version. This likely means it can work, but you'll be on your own.

## Composer
| Magento Minor Version | 1 | 2
|:---|---|---|
|2.0|✓|✗|
|2.1|✓|✗|
|2.2|✓|✗|
|2.3|Until 2.3.7<sup>[1]</sup>|2.3.7+|
|2.4|Until 2.4.2<sup>[1]</sup>|2.4.2+|

Notes:
1. Composer 1 still works with Magento 2.3.7 and 2.4.2, but is no longer supported.

## Elasticsearch

| Magento Minor Version | ES 1.x | ES 2.x | ES 5.x | ES 6.x | ES 7.4.x | ES 7.6.x | ES 7.9.x | ES 7.10.x |
|:---|---|---|---|---|---|---|---|---|
|2.1|✓<sup>1</sup>|✓<sup>2</sup>|2.1.1<sup>3</sup>|✗|✗|✗|✗|✗
|2.2|Until 2.2.8<sup>4</sup>|✓|2.2.8+|2.2.8+|✗|✗|✗|✗
|2.3|✗|Until 2.3.5|Until 2.3.5|✓|2.3.5+|✗|2.3.7+|✗|
|2.4|✗|✗|✗|✗|2.4.2+<sup>6</sup>|2.4.0-2.4.1<sup>5</sup>|2.4.2+|2.4.4+

Notes:
1. Versions 2.1.1-2.1.2 declare support for all 1.x, but all other 2.1.x versions only declare support for 1.7
2. Version 2.1.0 only declares support for 2.0 and 2.1.  All other lines claim support for 2.x
3. Version 2.1.1 is the only version in the 2.1.x line to declare support for ES 5, and then only for 5.0
4. 2.2.0-2.2.7 declare support for ES 1.7
5. 2.4.0 specifically declares support for ES 7.6.x
6. 2.4.2 states "Magento 2.4.x remains compatible with Elasticsearch 7.4.x" despite compatibility not being declared at any point

## RabbitMQ

| Magento Minor Version | 3.5 | 3.7 | 3.8 |
|:---|---|---|---|
|2.0|✓|✗|✗|
|2.1|✓|✗|✗|
|2.2|✓|✓|✗|
|2.3|✗|Until 2.3.5|✓|
|2.4|✗|✗|✓|

## Redis

| Magento Minor Version | 2.4 | 3.0 | 3.2 | 4.x | 5.x | 6.0 |
|:---|---|---|---|---|---|---|
|2.0|✗|✓|✗|✗|✗|✗|
|2.1|✓|✓|✓|2.1.17+|2.1.17+|✗|
|2.2|✓|✓|✓|✗|✗|✗|
|2.3|Until 2.3.6|Until 2.3.6|Until 2.3.6|2.3.1 - 2.3.5|2.3.1 - 2.3.6|2.3.7+|
|2.4|✗|✗|✗|✗|2.4.0 - 2.4.1|2.4.2+|

## Varnish

| Magento Minor Version | 3.5 | 4.x | 5.x | 6.x |
|:---|---|---|---|---|
|2.0|✓|✓|✗|✗|
|2.1|✓|✓|✗|✗|
|2.2|✗|✓|✓|✗|
|2.3|✗|✓|✓<sup>1</sup>|✓<sup>2</sup>|
|2.4|✗|✗|✗|✓<sup>3</sup>|

Notes:
1. Magento declares support for 5.2+
2. Magento declares support for 6.2+, 6.5.1 explicitly supported with 2.3.7
3. Tested with 6.3.1.  Magento 2.4.2 tested with 6.4

## Databases

### MySQL

| Magento Minor Version | 5.6 | 5.7 | 8.0 |
|:---|---|---|---|
|2.0|✓|✗|✗|
|2.1|✓|2.1.2+|✗|
|2.2|✓|✓|✗|
|2.3|✓<sup>1</sup>|✓|✗|
|2.4|✗|✓<sup>1</sup>|✓|

Notes:
1. Magento is also compatible with, but has not been tested and is not recommended

### MariaDB

| Magento Minor Version | 10.0 | 10.1 | 10.2 | 10.3 | 10.4 | 10.5 |
|:---|---|---|---|---|---|---|
|2.0|✓|✓|✗|✗|✗|✗|
|2.1|✓|✓|2.1.2+|✗|✗|✗|
|2.2|✓|✓|✓<sup>1</sup>|✓<sup>1</sup>|✓<sup>1</sup>|✗|
|2.3|✓<sup>1</sup>|✓<sup>1</sup>|✓<sup>1</sup>|✓<sup>1</sup>|✓<sup>1</sup>|✗|
|2.4|✗|✗|✓<sup>2</sup>|✓<sup>2</sup>|✓<sup>2</sup>|✓|

Notes:
1. Magento only uses MySQL features compatible with MariaDB. MariaDB may not be compatible with all MySQL features, however, so be sure to research compatibility issues before using a feature in your Magento module.
2. Magento is also compatible, but has not been tested and is not recommended
