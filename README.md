dokku-nodejs
----------------------

dokku-nodejs is a plugin for [dokku][dokku] that injects node, and installs packages specified within your dokku app's package.json file.

Suitable for non node.js apps with Javascript SPAs. Doesn't require modification to your buildpack (Python, Ruby, etc.).

Installation
------------
```
cd /var/lib/dokku/plugins
git clone https://github.com/ademuk/dokku-nodejs nodejs
dokku plugins-install
```

NPM Scripts
-----------

There is a known issue whereby npm scripts are not executed due to dokku running as root.
[See issue here for a solution](https://github.com/progrium/dokku/wiki/Troubleshooting).

## License

The MIT License (MIT)

Copyright (c) 2014 Adem Gaygusuz

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[dokku]: https://github.com/progrium/dokku
