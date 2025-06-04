> This informal introduction leaves a lot unspecified. List several open
> questions you have about the language’s syntax and semantics.
> What do you think the answers should be?

Calling superclass methods, which I think should probably like:

```
class Brunch < Breakfast {
  serve(who) {
    var result = super.serve(who);
    return "Brunch: " + result;
  }
}
```

Are classes first-class objects like functions? Can they be defined in a
function body?

```
fun something() {
  class Thing {
    dance() { ... }
  }

  return Thing()
}
```

There are no modules or packages or anything like that. Is everything in the
same scope?

> Lox is a pretty tiny language. What features do you think it is missing that
> would make it annoying to use for real programs? (Aside from the standard
> library, of course.)

Modules/packages would probably be useful. Also some system for error-handling.
