# URL obfuscation

Different methods to obfuscate URLs.

Tools will come soon.

## Examples

Consider `http://facebook.com` as target URL.

Tested so far on Mozilla Firefox 56.0 and Google Chrome 62.0.3202.89.

### Dummy HTTP basic auth

Firefox shows an alert confirmation.

`http://dummy_username@facebook.com`

### URL redirection

Similar to URL shortener.

The sample domain needs to be replaced with a real URL redirection.

A third exploitable website could be used. See for example [Joomla! 1.5 - URL Redirecting](https://www.exploit-db.com/exploits/14722/).

`http://sample.tld/redirect-to=facebook.com`

### URL shortener

`https://goo.gl/mS4A`

### IP obfuscation

#### Decimal 8 bits

`http://31.13.83.36`

#### Decimal 32 bits

`http://520966948`

#### Octal 8 bits

`http://037.015.0123.044`

#### Octal 32 bits

`http://03703251444`

#### Hexadecimal 8 bits

`http://0x1f.0xd.0x53.0x24`

#### Hexadecimal 32 bits

`http://0x1f0d5324`

## Mixings

### Dummy HTTP basic auth + decimal 32 bits

`http://github.com@520966948`
