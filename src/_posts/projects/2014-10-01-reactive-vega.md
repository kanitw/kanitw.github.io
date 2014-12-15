---
layout: publication
category: publication
title: "Declarative Interaction Design for Data Visualization"
authors: [ ["Arvind Satyanarayan", "http://arvindsatya.com/"], ["Kanit Wongsuphasawat", "/"], ["Jeffrey Heer", "http://jheer.org"]]
venue: "ACM User Interface Software & Technology (UIST), 2014"
caption: "Schematic for declarative overview + detail interaction. Mouse events in an overview (top) feed selection predicates based on drag start and end coordinates. Scale inversion is used to map the pixel range to date values, lifting the pixel-level selection to a query over the source data. This query is used to drive a filter transform for the focus view (bottom)."

tags: []

thumb: "/assets/reactive-vega/figure.png"
thumb_align: top
figure: "/assets/reactive-vega/figure.png"

projectpage: "http://idl.cs.washington.edu/papers/reactive-vega"
paper: "http://idl.cs.washington.edu/files/2014-DeclarativeInteraction-UIST.pdf"
vimeo-id: 100936827
---
{% include JB/setup %}

### Abstracts

Declarative visualization grammars can accelerate development, facilitate retargeting across platforms, and allow language-level optimizations. However, existing declarative visualization languages are primarily concerned with visual encoding, and rely on imperative event handlers for interactive behaviors. In response, we introduce a model of declarative interaction design for data visualizations. Adopting methods from reactive programming, we model low-level events as composable data streams from which we form higher-level semantic signals. Signals feed predicates and scale inversions, which allow us to generalize interactive selections at the level of item geometry (pixels) into interactive queries over the data domain. Production rules then use these queries to manipulate the visualization’s appearance. To facilitate reuse and sharing, these constructs can be encapsulated as named interactors: standalone, purely declarative specifications of interaction techniques. We assess our model’s feasibility and expressivity by instantiating it with extensions to the Vega visualization grammar. Through a diverse range of examples, we demonstrate coverage over an established taxonomy of visualization interaction techniques.


<!-- ### Abstract

Interactive systems are increasingly being used to explicitly support change in the user's psychophysiological state and behavior. One important trend in this vein is systems that support calm breathing habits. We designed and evaluated techniques to support respiratory regulation to reduce stress and increase parasympathetic tone. Our study revealed that auditory guidance was more effective than visual at creating self-reported calm. We attribute this to the users' ability to effectively map sound to respiration, thereby reducing cognitive load and mental exertion. Interestingly, we found that visual guidance led to more respiratory change  but less subjective calm. Thus, motivating users to exert physical or mental efforts may counter the calming effects of slow breathing. Designers of calming technologies must acknowledge the discrepancy between mechanical slow breathing and experiential calm in designing future systems. -->

