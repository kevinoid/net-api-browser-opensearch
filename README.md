# Unofficial [OpenSearch Description](https://github.com/dewitt/opensearch) for the [.NET API Browser](https://docs.microsoft.com/dotnet/api/)

This project contains an **unofficial** [OpenSearch
Description](https://github.com/dewitt/opensearch) which can be used to search
the [.NET API Browser](https://docs.microsoft.com/dotnet/api/) directly from a
browser search box.


## Installation

This OpenSearch Description file can be added to a browser
<!-- The following is replaced (by ID) with an install button on index.md -->
<span id="nojs-self-link">from
<https://kevinoid.github.io/net-api-browser-opensearch/> (on JavaScript-enabled
browsers).</span>

Alternatively, run the following code in the browser console or address bar:

```js
window.external.AddSearchProvider('https://kevinoid.github.io/net-api-browser-opensearch/net-api-browser-opensearch.xml');
```


## Enabling Autodiscovery

To enable [autodiscovery of search
plugins](https://developer.mozilla.org/en-US/docs/Web/OpenSearch#Autodiscovery_of_search_plugins)
it would be preferable if this OpenSearch Description were referenced by the
pages on the .NET API Browser site.  That has been proposed in
[MicrosoftDocs/feedback#52](https://github.com/MicrosoftDocs/feedback/issues/52)
which has not seen any recent activity.


## License

To the extent possible under law, the author of this work (Kevin Locke) has
waived all copyright and related or neighboring rights to this work.  See the
[CC0 Public Domain Dedication](COPYING.txt) for details.
