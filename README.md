# Luma Packet Manager (LPM)

**LPM** (Luma Packet Manager) is the unified package and project management tool for the **Luma Language Ecosystem**, including:

- [Luma](https://luma-lang.org) – A modern systems programming language inspired by Rust and Python  
- **Lumo** – A lightweight scripting companion to Luma  
- **Wave** – A WebAssembly-oriented language for safe, portable modules  

LPM handles everything from dependency resolution, building, running, formatting, and eventually publishing Luma ecosystem packages.

---

## ✨ Features

- 🔧 `init` – Create a new project with a unified `Luma.toml`
- 📦 `install` – Manage dependencies for Luma, Lumo, and Wave
- ▶️ `run` – Automatically detect and execute `.lu`, `.luo`, or `.wv` files
- 🛠️ `build` – Compile Luma or Wave projects
- 🧪 `test` – Run test suites (coming soon)
- 🎨 `fmt` – Format source code (planned)
- 🚀 `publish` – Publish your package to the future Luma registry

---

## 📂 Example Project Structure

```

my-project/
├── src/
│   └── main.lu        # Luma source file
├── scripts/
│   └── setup.luo      # Lumo script
├── wasm/
│   └── frontend.wv    # Wave module (compiled to WASM)
├── Luma.toml          # Unified manifest
└── trial.lock         # Dependency lock file

````

---

## 🚀 Getting Started

### Install LPM (coming soon)

```bash
cargo install lpm
````

### Create a new project

```bash
lpm init my-app --lang luma
cd my-app
lpm run
```

### Add dependencies

```bash
lpm add wave-ui
lpm install
```

---

## 📖 Manifest Format: `Luma.toml`

```toml
[package]
name = "my-app"
version = "0.1.0"
language = "luma"

[dependencies]
lumo-utils = "0.1"
wave-ui = { git = "https://github.com/usr/wave-ui" }

[build]
target = "native"

[scripts]
setup = "scripts/setup.luo"
```

---

## 🛤 Roadmap

* [x] Project initialization (`lpm init`)
* [x] Unified runner (`lpm run`)
* [ ] Package registry support
* [ ] Plugin system for extensions
* [ ] REPL / Playground integration
* [ ] Testing & coverage tools
* [ ] LSP / editor toolchain integration

---

## 🧑‍💻 About

LPM is part of the **Luma Language Ecosystem**, a personal and open-source initiative to explore new frontiers in language design and software tooling.

Follow progress and contribute via:

* GitHub: [Liam Von Astoria](https://github.com/liamvnastoria)
* Website: [luma-lang.org](https://luma-lang.org)

---

## License

MIT © \[Liam Von Astoria] — Open for contribution.
