### Requirements for personal wiki

* Searchable
* Shows recent content?
* Plain text storage?
* Web front-end (only search from here, OK)
* Encrypted?
* NOT Wiki-markup
* Reasonable to get content out
* Doesn't use something disgusting like PHP
* Can make entries easily on Android
* Few dependencies (e.g. no ruby+rubygems)
* Content OK with being synced across devices (dropbox or git-annex like syncing)


### personal notes/wiki server wishlist

* markdown files rendered via javascript
  * https://github.com/evilstreak/markdown-js
* small angular app to search elastic search

* download markdown via ajax, render in browser, fancy urls that work forever

* ingestion into elasticsearch runs as a post-receive hook on git repo
* parse title, date, tags, and content into json doc
* send json doc to elasticsearch
* need to know how ES uniquely identifies documents


* would need small api to front elastic search...don't want to expose to interwebs

* is there any alternative to elastic search (non-runtime)
  * sphinx but api looks rough comparatively


### write angular app to fetch and render markdown
