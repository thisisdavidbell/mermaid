# mermaid
A repo to try out using mermaid diagrams

# Links
- [mermaid](https://mermaid-js.github.io/mermaid/#/)


# Examples

## Example TD Graph
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

## Example flowchart
- [Syntax](https://mermaid-js.github.io/mermaid/#/flowchart)
```mermaid
flowchart LR
A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

## Example Sequence Diagram
- [Syntax](https://mermaid-js.github.io/mermaid/#/sequenceDiagram)
```mermaid
sequenceDiagram
    participant dotcom
    participant iframe
    participant viewscreen
    dotcom->>iframe: loads html w/ iframe url
    iframe->>viewscreen: request template
    viewscreen->>iframe: html & javascript
    iframe->>dotcom: iframe ready
    dotcom->>iframe: set mermaid data on iframe
    iframe->>iframe: render mermaid
```

## Pie chart
- [Syntax](https://mermaid-js.github.io/mermaid/#/pie)
```mermaid
pie
    title Key elements in Product X
    "Calcium" : 42.96
    "Potassium" : 50.05
    "Magnesium" : 10.01
    "Iron" :  5
```

## Example Gant
- [Syntax](https://mermaid-js.github.io/mermaid/#/gantt)
```mermaid
gantt
    section Section
    Completed :done,    des1, 2014-01-06,2014-01-08
    Active        :active,  des2, 2014-01-07, 3d
    Parallel 1   :         des3, after des1, 1d
    Parallel 2   :         des4, after des1, 1d
    Parallel 3   :         des5, after des3, 1d
    Parallel 4   :         des6, after des4, 1d
```

```mermaid
gantt
    axisFormat %A
    apple :a, 1w
    banana :crit, b, 23-7, 1d
    cherry :active, c, after b a, 1d
```
```mermaid
 gantt
        apple :a, 2017-07-20, 1w
        banana :crit, b, 2017-07-23, 1d
        cherry :active, c, after b a, 1d
``` 
