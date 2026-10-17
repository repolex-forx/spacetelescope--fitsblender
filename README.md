# Repolex Knowledge Graph of spacetelescope/fitsblender

RDF knowledge graph data for [spacetelescope/fitsblender](https://github.com/spacetelescope/fitsblender), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download spacetelescope/fitsblender
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 035429ac2c8422b4a6f4872dffc1e594d90d0af3
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 035429ac2c8422b4a6f4872dffc1e594d90d0af3
│           └── chunk-001.nq.gz
├── blob
│   ├── 018c263f4061165734e3c5d1eaa49295aa87edf2.nq.gz
│   ├── 0cee401886c9645d2596e7e66afec16eadc91ce3.nq.gz
│   ├── 0ed7527a20cd8a5ba3634dd31101fb5239ac0d74.nq.gz
│   ├── 17ca9ab5ce9c31a2d88bf24110bfccc4aabb9e03.nq.gz
│   ├── 1db95e274b03bcc70b2e93ef2e24f5cc98e722aa.nq.gz
│   ├── 316ea67d05cd25f5725805d4491a55f3379f2c31.nq.gz
│   ├── 359eb6c6309158c049ae07e5b5582a518c980250.nq.gz
│   ├── 360d02a64854ddecd0c618b82280a329c7511448.nq.gz
│   ├── 40a4b30c1947ec3b60957d05a94dc3b7b0248f60.nq.gz
│   ├── 4e26b50346ad1267fa05968ed0fb8aa9b9025610.nq.gz
│   ├── 5b71ce5b26ba1c82c855087811d7c3b0a8aec0ae.nq.gz
│   ├── 5ec6c1ccf89d82fb46802a339565121c4835ad7b.nq.gz
│   ├── 60557c24b07e0b47c20766a542a736712d037439.nq.gz
│   ├── 6174d723705b3848c6ec9dd499f15e08bdabc6ae.nq.gz
│   ├── 61b904c7a3c9237f58a1891387f89c571c36f1b4.nq.gz
│   ├── 6a4f5eea95db2c7d83456153baea28d8cd850da2.nq.gz
│   ├── 6f5a205a29a4c6787b737410c860c07d1cb3c713.nq.gz
│   ├── 75aaf88d96746be1c758b4374424822df971c807.nq.gz
│   ├── 76de2887f15cf01fa691ca0a80cc97401fe4777c.nq.gz
│   ├── 98a8c0f911c03aa8f302835691a00776a764c751.nq.gz
│   ├── a09751cbe457aaab6652f083e66a132d8d76d2a8.nq.gz
│   ├── a69ab3f1e50022c9495c613508192fdc20ba33ec.nq.gz
│   ├── a72a68c22233656566c0187a768fb4e90f473191.nq.gz
│   ├── b33d4ece6ab5b52caf670ae15cae68dbe39e2227.nq.gz
│   ├── bf8316c53f7b03523911c10cf2f21b0902f6ec0c.nq.gz
│   ├── c5bbc629233d939c6ecea3dc4c9ace9f1d83e5c6.nq.gz
│   ├── c6c31176572d88e90f3e5640ecff0f91ce1f6e98.nq.gz
│   ├── cc3fd84110fb10e0a0b4a6572fa60f0208a29b8e.nq.gz
│   ├── d0e4d9e5414ea2005c290ad8a90598c7376eedfa.nq.gz
│   ├── d628fafbb82d696b1daae84eaaf4d93093951aa0.nq.gz
│   ├── d8227035cef113b212a1fa650cf6ea2b3a5c9c76.nq.gz
│   ├── dee581cf5ec91e84971be233185e5e9f48b39fbd.nq.gz
│   ├── e04887d1f855d14e90290ea56063ae2b7c3407a4.nq.gz
│   ├── e23cfe1bf087a7bc65785a61d04d819538db9e21.nq.gz
│   ├── e349511851baf633a338d579034e63eba4e15ea6.nq.gz
│   ├── e34c37015a4023a60308c8a5da8b8f9e975055ee.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e8634a4344e7bf778a5757942e15bc61f4934116.nq.gz
│   ├── ebfc6acccab0d10ba8aed9bbd07cb38b0305c113.nq.gz
│   ├── f7360b4f2a32ec54aa82f285ae2da3a2d92633b8.nq.gz
│   └── f8967e68902ce39f1bf7c5c790cc0729d056a049.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 035429ac2c8422b4a6f4872dffc1e594d90d0af3.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[spacetelescope/fitsblender](https://github.com/spacetelescope/fitsblender)

---
*Parsed on 2026-10-17 by [repolex](https://repolex.ai)*
