---
title: Vision
description: >-
  Vision, non-goals, and principles for Commerce DevKit as an open tooling
  ecosystem for SAP Commerce development.
keywords:
  - Commerce DevKit vision
  - SAP Commerce tooling
  - SAP Commerce developer experience
  - LSP
  - Tree-sitter
  - editor agnostic tools
draft: false
---

# Vision

Commerce DevKit is a modern, open tooling ecosystem for SAP Commerce
development.

Our goal is to provide fast, composable, and editor-agnostic tooling built
around open standards such as LSP and Tree-sitter. We believe SAP Commerce
development should integrate naturally with modern developer workflows instead
of depending on a single IDE or monolithic toolchain.

Commerce DevKit focuses on developer experience: fast navigation, intelligent
completion, diagnostics, project indexing, and support for SAP Commerce
specific languages such as Impex and FlexibleSearch. The project is designed as
a collection of small, reusable components - CLI tools, language servers,
parsers, and editor integrations - that work together while remaining
independently usable.

We aim to build upon existing ecosystems rather than replace them. Commerce
DevKit integrates with established tools such as Java language servers, modern
editors, and developer workflows instead of reinventing them.

# Non-goals

Commerce DevKit is not intended to be a full IDE, nor a clone of existing SAP
Commerce IntelliJ tooling. The project does not aim for feature parity with any
single editor or proprietary plugin. Instead, it focuses on providing an open
and extensible foundation that can support multiple editors and workflows.

The project also does not attempt to replace SAP Commerce platform internals or
build a monolithic "all-in-one" application. Simplicity, interoperability, and
long-term maintainability take priority over excessive abstraction or tightly
coupled tooling.

# Principles

- Open and editor-agnostic
- Fast and lightweight
- Composable instead of monolithic
- Built for contributors and extensibility
- Pragmatic over perfect
