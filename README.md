# VueJsNotes
Little tips and tricks for VueJs 2.0, that may come in handy

# Find Components on the page by name:
```
mounted: function () {
    window.App = this
    // add a utility method to retrieve children by name
    window.fc = function (cName) {
      cName =cName.toLowerCase()
      return _.filter(window.App.$children, function(f){
        return f.$options.name.toLowerCase() == cName
      })
    }
  }
 ```
 
 
