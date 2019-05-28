---
# Set page.title to match site.title so it is not added to the top of the page
# body by the default theme <https://github.com/pages-themes/primer>.
title: net-api-browser-opensearch
---

{% include_relative README.md %}

<script type="text/javascript">
(function() {
  'use strict';

  // Add a clickable button to install the OpenSearch Description.

  function addSearchProvider() {
    if (typeof window.external.AddSearchProvider !== 'function') {
      alert('Error: AddSearchProvider function not available.');
    } else {
      try {
        window.external.AddSearchProvider('net-api-browser-opensearch.xml');
      } catch (err) {
        alert('Error: ' + err);
      }
    }
  }

  var button = document.createElement('button');
  button.onclick = addSearchProvider;
  // Style similarly to "Add" button on addons.mozilla.org for usability
  button.setAttribute(
    'style',
    'display: block;'
    + ' margin: 0 auto 16px;'
    + ' padding: 0.5em 1em;'
    + ' color: white;'
    + ' background-color: #0060df;'
    + ' border: 1px solid transparent;'
    + ' border-radius: 2px;'
  );
  button.type = 'button';
  button.appendChild(document.createTextNode('Add .NET API Browser Search'));

  var selfLink = document.getElementById('nojs-self-link');
  selfLink.innerText = 'by clicking the following button:';

  var selfP = selfLink.parentNode;
  selfP.parentNode.insertBefore(button, selfP.nextSibling);
}());
</script>
