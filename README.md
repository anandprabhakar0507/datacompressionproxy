# Data Compression Proxy (deprecated)

**This extension is no longer supported. I do not take any responsibility for the current version in Chrome Web Store. Please use the official [Data Saver](https://chrome.google.com/webstore/detail/data-saver-beta/pfmgfdlgomnbgkofeojodiodmgpgmkac) extension from Google instead.**

This is an experimental extension for Google Chrome bringing [Chrome Data Compression Proxy](https://developers.google.com/chrome/mobile/docs/data-compression) from mobile to desktop PCs.

Version 2.0 added statistics, custom bypass and adblock lists.

## How it works

The extension sends all HTTP (but not HTTPS) traffic through Chrome Data Compression Proxy server, which uses SPDY protocol to speed up web browsing. Enabled state is indicated by a green icon. You can manually disable the proxy by clicking on it. When the proxy raises an error, it is being automatically disabled for adjustable number of seconds, so that the request can be resent.

The extension uses either `chrome.webRequest` (slower) in Chrome Stable or `chrome.declarativeWebRequest` (faster but without the stats) in Chrome Beta/Dev, so ignore any warnings.

## Statistics

You can find the savings statistics in Options, based on the `content-length` header.

## Disclaimer

The extension is provided as is with no warranty. Use it at your own risk. It is not affiliated with Google.
