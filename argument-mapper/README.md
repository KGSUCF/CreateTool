# Argument Mapper

Argument Mapper is a low-code scholarly visualization tool that helps users turn structured argumentative writing into a polished visual map. Instead of writing JavaScript, users write a simple text-based syntax describing claims, evidence, counterclaims, rebuttals, and relationships. The tool then renders that input as a presentation-ready argument diagram.

This project was created as a prototype for a course exercise focused on designing new low-code/no-code tools.

## What the tool does

Argument Mapper lets users:

- write argument structures in a simple custom syntax
- render those structures as styled visual maps
- compare debate-style and scholarly layouts
- visualize relationships such as support, challenge, rebuttal, extension, and context
- use strength values to visually emphasize stronger claims
- load sample examples for demonstration and testing
- access a built-in syntax help guide

The goal is to bridge the gap between scholarly thinking and code-based visual expression.

## Why this tool exists

Many scholars, students, and writers can describe complex relationships between ideas, but they may not know how to translate those structures into visual, interactive, or presentation-ready formats using code.

Argument Mapper addresses that problem by providing:

- **constraints**, through a simple structured language
- **freedom**, through editable content and multiple argument forms
- **visual expression**, without requiring programming knowledge

## Features

- Structured input through a textarea
- Sample presets:
  - Voting Example
  - AI Education Example
  - Inflation Example
  - Write Your Own Map
- Styled argument nodes
- Strength-based visual emphasis
- Color- and pattern-coded connectors
- Relationship legend
- Syntax Help modal
- Browser-based interface with no external libraries required

## Syntax overview

The tool uses three main parts:

### 1. Top-level metadata

```text
TITLE: Main title
SUBTITLE: Optional subtitle
THEME: scholarly | dramatic
LAYOUT: debate | cascade
PALETTE: descriptive palette label
BACKGROUND: paper | dark
EMPHASIS: strength
### 2. Node blocks


NODE: P1
SIDE: PRO
TYPE: CLAIM
LABEL: Stronger democracy
TEXT: Mandatory voting strengthens representative democracy.
STRENGTH: 5

### 3. Link blocks
LINK:
FROM: P2
TO: P1
RELATION: supports

Supported values

SIDE
PRO
CON
NEUTRAL
TYPE
CLAIM
EVIDENCE
COUNTERCLAIM
REBUTTAL
CONTEXT
QUESTION
RELATION
supports
challenges
rebuts
extends
contextualizes
STRENGTH
integer from 1 to 5
Example input

TITLE: Should Voting Be Mandatory?
SUBTITLE: Participation vs. personal liberty
THEME: scholarly
LAYOUT: debate
PALETTE: plum-gold-slate
BACKGROUND: paper
EMPHASIS: strength

NODE: P1
SIDE: PRO
TYPE: CLAIM
LABEL: Stronger democracy
TEXT: Mandatory voting strengthens representative democracy.
STRENGTH: 5

NODE: C1
SIDE: CON
TYPE: COUNTERCLAIM
LABEL: Individual freedom
TEXT: Citizens should not be forced to participate in political expression.
STRENGTH: 5

LINK:
FROM: C1
TO: P1
RELATION: challenges

At this stage, the tool is contained in a single HTML file with embedded CSS and JavaScript.

Design goals

This prototype was designed to be:

low-code
visually expressive
useful for scholarly work
easy to learn quickly
exportable to future contexts

It is intended as a proof of concept showing how a scholar could create a non-prose visual representation of an argument without coding directly.

Current status

This is a working prototype. It currently supports:

parsing custom structured input
rendering styled nodes
drawing relationship connectors
displaying a visual legend
loading example datasets
showing syntax instructions in a modal

Possible future improvements include:

export to standalone HTML
PNG or SVG export
more layout modes
drag-and-drop adjustment
theme presets for publication, lecture, or poster use
improved cascade layout logic
editable palettes and typography options
Course context

This project was built in response to an assignment inviting students to create a new low-code/no-code tool. The assignment emphasized:

direct user editing
a sample outcome
export potential
GitHub sharing

Argument Mapper responds to that prompt by functioning as a mini authoring environment for scholarly visualization.

Author statement

Argument Mapper was designed as a bridge between scholarly writing and computational display. It treats structured thought as something that can be authored in plain language and then translated into a visual form suitable for teaching, presentations, and academic communication.

License

This project is shared as an educational prototype.
