# Repolex Knowledge Graph of eyre-rs/eyre

RDF knowledge graph data for [eyre-rs/eyre](https://github.com/eyre-rs/eyre), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download eyre-rs/eyre
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 32d84dcbacf607d7c6e1050b54d585622c8de4fc
│   │   │   └── chunk-001.nq.gz
│   │   └── b6075394bcaaa8cc311321239f8964099bb02a88
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 32d84dcbacf607d7c6e1050b54d585622c8de4fc.nq.gz
│   │   └── b6075394bcaaa8cc311321239f8964099bb02a88.nq.gz
│   └── repolex
│       ├── 32d84dcbacf607d7c6e1050b54d585622c8de4fc
│       │   └── chunk-001.nq.gz
│       └── b6075394bcaaa8cc311321239f8964099bb02a88
│           └── chunk-001.nq.gz
├── blob
│   ├── 0309398080f053c957ff45676ee1a62f8ecaa809.nq.gz
│   ├── 032f82a24de2bf3998e48bc62cf7d84de6ac3583.nq.gz
│   ├── 0515a7a8d7ccb3c527459ee69f097f866a0d7374.nq.gz
│   ├── 06ec8058c503c26645ef52b69f37df7298564adf.nq.gz
│   ├── 08ae50459cdb0749661095ea7423b1b3a7a97c9d.nq.gz
│   ├── 08c08156e36085e88362facd72fa0daed289d05f.nq.gz
│   ├── 0ad71af801bda8849202555b24af022c1dbbbe3d.nq.gz
│   ├── 11556f27042abc91d7c402af62aef49ba3091fef.nq.gz
│   ├── 1279de7af8ec8f5657f0ecee9218d3f87845b00b.nq.gz
│   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│   ├── 1d3bcb0f6f37a7f636f97fb0db100aa61ef02c7a.nq.gz
│   ├── 20bdbfae9d26716850728f3bbc9f9fa0fe3bbacc.nq.gz
│   ├── 214799b1faa473b729c624c2f543dc08808ee88d.nq.gz
│   ├── 21cca48bd655faf402e943b8dd84c6c0b125c680.nq.gz
│   ├── 292c93cc78b1621c022603dcb4cb0504bf334531.nq.gz
│   ├── 2f24d636bee13f18656a5854b0881c5ba7f5a709.nq.gz
│   ├── 2f58c6bc07f588c8ce8c68846d3e243ba9f395fa.nq.gz
│   ├── 31aa79387f27e730e33d871925e152e35e428031.nq.gz
│   ├── 32d46ee883b58d6a383eed06eb98f33aa6530ded.nq.gz
│   ├── 3d118e51ef6791fc688b8b96eedf60e3ed4318c9.nq.gz
│   ├── 3d69c04179c3ba5804a4bf2e9b2ff81524abde53.nq.gz
│   ├── 41d3ddbb480c8460b0b861d9a3fa2273f35acab0.nq.gz
│   ├── 489da117473aa044c5d7b18eacab696d9acf1dc6.nq.gz
│   ├── 54e3da49c5eeede7490b1cbb464ae970f00ed469.nq.gz
│   ├── 56e80be142f5fb9b38503d6f32f4cad615bc3f31.nq.gz
│   ├── 58737fe1ac0d5aa878d5235d6b131e88ae1b6750.nq.gz
│   ├── 5c8d815a332b1cf779839ba105bdb1a9ceb9f57f.nq.gz
│   ├── 60371ab919c7a47ee0e350ca3bd48bdf64b3e6d5.nq.gz
│   ├── 6465433129c15c9874ee9108fad2d2ea93580930.nq.gz
│   ├── 66683b90ef68a8da52782491250f7a5a920c0e23.nq.gz
│   ├── 6c00d7fab69dc94429482f4cb84a4351634850f3.nq.gz
│   ├── 6f699243a5b0557d70ca7c1a43f77da4b4dc8844.nq.gz
│   ├── 701a0fd86146ca0a7fe2b39488f463191cdd3a9c.nq.gz
│   ├── 709955c62525fde8023ea4cb8229cfe9fca25696.nq.gz
│   ├── 751767dcf13280498af7683c66dc062fe92b3b27.nq.gz
│   ├── 76219eb72e8524f15c21ec93b9b2592da49b5460.nq.gz
│   ├── 77b8743623e66a3eaac5d814644a22c9c4bf1ae7.nq.gz
│   ├── 77e7811df922521519d2ee669dfca57f438a87d1.nq.gz
│   ├── 78131f2ec6e9f3fe066a15541ff04ff6d3a70285.nq.gz
│   ├── 792a64628f6c68132e20826e5ac765c70f7d9111.nq.gz
│   ├── 7974a6249e43040f8ac079e1f0c7ba3abb61329f.nq.gz
│   ├── 7c9349ab400f43e6e30868ee86d80813ec718675.nq.gz
│   ├── 7d3dfd669703c7eba6cc175437bedb3fb914cc56.nq.gz
│   ├── 7f4594bb47c827b9048d16fe6cd67f3a2bff9c25.nq.gz
│   ├── 8b0484d036a2380bbf01b9ac1bc3412ae430a567.nq.gz
│   ├── 8fd54b9b9def46087108aa7db1ef8ce8f71f6b7a.nq.gz
│   ├── 913649e7b453946acf841f53b4681286869f5add.nq.gz
│   ├── 965b606f331b51d566b46025f9ff311a7aad0c12.nq.gz
│   ├── 96d88303d76de1a4885e5e9f70af550b344c788c.nq.gz
│   ├── 96ef6c0b944e24fc22f51f18136cd62ffd5b0b8f.nq.gz
│   ├── 9a75a2362c9e9d456065ea205af3a59fc358d239.nq.gz
│   ├── a15b41ba89ec9bd4049b8366656bbbdc355ae387.nq.gz
│   ├── a6f0ab206b11c9c8336d03c4c79429601967e701.nq.gz
│   ├── aae2878cc6743492f86e97ecd8f047f5dffc4147.nq.gz
│   ├── abcc3c96db1d6ac4fb0d0e87e21cd11222c12ef6.nq.gz
│   ├── b4da68abe9a2fdcf97b632b4d9d27ff3a519eb9d.nq.gz
│   ├── b4e97a3efa6eb41bc2c40a5d7624ad52de0360ae.nq.gz
│   ├── b70b6a54634a68d65b442346e9118db1beb89cbc.nq.gz
│   ├── bb7c5c0be8aa34b9a1225a4ea43982f0458cf632.nq.gz
│   ├── c0d69191db5489013231e2bef436a1b3639fc3a8.nq.gz
│   ├── c66620e243d519ceabfa2121cd94cf7c8953ab99.nq.gz
│   ├── c9d71444794a3086f38e222423a0fd5c85f0d57d.nq.gz
│   ├── d31756e1c52ff010ad43f362a3a700d09ec339e4.nq.gz
│   ├── d6187448d8caf23a5e83497f1ce78bfc41aecd23.nq.gz
│   ├── d851f5ac7b4d12f2dee599e966a41c9a641889fc.nq.gz
│   ├── df33536bda45a60c3f351297d49d5a7ba1d86ff7.nq.gz
│   ├── df536c5b89a3f1d60ec2ffd1b19d5da3ba6b927e.nq.gz
│   ├── e0b2d292e78ebe9f9c3c44acac0def8c94bbb1c0.nq.gz
│   ├── e7251c263a2089b4de18d0b8735a22d7a2ca4081.nq.gz
│   ├── e7f58c1ba1e08b31ae42fd7e121e6be1f365b8f8.nq.gz
│   ├── eaa1e84ba289871d62bec8c0152fbe922804f6a0.nq.gz
│   ├── f0334e5cf6efea6a606dcf75b1705d466f26f396.nq.gz
│   ├── f9aea23b5154721f04537b60075baf789f06e6ba.nq.gz
│   └── fef121fbf8369a87d8bd6a45f0774fce8e5571f7.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 32d84dcbacf607d7c6e1050b54d585622c8de4fc.nq.gz
│   └── b6075394bcaaa8cc311321239f8964099bb02a88.nq.gz
├── filetree
│   ├── 32d84dcbacf607d7c6e1050b54d585622c8de4fc.nq.gz
│   └── b6075394bcaaa8cc311321239f8964099bb02a88.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

17 directories, 89 files
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

## Source repository

[eyre-rs/eyre](https://github.com/eyre-rs/eyre)

---
*Parsed on 2026-05-09 by [repolex](https://repolex.ai)*
