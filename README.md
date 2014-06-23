cssin
=====

A CSS inliner that works pretty well.

#Features

* CSSIN understands the !importance of !important CSS properties.
* CSSIN will parse your HTML document and retrieve the CSS stylesheets all by itself, you don't need to tell it what to do.
* Resting on standard, proven tools to do the heavy lifting, cssin is less prone to errors than other CSS inliners out there.
* Uses [CSSTidy] (http://csstidy.sourceforge.net/), a real CSS parser, i.e. a parser that doesn't just use a bunch of regexps and choke on weird, valid input.
* Uses [PHP Simple HTML DOM Parser] (http://simplehtmldom.sourceforge.net/) to parse and modify the HTML. It uses regexps internally, which is bad, but this parser is robust and well tested.
* It is not extremely slow.
* It will not hurt your cat, although I decline any responsibility if it does.

#License

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>

#Usage

```php

require 'cssin.php'

$cssin = new FM\CSSIN();

$html_with_inlined_css = $cssin->inlineCSS('http://some_url.com/file.html');

```
