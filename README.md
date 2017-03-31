# Thunderbird Grammar Checker
Thunderbird extension for checking grammar using LanguageTool facilities. This extension is compatible only with Thunderbird 1.5 and above.

Homepage: [Thunderbird Grammar Checker extension
](http://nuald.blogspot.com/2009/10/thunderbird-grammar-checker-extension.html)

## Quick Start

The extension uses either a local LanguageTool server (recommended) or the public one.
Please note that the public server has the certain restrictions: [Public HTTP API](http://wiki.languagetool.org/public-http-api).

To use the local server, please [download](https://languagetool.org/) the stand-alone version for the desktop, unpack and run it as described here: [HTTP Server](http://wiki.languagetool.org/http-server).

The sample instructions:

    $ wget https://languagetool.org/download/LanguageTool-3.7.zip
    $ unzip LanguageTool-3.7.zip
    $ cd LanguageTool-3.7
    $ java -cp languagetool-server.jar org.languagetool.server.HTTPServer --port 8081

## Development

In general, please follow the [Thunderbird extensions](https://developer.mozilla.org/en-US/Add-ons/Thunderbird) official documentations. There are several [Gradle](https://gradle.org/) tasks specified to make the development easier:

- `gradle eslint` __[Run ESLint check for the JS files]__
- `gradle xpi` __[Package the XPI file for the deployment]__
