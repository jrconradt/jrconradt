### J.R. Conradt

.NET engineer. I move decisions from runtime to compile time, and make the secure path the only one that compiles.

One throughline across five projects: source generators, closed-set dispatch, and typed contracts turn what would be runtime failures into build errors.

| Repo | What it demonstrates |
|------|----------------------|
| **[Atelier](https://github.com/jrconradt/Atelier)** | Compile-time DI and product composition via Roslyn generators; `Outcome<T>` contracts in place of exceptions. |
| **[Vice](https://github.com/jrconradt/Vice)** | CLI framework whose natural-language command grammar is wired by source generators and piped through backpressured channels. Outbound connections pass an IP/host allow-deny policy; downloads are confined to canonicalized allow-listed write roots. |
| **[Templar.Net](https://github.com/jrconradt/Templar.Net)** | Indentation-aware C# code-generation engine — multi-line values inherit the placeholder's column; trim/AOT-safe. |
| **[FWHT.Net](https://github.com/jrconradt/FWHT.Net)** | A 9-stage GF(2) Walsh–Hadamard butterfly in one AVX-512 register: ~13 ns per 64-byte window per worker; saturates two-socket DRAM bandwidth (~105 GB/s read+write combined). |
| **[LinearPipe.Net](https://github.com/jrconradt/LinearPipe.Net)** | Wait-free, memory-mapped data-plane pipeline — workers never share a chunk; per-chunk SIMD transform, non-temporal stores. |

All Apache-2.0, .NET 10.

---

**Contact:** [jeff.r.conradt@gmail.com](mailto:jeff.r.conradt@gmail.com)
