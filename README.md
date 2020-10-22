# Magento 2 Supported Versions

This repository is an up-to-date table of the versions of various software that various versions of Magento support.

## PHP

| Magento Minor Version | PHP 5.5 | PHP 5.6 | PHP 7.0 | PHP 7.1 | PHP 7.2 | PHP 7.3 | PHP 7.4 |
|:---|---|---|---|---|---|---|---|
|2.0|✓|✓|✓|✗|✗|✗|✗|
|2.1|✗|✓|✓<sup>[1]</sup>|2.1.16+|✗|✗|✗|
|2.2|✗|✗|✓<sup>[2]</sup>|✓|2.2.10+|✗|✗|✗|
|2.3|✗|✗|✗|✓<sup>[3]</sup>|✓|2.3.3+|2.3.7+|
|2.4|✗|✗|✗|✗|✗|✓|✓|

Notes:
1. Only 7.0.2 and ~7.0.6 for 2.1.0-2.1.1.  Starting with 2.1.2 that was expanded to include 7.0.4.
2. 7.0.2, 7.0.4, and ~7.0.6 for 2.2.0-2.2.4.  Starting with 2.2.5 7.0 support was limited to ~7.0.13
3. Supports ~7.1.3

## Elasticsearch

| Magento Minor Version | ES 1.x | ES 2.x | ES 5.x | ES 6.x | ES 7.x
|:---|---|---|---|---|---|
|2.1|✓<sup>1</sup>|✓<sup>2</sup>|2.1.1<sup>3</sup>|✗|✗|
|2.2|Until 2.2.8<sup>4</sup>|✓|2.2.8+|2.2.8+|✗
|2.3|✗|Until 2.3.5|Until 2.3.5|✓|2.3.5+
|2.4|✗|✗|✗|✗|✓<sup>5</sup>

Notes:
1. Versions 2.1.1-2.1.2 declare support for all 1.x, but all other 2.1.x versions only declare support for 1.7
2. Version 2.1.0 only declares support for 2.0 and 2.1.  All other lines claim support for 2.x
3. Version 2.1.1 is the only version in the 2.1.x line to declare support for ES 5, and then only for 5.0
4. 2.2.0-2.2.7 declare support for ES 1.7
5. 2.4.0 only declares support for 7.6.x

## RabbitMQ

| Magento Minor Version | 3.5 | 3.7 | 3.8 |
|:---|---|---|---|
|2.0|✓|✗|✗|
|2.1|✓|✗|✗|
|2.2|✓|✓|✗|
|2.3|✗|✓|✓|
|2.4|✗|✗|✓|
