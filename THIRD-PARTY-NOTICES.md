# Third-party notices — PIN MINER

PIN MINER is distributed as a compiled binary that includes the third-party
components listed below. Each remains under its own license; those licenses —
not the PIN MINER license — govern your rights in these components. The
PIN MINER license (see `LICENSE`) covers only PIN MINER's own code.

This file lists the significant components and reproduces the required notices.
The authoritative, complete list for a given build (including all transitive
Rust dependencies) can be regenerated on the build machine — see "Regenerating
this list" at the end.

---

## Pearl (zk-pow, pearl-blake3) — ISC License

Copyright (c) 2025-2026 Pearl Research Labs
Copyright (c) 2015-2016 The Decred developers

Permission to use, copy, modify, and distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

---

## Plonky2 (via zk-pow) — MIT OR Apache-2.0

Copyright (c) 2022-2025 The Plonky2 Authors
Copyright (c) 2025-2026 Pearl Research Labs

Licensed under either the MIT license or the Apache License, Version 2.0, at
your option. Full texts: https://opensource.org/license/mit and
https://www.apache.org/licenses/LICENSE-2.0

---

## Rust crates — MIT / Apache-2.0 / CC0 (permissive)

The binary links the following Rust crates and their transitive dependencies,
each under a permissive license (MIT, Apache-2.0, or CC0-1.0, individually or
dual-licensed). © their respective authors:

  blake3, rayon, anyhow, hex, primitive-types, bincode, serde_json, base64,
  flate2

MIT license text: https://opensource.org/license/mit
Apache-2.0 license text: https://www.apache.org/licenses/LICENSE-2.0
CC0-1.0: https://creativecommons.org/publicdomain/zero/1.0/

(See "Regenerating this list" for the exact per-crate licenses and copyright
lines of the specific versions in a build.)

---

## NVIDIA CUDA Runtime — NVIDIA CUDA EULA

The binary statically links the NVIDIA CUDA runtime (cudart). It is
redistributed under, and its use is governed by, the NVIDIA CUDA Toolkit
End User License Agreement: https://docs.nvidia.com/cuda/eula/

---

## Regenerating this list (build machine)

For a complete, authoritative list of every Rust dependency and its exact
license in a given build, run in the source tree:

    cargo install cargo-about
    cargo about generate about.hbs > THIRD-PARTY-NOTICES.md

or, for a quick table:

    cargo install cargo-license
    cargo license
