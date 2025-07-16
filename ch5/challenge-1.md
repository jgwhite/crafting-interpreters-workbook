```
expr → expr ( "(" ( expr ( "," expr )* )? ")" | "." IDENTIFIER )+
     | IDENTIFIER
     | NUMBER

expr → expr "(" ")"
expr → expr "(" expr ")"
expr → expr "(" expr "," expr ")"
expr → expr "(" expr "," expr "," expr ")"
expr → expr "(" expr "," expr "," expr "," expr ")"
expr → expr "." IDENTIFIER
expr → IDENTIFIER
expr → NUMBER
```
