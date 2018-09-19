##Chapter 1 Quiz: What is Scope? 
```
function foo(a) {
   	var b = a;
   	return a + b;
   }
   
   var c = foo( 2 );
   ```

1. Find all the LHS look ups (there are 3.)
- `foo( 2 )` (where a = 2)
- `var b = a`
- `var c = foo(2)`


2. Find all the RHS look ups (there are 4.)
- `var b = a` where a looks inside of function scope and finds foo(a)
- ` a + ` where a looks inside of function scope and finds foo(a)
- ` + b ` where b looks inside of function scope and finds var b 
- `var c = foo( 2 )` where foo( 2 ) looks up the function foo()
