# SecurityScanner

A basic tool for detecting vulnerabilities in web applications

## Requirements

 * PHP 5.5.0+

## Installation

 * Install via [Composer](https://getcomposer.org/) (recommended)

   `$ composer require delight-im/security-scanner`

   Include the Composer autoloader:

   `require __DIR__.'/vendor/autoload.php';`

 * or
 * Install manually
   * Copy the contents of the [`src`](src) directory to a subfolder of your project
   * Include the files in your code via `require` or `require_once`

## Usage

```
// header('Content-type: text/plain; charset=utf-8');

$scanner = new \Delight\SecurityScanner\SecurityScanner('http://www.example.com/');
$scanner->run();
$scanner->printResults();
```

## More advanced tools

 * [OWASP Zed Attack Proxy (ZAP)](https://github.com/zaproxy/zaproxy)
 * [Vega](https://subgraph.com/vega/)
 * [Wapiti](http://wapiti.sourceforge.net/)
 * [Nikto](https://github.com/sullo/nikto)
 * [Grabber](http://rgaucher.info/beta/grabber/)
 * [GoLismero](https://github.com/golismero/golismero)
 * [Detectify](https://detectify.com/)
 * [HP WebInspect](http://www8.hp.com/us/en/software-solutions/webinspect-dynamic-analysis-dast/index.html)
 * [Burp Suite](https://portswigger.net/burp/)

## Contributing

All contributions are welcome! If you wish to contribute, please create an issue first so that your feature, problem or question can be discussed.

## Disclaimer

You should probably use this library with your own websites and repositories only.

## License

```
Copyright (c) delight.im <info@delight.im>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
