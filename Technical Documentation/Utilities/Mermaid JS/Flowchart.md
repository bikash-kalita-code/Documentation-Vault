### NOTE
- Instead of `flowchart` one can also use `graph`.

#### A node (default)
```mermaid
---
title: Node
---
flowchart LR
	id
```
#### A node with text
```mermaid
---
title: Node with text
---
graph LR
	id1[This is the text in the box]
```
#### Unicode text
Use `"` to enclose the unicode text.
```mermaid
flowchart
	id["This ❤ Unicode"]
```
#### Markdown formatting
Use double quotes and backticks "` text `" to enclose the markdown text.
```mermaid
%%{init: {"flowchart": {"htmlLabels": false}} }%%
flowchart LR
	markdown["`This **is** _Markdown_`"]
	newLines["`Line 1
	Line 2
	Line 3`"]
	markdown --> newLines
```
```mermaid
flowchart LR
	markdown["`This **is** _Markdown_`"]
	newLines["`Line 1
	Line 2
	Line 3`"]
	markdown --> newLines
```
#### Direction
This statement declares the direction of the Flowchart.
Possible FlowChart orientations are:
- TB - Top to bottom
- TD - Top-down/ same as top to bottom
- BT - Bottom to top
- RL - Right to left
- LR - Left to right
```mermaid
flowchart TB
	Start-->Stop
```
```mermaid
flowchart LR
	Start-->Stop
```
#### Node shapes
- **round edges:** `()`
- 
1. A node with round edges
```mermaid
flowchart LR
	id1(This is the text in the box)
```
2. A stadium shaped node
```mermaid
flowchart LR
	id1([This is the text in the box])
```
3. A node in a subroutine shape
```mermaid
flowchart LR
	id1[[This is the text in the box]]
```
4. A node in a cylindrical shape
```mermaid
flowchart TB
	id1[(This is the text in the box)]
```

