## Local Hosting for Development

### LAMP/WAMP/MAMP

- http://www.wampserver.com - Windows
- http://www.mamp.info - Mac & Windows

#### For MAMP, localhost => http://localhost:8888/
	- default folder: /Applications/MAMP/htdocs/
#### For WAMP, localhost => http://localhost/
	- default folder: C:\wamp\www
	- 
---

## Intro to PHP

##### Single Quote vs. Double Quote
###### Double quotes 
1. Parses strings => slower
2. Best suited for:
  * escaped strings
  * strings with multiple variables and plain text
  * condensing multi-line concatenation, & improving readibility

```php
<?php
echo 'phptherightway is ' . $adjective . '.'
	. "\n"
	. 'I love learning' . $code . '!';
?>
```
- single quotes => uses multiple concatenating for variables & escaped string

vs.
```php
<?php
echo "phptherightway is $adjective.\n I love learning $code!"
?>
```
- double quotes => enables us to use a parsable string
