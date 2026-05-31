---
title: Roadmap
description: >-
  The Commerce DevKit roadmap organized around capabilities and maturity
  milestones for the SAP Commerce open tooling ecosystem.
keywords:
  - Commerce DevKit roadmap
  - SAP Commerce tooling roadmap
  - LSP
  - Tree-sitter
  - project indexer
  - Impex parser
  - FlexibleSearch parser
draft: false
---

# Roadmap

Progress is tracked in capability stages rather than version numbers.
Commerce DevKit is an ecosystem, and each stage unlocks the next.

{{< roadmap-stages >}}

---

## Stage 1: Foundation

The first objective is not editor support. It is creating a shared
understanding of a SAP Commerce workspace.

A **project scanner** discovers extensions, configuration locations,
`items.xml` files, Spring XML definitions, and project boundaries. It becomes
the foundation for every subsequent component. The most important deliverable
of this stage is the definition of the **Commerce DevKit project model**: a
machine-readable index that other tools consume.

A project can be scanned from the command line. Extension relationships are
discovered automatically. Item types are indexed, and the index format is
documented and stable.

---

## Stage 2: Language Foundations

With project information available, the focus shifts to understanding
SAP Commerce-specific languages. The priority is **parsing before intelligence**.

The first parsers target **Impex** and **FlexibleSearch** because they are
widely used and currently underserved outside IntelliJ. Commerce DevKit
establishes Tree-sitter grammars and begins defining language semantics.
Community members can contribute grammar improvements independently of
any editor integration.

By the end of this stage, Commerce DevKit becomes the canonical open-source
parser ecosystem for SAP Commerce languages.

---

## Stage 3: Developer Tooling

With project indexing and language parsing in place, the ecosystem begins
delivering **practical developer value**: navigation, search, and workspace
exploration.

Editor integrations start with **Neovim**, the primary environment of the
founding team. Developers can navigate from an item type to its declaration,
search extensions with workspace awareness, and author Impex with project
context. Commerce DevKit becomes useful at this point even without a language
server.

---

## Stage 4: Language Server

The long-term goal is a language server that serves multiple editors.
By this stage the project already has the two things most language servers
struggle to build: workspace understanding and language parsing. The server
therefore focuses on **intelligence rather than discovery**.

Completion draws from the indexed project model. Navigation works across
Java, XML, Impex, and FlexibleSearch. Workspace diagnostics, reference
discovery, and semantic understanding of SAP Commerce concepts are all within
reach. The language server becomes the central integration point for editor
support.

---

## Stage 5: Ecosystem Expansion

Once the language server exists, the focus becomes **adoption over features**.
Editor integrations, documentation, APIs, and community contributions take
centre stage.

Potential targets include Visual Studio Code, Helix, Zed, Eclipse, and
JetBrains. At this point Commerce DevKit transitions from a project into
a platform.

---

## Documentation Track

This track runs in parallel from day one and continues indefinitely.

SAP Commerce knowledge is often trapped inside consulting organisations and
internal wikis. Commerce DevKit has an opportunity to become a neutral,
practical knowledge base for tooling, architecture, and development practices —
documenting the **practical reality** of SAP Commerce development rather than
competing with official SAP documentation.
