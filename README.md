# refer to
* https://www.twilio.com/blog/how-to-build-a-cli-with-node-js
# test
```
mkdir ~/test-dir
cd ~/test-dir
create-project typescript --git
```
# test with install
```
create-project typescript --git --install
```
# make your own
If you want to make your code consumable as an actual module so that others can reuse your logic in their code, we'll have to add an index.js file to our src/ directory that exposes the content from main.js:
```
require = require('esm')(module);
require('../src/cli').cli(process.argv);
```
# npm publish
```
npm pack --dry-run
```
or
```
np
```
# fork from
npm init @dkundel/project

* Email: dkundel@twilio.com
* Twitter: @dkundel
* GitHub: dkundel
* dkundel.com
