lox/Lox.class: lox/*.java
	javac lox/Lox.java

run: lox/Lox.class
	java lox.Lox

test: lox/Lox.class
	java lox.Lox test.lox

tool/GenerateAst.class: tool/GenerateAst.java
	javac tool/GenerateAst.java

gen/ast: tool/GenerateAst.class
	java tool.GenerateAst lox

