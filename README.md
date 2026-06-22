### J.R. Conradt

Systems and compiler-adjacent engineering in .NET. I move decisions from runtime to compile time — and make the secure path the only one that compiles.

The throughline across these projects: behavior usually deferred to runtime — dependency wiring, command dispatch, indentation, store ordering — is settled *before* the program runs, by Roslyn source generators, closed-set dispatch, and typed contracts. A mistake that can be a build error has no business being a production incident.

#### Selected work

| Repo | What it demonstrates |
|------|----------------------|
| **[Atelier](https://github.com/jrconradt/Atelier)** | .NET 10 orchestration framework. Source generators wire dependency injection and product composition at compile time instead of a runtime container; `Outcome<T>` result contracts flow through messaging, events, and state machines in place of exceptions. |
| **[Vice](https://github.com/jrconradt/Vice)** | A .NET CLI framework with a natural-language command grammar. Command packs are discovered and wired by source generators, then piped into one another through backpressured streaming channels. |
| **[Templar.Net](https://github.com/jrconradt/Templar.Net)** | Indentation-aware template engine for C# codegen — multi-line values inherit the placeholder's column. Trim/AOT-safe, zero dependencies. |
| **[FWHT.Net](https://github.com/jrconradt/FWHT.Net)** | A 9-stage GF(2) Walsh–Hadamard butterfly in a single AVX-512 register — no loops, no memory between stages. ~13 ns per 64-byte window; ~105 GB/s streamed across two NUMA sockets. |
| **[LinearPipe.Net](https://github.com/jrconradt/LinearPipe.Net)** | A memory-mapped, chunk-disjoint data-plane pipeline. Wait-free by construction — workers never share a chunk — with a per-chunk SIMD transform behind an unmanaged function pointer and non-temporal stores. |

All Apache-2.0, all targeting .NET 10.
