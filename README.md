# bootswitch
Bookmarket for Bootstrap theme live preview. Supports all [Bootswatch themes](http://www.bootstrapcdn.com/#bootswatch_tab).

## Bookmarklet
Add the following code to your bookmarks bar:

```javascript
javascript:(function(){var theme=window.prompt('Enter the name of a Bootstrap theme:');Array.prototype.forEach.call(document.querySelectorAll('link[rel=stylesheet]'),function(link){if(!theme||theme==='default'){link.href='//maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css'}else if(link.href.search(/bootstrap(\.min)?\.css/)!=-1){link.href='//maxcdn.bootstrapcdn.com/bootswatch/3.3.1/'+theme+'/bootstrap.min.css'}})})();
```
