# java-script-demo

### variables ###

```
* var x = 10  vs   x = 10
```


#### variables scopes ####
``` 
* java script follows functional scopping not block scopping
```
```javascript
var name="anand"
if(name=="anand") {
  var gender = "male"
}
console(name);
console(gender);  // accessable even outside the if scope
```
```javascript
function scopeDemo() {
  var name="anand"
  if(name=="anand") {
    var gender = "male"
  }
  console(name);
  console(gender);  // accessable even outside the if scope
}

console(gender);  // runtime exception : gender is reading without write operation

```


#### equals ( = | == | === ) ####
```
* var x=5  , var y="5" .   x==y -> true .   x===y -> false
```
