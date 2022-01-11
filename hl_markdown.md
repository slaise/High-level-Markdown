[TOC]

# High-level Markdown skills  

## TODO list

Future improvements:
- [ ] Point 1
- [ ] Point 2
- [x] Point 3

## Code diff

```diff
function compare (num1, num2) {
-  return ALL_SAME;
+  return NOT_SAME;
}
```

## Diagram
[Mermaid doc reference](https://mermaid-js.github.io/mermaid/#/flowchart)
### Flow Chart

```mermaid 
graph LR
    A[Christmas] -->|Get money| B(Go shopping)
    B --> C{Let me think}
    subgraph work
    C -->|One| D[Laptop]
    C --x|Two| E[iPhone]
    C -.->|Three| F[fa:fa-car Car]
    C ==> G((Bike))
    C --> J>TV]
    end
```

### Sequence Diagram
```mermaid
sequenceDiagram
    Alice->>+John: Hello John, how are you?
    Alice->>+John: John, can you hear me?
    John-->>-Alice: Hi Alice, I can hear you!
    John-->>-Alice: I feel great!
            
```

### Class Diagram
```mermaid
classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
      +String beakColor
      +swim()
      +quack()
    }
    class Fish{
      -int sizeInFeet
      -canEat()
    }
    class Zebra{
      +bool is_wild
      +run()
    }
            
```

### State Diagram
```mermaid
stateDiagram-v2
    [*] --> Still
    Still --> [*]
    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```

### Gantt
```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
            
```

### Pie chart
```mermaid
pie title Pets adopted by volunteers
    "Dogs" : 386
    "Cats" : 85
    "Rats" : 15
```

## Image
Control image width and height   
<img src="./cat.png" width=300px height=200px />    

Image align in the center
​​ <div align="center">![sleep-cat](./cat.png)</div>


## Fold 
<details>
<summary>Fold/Open</summary>
Folded content
</details>

## Math forumla
$\sum_{n=1}^{10} n^2$
$$\sum_{n=1}^{10} n^2$$

## Footnote
Here need a footnote[^noteID1]。

[^noteID1]: Here is the quote for **ID1**.
