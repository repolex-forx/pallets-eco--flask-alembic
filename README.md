# Repolex Knowledge Graph of pallets-eco/flask-alembic

RDF knowledge graph data for [pallets-eco/flask-alembic](https://github.com/pallets-eco/flask-alembic), parsed by [repolex](https://repolex.ai).

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
rlex download pallets-eco/flask-alembic
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 9425c61473ab4700706f13344217d6b605079371
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 9425c61473ab4700706f13344217d6b605079371
│           └── chunk-001.nq.gz
├── blob
│   ├── 04bbe92d12e0e9c17a87d93624e8fc2a2f4c3b6c.nq.gz
│   ├── 077803de32e30b781a49c81ddd7fff6e3385919d.nq.gz
│   ├── 0aa45abbebb2dfd729073cb47922f95e83c378a2.nq.gz
│   ├── 0d64bdfc5ae690459b6c50c6051cd15e86023d5d.nq.gz
│   ├── 0f433a047c73565c67a1eb48cb93c3879215e9a4.nq.gz
│   ├── 11016301e749297acb67822efc7974ee53c905c6.nq.gz
│   ├── 13369dcadf9cdafbe7b3661832d69ddfeed7c880.nq.gz
│   ├── 1aa2c55c4f0f61e80696dbbd61752cafb5d294a6.nq.gz
│   ├── 229c594159ff374818696eb770cb473773a27ac8.nq.gz
│   ├── 235df6aaea34e53851e62356d0a5aa7bfe42d8c5.nq.gz
│   ├── 2a9dc4d1c1eb778753b99dffd50d280d45e2f6d6.nq.gz
│   ├── 2ed26e17040006b09f57f2d85b769b37bbe16484.nq.gz
│   ├── 2fa197d7c56c2461cfff4ab7252fd54e76465c5f.nq.gz
│   ├── 2ff985a67af35fdfd1076354b771c425867cdab4.nq.gz
│   ├── 3132644c295a8b05b077dbfb8e1afc4ad0bffe0f.nq.gz
│   ├── 34d5309fd8485516165411dcb51480d333367358.nq.gz
│   ├── 35e705c5abf566a1ae72137eeb3fab13e89629b3.nq.gz
│   ├── 4a19af4b55ef8d3f2b0e2afdd9b936b9e720e2a7.nq.gz
│   ├── 5149e064dce29fbb0fd92773a95ee676196971d9.nq.gz
│   ├── 581db67248e51429531ad354337ab07691f007e1.nq.gz
│   ├── 58d8f3f0ee4d843304c3c465ec0996736f1b7ac1.nq.gz
│   ├── 5900647675ce4ae471749587a4e083faa87c6a7b.nq.gz
│   ├── 5eb4a7b61d4aec9ef4389e9fafb6895b07563a8b.nq.gz
│   ├── 5f522c22204b689033f69e581c007bc1e1d73774.nq.gz
│   ├── 62b0f50ef5d1d1bfceae2f89ab87a5a9918ab507.nq.gz
│   ├── 759c637448dccfad470b215ea589d899ed4c35de.nq.gz
│   ├── 7e798ab4ac2d386a0133e8667d3eaec622ae0c40.nq.gz
│   ├── 7e93e4cef3e2f76917c71ebdebbc3d45c261ebf6.nq.gz
│   ├── 8441e5a64f3bdd680c9d67e8b44c9f176d2a351b.nq.gz
│   ├── 86241c2921cdcf9f2903e4c2628a4a2af89ba7bf.nq.gz
│   ├── 90d1b9710295b4cb3c612049b660a487e7b3d3ba.nq.gz
│   ├── 9840cb60b1325b955c63550a3bf937f31213ead4.nq.gz
│   ├── 98f0144519ad98171340420bbe55125f0b68b400.nq.gz
│   ├── a0008f5633f562e34a91bf16c8d6b46c920a0d75.nq.gz
│   ├── a5bdafdc3bb27568009f0fed88223cc2593fa09d.nq.gz
│   ├── acbd83f90b38e208b211fc7e62366556e9565dd8.nq.gz
│   ├── b2a25e747bc319277ad4bcd1470b72a554180d01.nq.gz
│   ├── e51a771b565c4d06c29b50d7e1c1333df8d58521.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── ed3b02ed3b2b3f320252223e1b26adcd9e310e22.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 9425c61473ab4700706f13344217d6b605079371.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
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

[pallets-eco/flask-alembic](https://github.com/pallets-eco/flask-alembic)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
