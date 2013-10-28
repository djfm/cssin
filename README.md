cssin
=====

A CSS inliner that works pretty well.

#Features

* Resting on standard, proven tools to do the heavy lifting, cssin is less prone to errors than other CSS inliners out there.
* Uses [CSSTidy] (http://csstidy.sourceforge.net/), a real CSS parser, i.e. a parser that doesn't just use a bunch of regexps and choke on weird input.
* Uses [PHP Simple HTML DOM Parser] (http://simplehtmldom.sourceforge.net/) to parse and modify the HTML. It uses regexps internally, which is bad, but this parser is robust and well tested.
* It is not extremely slow.
* It will not hurt your cat, although I decline any responsibility if it does.

#License

Do whatever you like if it is free.

#Usage

```php

$cssin = new CSSIN();

$html_with_inlined_css = $sccin->inlineCSS('http://some_url.com/file.html');

```
