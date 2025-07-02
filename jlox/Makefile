.PHONY: run
run: lox/Lox.class
	java lox.Lox

.PHONY: test
test: lox/Lox.class
	java lox.Lox test.lox

.PHONY: gen/ast
gen/ast: tool/GenerateAst.class
	java tool.GenerateAst lox

tool/GenerateAst.class: tool/GenerateAst.java
	javac tool/GenerateAst.java

lox/Lox.class: lox/*.java
	javac lox/Lox.java

