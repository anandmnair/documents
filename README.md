# java-script-demo

### variables ###

```
* var x = 10  vs   x = 10
```


#### equals ( = | == | === ) ####
```
* var x=5  , var y="5" .   x==y -> true .   x===y -> false
```


#### variables scopes ####
* global variables : stored iin window object
* functional variables 
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

#### IIFE ####

**I**mmediately **I**nvoked **F**unction **E**xpression

```
 - Always make a variable with in functional scope 
 - anonymous function
```

```javascript
(function() {
 console.log("hello anand")
})();     // this anonymous function calling at the same point of declaration - > IIFE  
```


```javascript
var fun = (function() {        //save funtion to fun variable
 console.log("hello anand")
});
fun(); // calling anonymous function from the reference var
```
