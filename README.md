# From Power Set to Boolean Lattice

An interactive visualization for **Discrete Mathematics & Graph Theory** that shows how the power set of a set becomes a Boolean lattice (a poset under subset inclusion).
Click For Visualization (https://surajit-sahoo-iitian.github.io/Boolean-Lattice/)
## What students can explore

Choose \(B_1\), \(B_2\), \(B_3\), or \(B_4\) and move through the construction step by step:

1. Start with the set \([n]\).
2. Generate the power set \(2^{[n]}\).
3. Arrange subsets by their cardinality.
4. Build the **complete relation** \(A\subseteq B\), layer by layer.
5. Remove self-loops.
6. Remove transitive relations.
7. Obtain the Hasse diagram.
8. Explore least, greatest, minimal, maximal, comparable, and incomparable elements.

### Important pedagogical feature

During the relation-building stage, the visualization intentionally keeps **all** subset relations, including:

- self-loops \(A\subseteq A\), and
- transitive relations such as \(A\subseteq B\subseteq C\).

Only after all layers have been constructed are the self-loops and transitive relations removed to obtain the Hasse diagram.

## GitHub Pages

This repository is designed to run as a static GitHub Pages site. No external JavaScript libraries are required.

After enabling GitHub Pages with **GitHub Actions** as the source, the workflow in `.github/workflows/pages.yml` deploys `index.html` automatically.

## Repository structure

```text
.
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── pages.yml
