Source code -> Tokens -> Abstract Syntax Tree -> Evaluation

From source code to tokens, is called “lexical analysis”. It’s done by a lexer (also called tokenizer

Tokens itself are small, easily categorizable data structures that are then fed to the parser, which does the second transformation and turns the tokens into an “Abstract Syntax Tree”.

Here’s an example. This is the input one gives to a lexer:

"let x = 5 + 5;"

And what comes out of the lexer looks kinda like this:

[
LET,
IDENTIFIER("x"),
EQUAL_SIGN,
INTEGER(5),
PLUS_SIGN,
INTEGER(5),
S
