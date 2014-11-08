---
layout: project
title: "Declarative Interaction Design for Visualization"
tagline: ""
description: "A declarative model for designing interactive visualization"
category: "paper"
tags: [Visualization, Interaction Design, Toolkits, Declarative design]

authors: [["Arvind Satyanarayan", "http://www.arvindsatya.com"], ["Kanit Wongsuphasawat", "http://kanitw.yellowpigz.com"], ["Jeffrey Heer", "http://jheer.org"]]

thumb: "/assets/peerapi/thumbs.png"
thumb_align: top
figure: "/assets/peerapi/thumbs.png"

link: ""

---
{% include JB/setup %}

Declarative visualization grammars can accelerate development, facilitate
retargeting across platforms, and allow language-level optimizations. However,
existing declarative visualization languages are primarily concerned with
visual encoding, and rely on imperative event handlers for interactive
behaviors. In response, we introduce a model of declarative interaction design
for data visualizations. Adopting methods from reactive programming, we model
low-level events as composable data \emph{streams} from which we form
higher-level semantic \emph{signals}. Signals feed \emph{predicates} and
\emph{scale inversions}, which allow us to generalize interactive selections
at the level of item geometry (pixels) into interactive queries over the data
domain. \emph{Production rules} then use these queries to manipulate the
visualization's appearance. To facilitate reuse and sharing, these constructs
can be encapsulated as named \emph{interactors}: standalone, purely
declarative specifications of interaction techniques. We instantiate our model
with extensions to the Vega visualization grammar. Through a diverse range of
examples, we demonstrate coverage over taxonomies of visualization interaction
techniques.
