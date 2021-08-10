# Lark.js

**Generate LALR(1) parsers in Javascript**

Lark is a popular parsing toolkit for Python.

This project is a port of the Lark standalone parser to Javascript.

Lark.js takes a `.lark` grammar, and from it generates a standalone Javascript parser.

The generated Javascript module will include Lark's base classes and utilities, 
such as `Tree`, `Transformer`, `Visitor` and `InteractiveParser`.

**Lark grammars**

Lark grammars are written in an augmented EBNF (a textual format), and usually use the `.lark` extension.

Because they are purely declarative, and don't contain code, they are entirely portable between languages.

It is now possible to use Lark grammars in 3 languages: Python, Javascript and Julia.

### Install Lark.js

Install lark-js on Python:

```sh
    pip install lark-js --upgrade
```

### Generate a Javascript LALR(1) parser

```sh
	lark-js my_grammar.lark -o my_parser.js
```

For help, run:

```sh
	lark-js --help
```

### Quick links

- [Lark](https://https://github.com/lark-parser/lark) - The Python library
- [Online IDE](https://lark-parser.github.io/ide)
- [Gitter chat](https://gitter.im/lark-parser/Lobby) - A place to ask questions and discuss

## Features

 - Builds a parse-tree (AST) automagically, based on the structure of the grammar
 - **LALR(1)** parser - Fast and light
 - **EBNF** grammar
 - Usable in the browser and in Node.js
 - Line & column tracking
 - Standard library of terminals (strings, numbers, names, etc.)
 - Import grammars from Nearley.js

 Planned features:

 - Support for Earley

### Syntax Highlighting

Lark provides syntax highlighting for its grammar files (\*.lark):

- [Sublime Text & TextMate](https://github.com/lark-parser/lark_syntax)
- [vscode](https://github.com/lark-parser/vscode-lark)
- [Intellij & PyCharm](https://github.com/lark-parser/intellij-syntax-highlighting)
- [Vim](https://github.com/lark-parser/vim-lark-syntax)
- [Atom](https://github.com/Alhadis/language-grammars)

### Automatic sync with the Python code

Ports from one language to another are often at risk of falling out of sync as time goes on.

But Lark.js wasn't just written by hand -- it was transpiled directly from Lark's Python code!

That means that futures updates to Lark-Python will be automatically added to Lark.js too. 

## License

Lark.js uses the [MIT license](LICENSE).

## Contribute

Lark.js is accepting pull-requests. If you would like to help, open an issue or find us on gitter.

## Sponsoring

Lark.js was made possible with the help of a generous donation by [Smore](https://www.smore.com/) ❤️

If you like Lark, and want to see it grow, please consider [sponsoring us!](https://github.com/sponsors/lark-parser)
