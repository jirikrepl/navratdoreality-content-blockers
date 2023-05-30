# navratdoreality-content-blockers

## javascript by chee plugin

```javascript
function blockElementsPeriodically() {
  // Select the elements using XPath
  var xpathExpression = "//div[@class='item'][.//a[text()='porno']]";
  var matchingElements = document.evaluate(xpathExpression, document, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE, null);

  // Iterate over the matching elements
  for (var i = 0; i < matchingElements.snapshotLength; i++) {
    var element = matchingElements.snapshotItem(i);
    // Hide or remove the element
    element.style.display = "none";  // To hide the element
    // element.parentNode.removeChild(element);  // To remove the element from the DOM
  }
}

// Run the blocking script every 1 seconds (adjust the interval as needed)
setInterval(blockElementsPeriodically, 1000);
```

## Stylus plugin

```css
#banner-list1, #banner-list2, #snippet--banners-bot {
    display: none;
}

.jumbotron, .sidebar {
    display: none;
}
```
