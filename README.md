<p align="center">
	<img src="./lahlang-extension/icon.png" alt="Lahlang icon" width="140" />
</p>

<p align="center">
	<a href="https://x.com/suryanshkush10">
		<img src="https://img.shields.io/badge/Follow%20on%20X-000000?style=for-the-badge&logo=x&logoColor=white" alt="Follow on X" style="height: 30px; border-radius: 4px;" />
	</a>
	<a href="https://buymeacoffee.com/suryanshkushwaha">
		<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" style="height: 30px;" />
	</a>
</p>

# Lahlang 🇸🇬

> A programming language for Singaporeans, by not a Singaporean yet. Can one lah!

## Table of Contents

- [Overview](#overview)
- [Documentation](#documentation)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Language Examples](#language-examples)
- [Wall of Lah](#wall-of-lah)
- [CLI Options](#cli-options)
- [Project Structure](#project-structure)
- [Architecture](#architecture)
- [Testing](#testing)
- [Contributing](#contributing)
- [Support](#support)
- [Star History](#star-history)
- [License](#license)

---

## Overview

Lahlang is a fun, expressive programming language inspired by Singlish and Singaporean culture. It’s designed for learning, experimentation, and joy, with syntax and keywords that reflect local slang and humor.

## Documentation

For a complete guide on how to use Lahlang, check out our extensive documentation:

1.  **[Installation Guide](./docs/01-Installation.md)**: Node.js/pnpm prerequisites and global CLI installation.
2.  **[VS Code Extension](./docs/02-VSCode-Extension.md)**: How to get syntax highlighting.
3.  **[Getting Started](./docs/03-Getting-Started.md)**: Your first `.lah` file and "Hello World".
4.  **[Variables and Types](./docs/04-Variables-and-Types.md)**: Data handling with Singlish types.
5.  **[Control Flow](./docs/05-Control-Flow.md)**: Logic with `confirm or not` and `which one lah`.
6.  **[Loops](./docs/06-Loops.md)**: Iteration with `keep going lah` and `every one also`.
7.  **[Functions](./docs/07-Functions.md)**: Defining and calling reusable blocks.
8.  **[Error Handling](./docs/08-Error-Handling.md)**: Wholesome and **Spicy 🌶️** tiers.
9.  **[CLI Reference](./docs/09-CLI-Reference.md)**: Commands, debugging, and meta keywords.
10. **[Examples Walkthrough](./docs/10-Examples-Walkthrough.md)**: Deep dive into the `examples/` folder.

## Features

- **Singlish Syntax:** Keywords like `eh listen lah`, `ok lah bye`, `oi`, `confirm or not`, `keep going lah`, etc.
- **Interactive REPL:** Run `lahlang` with no arguments to enter the REPL — type Singlish code line by line with multi-line support.
- **VS Code Support:** Get syntax highlighting with the [Lahlang VS Code Extension](https://marketplace.visualstudio.com/items?itemName=suryanshkushwaha.lahlang-vscode).
- **Variables & Constants:** `eh got`, `confirm got`
- **Control Flow:** `confirm or not` (if), `or maybe` (else if), `abuden` (else), `keep going lah` (while), `one by one lah` (for), `every one also` (foreach), `hantam lah...until` (do-while)
- **Functions:** `steady lah do this`, `here take`, `eh do this`, `one time only`, `jio` (casual call)
- **Error Handling:** `see how lah`, `aiyoh kena`, `confirm do`, `jialat throw`, `paiseh warn`, `hong gan lah`, `chao cb assert`, `act blur` (silent try)
- **Types:** `words` (string), `nombor` (number), `can cannot` (boolean), `whole list` (array), `all the things` (object)
- **Singlish Expressions:** `kaypoh` (typeof), `gostan` (reverse), `swee` (pretty print), `agak agak` (round), `makan` (pop), `tabao` (clone), `chope` (freeze), `sabo` (delete), `die die must` (assert), `sian`/`lepak` (sleep)
- **Built-in Methods:** String methods (`.upper()`, `.lower()`, `.trim()`, `.split()`, etc.), array methods (`.push()`, `.pop()`, `.map()`, `.filter()`, etc.), object methods (`.keys()`, `.values()`, `.entries()`), and global helpers (`panjang`, `to_nombor`, `to_words`, math functions)
- **String Escapes:** `\n`, `\t`, `\r`, `\\`, `\"` inside double-quoted strings
- **Operators:** `same same` (==), `not same` (!=), `and also` (&&), `or can` (||), `add some more` (+=), `minus a bit` (-=)
- **Comments:** `// shiok:` (single-line), `wahlau start ... wahlau end` (multi-line)
- **Meta:** `chiong bring in` (import), `share out` (export), `eh check this` (debug/inspect)
- **Spicy Error Types:** `JialatError`, `BoJioError`, `SiaoError`, `TokKokError`, `TanKuKuError`, `SuayError`, `WahLauError`, `GoneCase`, `CbError`, `LanJiaoError`, `CcbError`

## Installation

Install globally using [pnpm](https://pnpm.io):

```bash
pnpm i -g lahlang
```

## Usage

Run a `.lah` file:

```bash
lahlang myfile.lah
```

Or start the interactive REPL:

```bash
lahlang
```

```
lah> oi "Hello from REPL!"
Hello from REPL!
lah> eh got x = 42
lah> oi x + 8
50
```

Type Singlish code directly — no need for `eh listen lah` / `ok lah bye` wrappers. Multi-line blocks (with `{}`) are supported. Press Ctrl+C to exit.

To close REPL with a keyword, type `bye lah` on its own line.

## Language Examples

### Hello World

```lah
eh listen lah
	oi "Hello World";
ok lah bye
```

### FizzBuzz

```lah
eh listen lah
	one by one lah (i from 1 to 15) {
		confirm or not (i % 15 same same 0) {
			oi "FizzBuzz";
		} or maybe (i % 3 same same 0) {
			oi "Fizz";
		} or maybe (i % 5 same same 0) {
			oi "Buzz";
		} abuden {
			oi i;
		}
	}
ok lah bye
```

### Data Structures

```lah
eh listen lah
	eh got my_list = [1, 2, "shiok", can];
	oi my_list;
	every one also (item in my_list) {
		oi item;
	}
	eh got my_bag = {
		food: "Chicken Rice",
		price: 4.5,
		tasty: can
	};
	oi my_bag;
ok lah bye
```

### Advanced Logic

```lah
eh listen lah
	steady lah do this makeCounter(start) {
		eh got count = start;
		steady lah do this increment() {
			eh change count = count + 1;
			here take count;
		}
		here take increment;
	}
	eh got my_counter = makeCounter(10);
	oi my_counter();
ok lah bye
```

### Singlish Expressions

```lah
eh listen lah
	// typeof
	oi kaypoh "hello";          // "words"
	oi kaypoh 42;               // "nombor"

	// reverse
	oi gostan "lahlang";        // "gnalhal"
	oi gostan [1, 2, 3];        // [3, 2, 1]

	// round
	oi agak agak 3.7;           // 4

	// pretty print
	eh got obj = { name: "Ah Beng", age: 25 };
	swee obj;

	// clone and freeze
	eh got copy = tabao obj;
	chope obj;

	// silent error handling
	act blur {
		jialat throw "this error is swallowed";
	}

	// assert
	die die must (1 + 1 same same 2);
ok lah bye
```

### Do-While Loop

```lah
eh listen lah
	eh got i = 0;
	hantam lah {
		oi i;
		eh change i = i + 1;
	} until (i less than 5)
ok lah bye
```

### Built-in Methods

```lah
eh listen lah
	// String methods
	eh got s = "hello world";
	oi s.upper();               // "HELLO WORLD"
	oi s.split(" ");            // ["hello", "world"]
	oi panjang(s);              // 11

	// Array methods
	eh got arr = [3, 1, 2];
	oi arr.sort();              // [1, 2, 3]
	oi arr.map(steady lah do this(x) { here take x * 2; });

	// Type conversion
	oi to_nombor("42");         // 42
	oi to_words(100);           // "100"
ok lah bye
```

## Wall of Lah

We do it for the community one lah.

Contribute any `.lah` example and get featured automatically as a repository contributor on the Wall of Lah.

See contribution details in [wall-of-lah/README.md](./wall-of-lah/README.md).

## CLI Options

- `lahlang <file.lah>`: Run a Lahlang program.
- `lahlang`: Start the interactive REPL.
- Only `.lah` files are accepted.
- Errors are reported in Singlish style, e.g. `[TOK KOK]`, `[RUNTIME ERROR]`, `[FATAL]`, `[ALAMAK]`.

## Project Structure

```
lahlang/
├── src/                # Source code (lexer, parser, interpreter, CLI)
├── examples/           # Example .lah programs
├── tests/              # Unit and integration tests
├── package.json        # Project metadata and scripts
├── tsconfig.json       # TypeScript config
├── vitest.config.ts    # Test config
```

## Architecture

- **Lexer:** Tokenizes source code using Singlish keywords.
- **Parser:** Builds AST from tokens, supports all language features.
- **Interpreter:** Executes AST, manages environment, handles errors.
- **CLI:** Entry point for running `.lah` files, handles file I/O and error reporting.

## Testing

Run all tests with:

```bash
pnpm test
```

- Uses [Vitest](https://vitest.dev/) for unit and integration tests.
- Test coverage includes lexer, parser, interpreter, error handling, and full language features.

## Contributing

Contributions are welcome! Please open issues or pull requests for:

- Bug fixes
- Feature requests
- Documentation improvements
- New examples

---

## Star History

<a href="https://www.star-history.com/?repos=suryanshkushwaha%2Flahlang&type=date&legend=top-left">
 <picture>
	 <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=suryanshkushwaha/lahlang&type=date&theme=dark&legend=top-left" />
	 <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=suryanshkushwaha/lahlang&type=date&legend=top-left" />
	 <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=suryanshkushwaha/lahlang&type=date&legend=top-left" />
 </picture>
</a>

---

## Support

If Lahlang helps you or made you smile, you can support the project here:

- GitHub Sponsors: https://github.com/sponsors/suryanshkushwaha
- Buy Me a Coffee: https://buymeacoffee.com/suryanshkushwaha

## License

MIT License

---
