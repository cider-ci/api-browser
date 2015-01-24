
# Deprecation Notice

**This component is not used by Cider-CI anymore.**

Cider-CI switched from HAL to [JSON-ROA](http://json-roa.github.io/) 
and the [JSON-ROA Browser](http://json-roa.github.io/browser/about.html)
in version 2.0 and later.



Cider-CI API  browser
======================

This is a slightly adopted variant of [The HAL Browser](https://github.com/mikekelly/hal-browser.git)
for the [Cider-CI Project](https://github.com/cider-ci/cider-ci.git).


About HAL
========
HAL is a format based on json that establishes conventions for
representing links. For example:

```javascript
{
    "_links": {
        "self": { "href": "/orders" },
        "next": { "href": "/orders?page=2" }
    }
}
```

More detail about HAL can be found at
[http://stateless.co/hal_specification.html](http://stateless.co/hal_specification.html).

Instructions
============
All you should need to do is copy the files into your webroot.
It is OK to put it in a subdirectory; it does not need to be in the root.

All the JS and CSS dependencies come included in the vendor directory.


TODO
===========
* Make Location and Content-Location headers clickable links
* Provide feedback to user when there are issues with response (missing
self link, wrong media type identifier)
* Give 'self' and 'curies' links special treatment
