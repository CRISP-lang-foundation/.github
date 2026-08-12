<p align="center">
  <img src="https://github.com/CRISP-lang-foundation/.github/blob/main/crisp-banner.png" width="100%" alt="Banner">
</p>

<h1 align="center">🦀 CRISP Language Foundation </h1>
<p align="center">

Welcome to the **CRISP Language Foundation** — the home of the **CRISP** programming language and its ecosystem.

CRISP (**C**reative **R**ust **I**mplemented **S**cripting **P**aradigm) is a modern, expressive scripting language inspired by Perl and built on Rust's safety and performance.

---

## 🌟 Mission

The CRISP Language Foundation exists to:

- **Develop and maintain** the CRISP programming language and its standard library
- **Foster a community** of developers, contributors, and users
- **Provide documentation** and educational resources
- **Ensure the language remains** open, free, and accessible to everyone

---

## 📦 Projects

### Core Projects

| Project | Description | Status |
|---------|-------------|--------|
| **[CRISP](https://github.com/CRISP-lang-foundation/CRISP-lang)** | The main interpreter and language implementation | 🚀 Active |
| **[crisp-mode](https://github.com/CRISP-lang-foundation/crisp-mode)** | Emacs major mode for CRISP | ✅ Stable |

### Upcoming Projects

- **CRISP Package Manager** — `crispan` — Package manager for CRISP
- **CRISP LSP** — Language Server Protocol implementation
- **CRISP VS Code Extension** — VS Code support
- **CRISP Web** — WebAssembly bindings

---

## 🚀 Get Started

### Installation

```bash
# Clone the repository
git clone https://github.com/CRISP-lang-foundation/crisp.git
cd crisp

# Build from source
cargo build --release

# Install
cargo install --path .
```

### Hello World

```crisp
# hello.csp
say "Hello, World!";
```

### Run

```bash
crisp hello.csp
```

### Or try the REPL

```bash
crisp
>>> say "Hello, World!";
Hello, World!
```

---

## 📚 Language Highlights

- **Perl-inspired syntax** — Expressive and concise
- **Rust-powered** — Memory-safe and fast
- **Optional sigils** — `$scalar`, `@array`, `%hash`
- **Native regular expressions** — Built-in regex support
- **Functional programming** — `map`, `grep`, `filter`, `sort`
- **Object-Oriented Programming** — Classes with inheritance
- **Pattern matching** — `match` with `where` guards
- **Error handling** — `try`/`catch`/`finally`
- **POSIX integration** — `use posix` for system calls
- **Embeddable** — Use CRISP as a scripting language in your Rust projects

---

## Examples

### FizzBuzz

```crisp
fn fizzbuzz(n) {
    for i in 1..n+1 {
        if i % 15 == 0 {
            say "FizzBuzz";
        } else if i % 3 == 0 {
            say "Fizz";
        } else if i % 5 == 0 {
            say "Buzz";
        } else {
            say i;
        }
    }
}

fizzbuzz(20);
```

### Object-Oriented Programming

```crisp
class Animal {
    fn new(name) {
        self.name = name;
    }
    
    fn speak() {
        say self.name + " makes a sound";
    }
}

class Dog extends Animal {
    fn speak() {
        say self.name + " barks!";
    }
}

let dog = Dog.new("Rex");
dog.speak();  # Rex barks!
```

### Functional Programming

```crisp
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

let evens = numbers
    |> filter { |n| n % 2 == 0 }
    |> map { |n| n * n };

say evens;  # [4, 16, 36, 64, 100]
```

### Quadratic Equation Solver

```crisp
# Quadratic Equation Solver
# Usage: crisp quadratic.csp

say "Enter coefficient a:";
let a = float(readline());

say "Enter coefficient b:";
let b = float(readline());

say "Enter coefficient c:";
let c = float(readline());

let d = pow(b, 2) - 4 * a * c;

if d > 0.0 {
    let x1 = (-b + sqrt(d)) / (2 * a);
    let x2 = (-b - sqrt(d)) / (2 * a);
    say "Roots: x1 = " + x1 + ", x2 = " + x2;
} else if d == 0.0 {
    let x = (-b) / (2 * a);
    say "Double root: x = " + x;
} else {
    let real = (-b) / (2 * a);
    let imag = sqrt(-d) / (2 * a);
    say "Complex roots: " + real + " ± " + imag + "i";
}
```

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Code Contributions

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Other Ways to Contribute

- **Report bugs** — Open an issue with a minimal reproduction
- **Suggest features** — Share your ideas in the discussion forum
- **Improve documentation** — Help us write better docs
- **Write examples** — Share your CRISP code snippets
- **Spread the word** — Star the repo and share with others

---

## 🧪 Testing

Run the test suite:

```bash
cargo test
```

Run specific tests:

```bash
cargo test --test integration
```

---

## 📄 License

CRISP is dual-licensed under:

- **Apache License, Version 2.0** ([LICENSE-APACHE](LICENSE-APACHE))
- **MIT License** ([LICENSE-MIT](LICENSE-MIT))

You may choose either license at your option.

---

## 💬 Community

- **GitHub Discussions** — [Join the conversation](https://github.com/CRISP-lang-foundation/CRISP-lang/discussions)
- **Issue Tracker** — [Report bugs](https://github.com/CRISP-lang-foundation/CRISP-lang/issues)
- **Documentation** — [ 🧰 WIP 🛠️]

---

## 🛠️ Development

### Prerequisites

- Rust 1.90 or later
- Cargo
- Git

### Build

```bash
git clone https://github.com/CRISP-lang-foundation/crisp.git
cd crisp
cargo build
```

### Run with debug

```bash
cargo run -- --debug
```

### Build for release

```bash
cargo build --release
```

---

## 📊 Project Status

| Version | Status | Notes |
|---------|--------|-------|
| v0.1.7 | ✅ Stable | Bug fixes, tests, minor changes |
| v0.1.8 | 🚀 In Progress | Feature enhancements |
| v1.0.0 | 📅 Planned | First stable release |

---

## 👥 Team

- **Peter Leukanič** — Founder & Lead Developer

---

## 🙏 Acknowledgments

- **The Rust Community** — For the amazing language and ecosystem
- **The Perl Community** — For the inspiration and expressiveness
- **The Emacs Community** — For the great tools and support

---

## 📌 Quick Links

- [GitHub Organization](https://github.com/CRISP-lang-foundation)
- [Main Repository](https://github.com/CRISP-lang-foundation/crisp)
- [Documentation](https://crisp-lang.org)
- [Issue Tracker](https://github.com/CRISP-lang-foundation/crisp/issues)
- [Discussions](https://github.com/CRISP-lang-foundation/crisp/discussions)

---

## 🌈 Why CRISP?

> *"Perl's expressiveness, Rust's safety."*

CRISP brings together the best of both worlds:

- **Expressiveness** — Write concise, readable code like in Perl
- **Safety** — Memory safety from Rust
- **Performance** — Native speed when you need it
- **Flexibility** — From quick scripts to large applications
- **Ecosystem** — Access to Rust's crates and Perl's CPAN

---

## Support

If you like CRISP, please consider:

- ⭐ **Starring** the repository
- 🐛 **Reporting** issues
- 📝 **Contributing** code or documentation
- 📢 **Spreading** the word

---

**Made with 🦀 by the CRISP Language Foundation**
