### 1. Prerequisites

Ensure you have the **Rust toolchain** installed. If not, get it at [rustup.rs](https://rustup.rs/).
For example for Linux,
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Then, install `maturin`:

```bash
pip install maturin

```

### 2. Clone and Build

Run the following commands to clone the repository and install the patched version directly into your current Python environment:

```bash
# Clone the repository
git clone https://github.com/MENOENGLISH/tokenizers.git
cd tokenizers/bindings/python

# Compile and install (overwrites the existing tokenizers package)
maturin develop --release

```

### 3. Verification

Verify that the installation was successful and points to your local build:

```python
import tokenizers
print(f"Location: {tokenizers.__file__}")

```


---

Would you like me to add a **Troubleshooting** section for common Rust compilation errors?
