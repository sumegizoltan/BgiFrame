BgiFrame
========

bgiframe for IE6 - without jQuery 

The original jQuery.bgiframe plugin in pure javascript.

Based on
--------

https://github.com/brandonaaron/bgiframe

The jQuery plugin copyrights:
Copyright (c) 2013 Brandon Aaron (http://brandonaaron.net)

NuGet package
-------------

https://nuget.org/packages/typecript.bgiframe

Usage
-----

Usage of the native javascript plugin:
```html
<html>
<head>
    <meta charset="utf-8" />
    <title>TypeScript HTML App</title>
    <script type="text/javascript" src="Scripts/typescript.bgiframe.js"></script>
</head>
<body>
  <h1>TypeScript HTML App for plugin bgiframe (IE6)</h1>

  <div id="content">content</div>
  <div id="content2">content2</div>

  <input type="button" name="btnRefresh" value="refresh content2" onclick="refresh();" />
  
  <script type="text/javascript">
```
  ```javascript
      var content = document.getElementById('content');
      var bgiframe = new BgiFrame.Bgiframe(content);

      function refresh() {
          if (bgiframe) {
              // bgiframe.fire(document.getElementById('content'));
              bgiframe.fire(document.getElementById('content2'));
          }
      }
  ```
```html
  </script>
</body>
</html>
```
