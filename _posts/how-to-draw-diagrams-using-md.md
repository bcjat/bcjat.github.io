---
title: 	Example Diagrams
date: 2020-08-02 23:50:12 +0530
categories: [Technology, Markdown]
tags: [mermaid]     # TAG names should always be lowercase
author: Balvant Jat
---



# How to draw diagrams using markdown?

### Simple Sequence Diagram

```mermaid
sequenceDiagram
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```



```mermaid
flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```



### Complex Sequence Diagram 

```mermaid
  sequenceDiagram
    Alice->>Bob: Hello Bob, how are you?
    alt is sick
    Bob->>Alice: Not so good :(
    else is well
    Bob->>Alice: Feeling fresh like a daisy
    end
    opt Extra response
    Bob->>Alice: Thanks for asking
    end
```

