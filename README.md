Playwright process bug
===

If you import chromium from playwright, the parent node process can no longer be exited with control-c.

## Steps to reproduce

1. Clone this repo
2. run `node index.js`.
3. Try and kill the process with control-c. It will not work

To fix it, comment out the chromium import line in `my-module.js`.
