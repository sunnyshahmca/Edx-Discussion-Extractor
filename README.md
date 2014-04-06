Edx discussion data extractor is implemented using Google chrome extension which uses cross-site-scripting to extract data using AJAX APIs of Edx. Google extensions are not allowed to access local file-system, so we implemented one node.js web-server to store the data. chrome-extension posts the data retrieved from Edx to node.js webserver which internally writes it to local filesystem.

Check comments in chrome-extension/content.js to understand the usage of plugin. 