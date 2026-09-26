# MatryGram

MatryGram is a visual notation for representing nested algorithmic structures as spatial hierarchies.

The name comes from Matryoshka dolls, reflecting the way multiple structures can be nested within one another.

## Overview

Flowcharts are well suited for understanding the overall flow of a program. However, when a flowchart is used to represent detailed algorithms with deeply nested conditionals and loops, the result can be hard to follow.

MatryGram was created to fill this gap. It represents containment relationships between structures such as conditionals and loops as spatial hierarchies, making it possible to visualize the internal structure of a function or algorithm.

MatryGram is not intended to replace flowcharts. Instead, we recommend using the two together: use flowcharts for large-scale structures such as the overall execution flow of a program, and use MatryGram for detailed structures within functions or algorithms.

When too much of a program is represented in a single MatryGram, the diagram can quickly become cluttered and hard to read. We therefore recommend dividing a program into smaller units, such as individual functions, rather than representing it as one large MatryGram.

## Core Concept

MatryGram represents nested program structures through spatial containment.

When code is contained within a conditional or loop, the corresponding element is placed inside its parent structure in the diagram. The core idea is to convey nesting through visual hierarchy rather than relying primarily on arrows that show execution flow.

## Design Method — Inside-Out Design

When creating a MatryGram, you can start with the smallest operation.

First, define the core operation to be performed. Then, as needed, add conditionals or loops around it to gradually build up a larger structure.

```text
Small operation → Condition → Loop → Larger structure
```

Rather than defining the entire control structure up front and filling it in afterward, this approach lets you keep existing operations intact while adding control structures incrementally.

## Implementation Method — Outside-In Implementation

When translating a MatryGram into code, read it in the opposite direction.

Working from the outermost layer inward naturally mirrors the nesting of the resulting code.

```text
Larger structure → Loop → Condition → Small operation
```

In this way, you can read a MatryGram in different directions depending on whether you are using it for design or implementation.

## Specification

The symbols, layout rules, and syntax of MatryGram are maintained separately in the Specification.

The syntax may change as the project evolves. For the exact notation rules of a given version, refer to that version's Specification.

[View Specification](./specification/)

## Examples

Examples of algorithms represented in MatryGram, along with their corresponding code, are available in the Examples directory.

[View Examples](./examples/)

## Project Status

MatryGram is in the early stages of development.

Its syntax, symbols, and detailed rules may change as development continues. The current priority is to develop a notation that makes basic algorithms easy to write and read.

## License

Unless otherwise specified, the documentation, examples, images, and other creative works provided by the MatryGram project are licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

No attribution is required when you use the MatryGram notation to create your own diagrams. You may freely use the notation for personal, educational, research, and commercial purposes.

The MatryGram project does not own, and claims no rights over, diagrams created with the MatryGram notation or programs based on such diagrams.

---

This project is under active development and will continue to evolve through feedback and experimentation.
