# Repolex Knowledge Graph of asimov-modules/asimov-signal-module

RDF knowledge graph data for [asimov-modules/asimov-signal-module](https://github.com/asimov-modules/asimov-signal-module), parsed by [repolex](https://repolex.ai).

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
rlex download asimov-modules/asimov-signal-module
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 582bbdf2edaefbc65944cbd7a90c0a4843ffa267
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 582bbdf2edaefbc65944cbd7a90c0a4843ffa267.nq.gz
│   └── repolex
│       └── 582bbdf2edaefbc65944cbd7a90c0a4843ffa267
│           └── chunk-001.nq.gz
├── blob
│   ├── 10b359dd05935c73efb064470f9ecda90f6d28aa.nq.gz
│   ├── 110d24d3a6793f6646c8791d838e69e8be32ff19.nq.gz
│   ├── 27937c34773b555ff7e15dc3f37ebeb2f687ab33.nq.gz
│   ├── 36b1e9eb8b1994248b6803bf0ff4b0ed9dd18c03.nq.gz
│   ├── 44a3f23bb2df1a7e00d9828dc31c9d3cca7567ec.nq.gz
│   ├── 5182ce0f221c09b03a5551454dac26fb13dbd2e1.nq.gz
│   ├── 580e027776ce95da32528f7ea960e88f38a5049b.nq.gz
│   ├── 5892f46b76031ab3cd9a239f02022b3f656c1776.nq.gz
│   ├── 5d4986990a704e67fd69541d1c39ce06e482587d.nq.gz
│   ├── 6b23d61018f43b840f8d2ff3b45a1c02d76df38d.nq.gz
│   ├── 75e3b65f99b29f48ab230e3eab3de8d0b7a9229f.nq.gz
│   ├── 78dd0a11ea597b717029092100fabf3132e38abb.nq.gz
│   ├── 792897719b12c36c0189953c176d9ef48f168d36.nq.gz
│   ├── 7ba0575fa18171914e71f5d58acead4926d1d7a8.nq.gz
│   ├── 7ba38f0a55e4fac446e05a9f2b719b9a4c73957a.nq.gz
│   ├── 7f3013e839cfcb4dc28385ceb4fe96bb15836067.nq.gz
│   ├── 8230fb79ff9d4908a86f95f458bd0794bd01df6f.nq.gz
│   ├── 8e80cfdb29a54d8ade640a6881643eb85d75004b.nq.gz
│   ├── 9ccbd756499016f25b180d565aeb7baf5dce23dc.nq.gz
│   ├── 9fe50de16e59d550235aa6d7d15ee12ddf054414.nq.gz
│   ├── a03275dd8821c43188c5ae3e934f90d00bebf31f.nq.gz
│   ├── ab83f73439a15541c783550d0a7063429e9c942e.nq.gz
│   ├── ade11fec0dd09ad519720fd3698460406406d17e.nq.gz
│   ├── af9908b08f4b33c32a0080af73f53bc0fa0cdce4.nq.gz
│   ├── ba28989df42ec618e57d56f8ea366b62b3027ff4.nq.gz
│   ├── bcab45af15a0f1b0166daf8cbf18b17cd8649277.nq.gz
│   ├── c60852d73b2ba161cdb27fad2f9b36b0e4fa034d.nq.gz
│   ├── cf42f6893594e2f8be2b722de51123d65e4d61c4.nq.gz
│   ├── e3e57a8ce4ccbf74759a6df8fa4a3980ff1c9209.nq.gz
│   ├── e432408314122661846779cba2076f6440b85f35.nq.gz
│   ├── ee4d9362508d63f9e156fe9ee1b11ebc1a3e86d6.nq.gz
│   └── efb98088164f5786b17e83ed384971fc3c74f93c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 582bbdf2edaefbc65944cbd7a90c0a4843ffa267.nq.gz
├── filetree
│   └── 582bbdf2edaefbc65944cbd7a90c0a4843ffa267.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 41 files
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

[asimov-modules/asimov-signal-module](https://github.com/asimov-modules/asimov-signal-module)

---
*Parsed on 2026-09-28 by [repolex](https://repolex.ai)*
