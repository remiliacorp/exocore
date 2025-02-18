---
subtitle:
published: draft
date: 2022-04-22
tags: meta exocore computers learning
---

# The Exocore Workflow

{% graphviz %}

digraph G {

    bgcolor="black"
    node [shape=rectangle, style=filled fillcolor=black, color=orange, fontcolor=orange, labelfontcolor=orange];
    edge [color=orange, fontcolor=orange, labelfontcolor=orange];

  subgraph cluster_0 {
    style=filled;
    color= white;
    a0 -> a1 -> a2 -> a3;
    label = "process #1";
  }

  subgraph cluster_1 {
    node [style=filled];
    b0 -> b1 -> b2 -> b3;
    label = "process #2";
    color=blue
  }
  start -> a0;
  start -> b0;
  a1 -> b3;
  b2 -> a3;
  a3 -> a0;
  a3 -> end;
  b3 -> end;

  Images -> Attachments
  PDFs -> Library
  Attachments, Library -> "Library Page" [label=automatic];
  Images -> Posts [label="via ImagePaste"]

  "Daily Notes" -> "Journal Entries", Articles [label=embed];
  Wiki ->  "Daily Notes", "Journal Entries", Articles [label=embed];

  "Daily Notes"
  "Journal Entries"
  Articles
  Wiki
  Attachments [shape=folder]
  Library [shape=folder]
  start [shape=doublecircle];
  end [shape=Msquare];
}

{% endgraphviz %}
