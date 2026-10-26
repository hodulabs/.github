<p align="center">
  <img src="https://raw.githubusercontent.com/hodulabs/hodu/main/assets/hodu_mascot_with_ferris_transparent.png" alt="hodu" width="300">
</p>

<h1 align="center">hodu</h1>

<p align="center">
  A machine-learning framework on the kurumi engine: NumPy-ergonomic<br>
  tensors, a real <code>nn</code>, training, and a single-file <code>.hodu</code> deploy artifact. CPU and Metal.
</p>

```rust
use hodu::prelude::*;

let ctx = Ctx::cpu();                  // or Ctx::metal() on Apple Silicon
let lin = Linear::new(&ctx, 1, 1, 0);  // build the graph once, feed batches, step an optimizer, then:
save("model.hodu", &lin).unwrap();     // a self-describing, re-runnable artifact
```

## Repositories

- [**hodu**](https://github.com/hodulabs/hodu) - the ML framework: `nn`, `optim`, `loss`, `data`, `.hodu` artifacts
- [**kurumi**](https://github.com/hodulabs/kurumi) - the tensor + autograd engine (CPU & GPU) beneath hodu
- *coming soon:* **hodu-py** (hodu for Python) and **hodu-rok** (hodu for rok)

<p align="center"><sub>Built by <a href="https://daminstudio.com">DaminStudio</a></sub></p>
