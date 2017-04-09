# Semantic Synchrony: An invitation to coders

Semantic Synchrony is a knowledge graph server with an Emacs front end. Here is a brief sample of its many [cool features]((https://github.com/synchrony/smsn/wiki/SmSn's-features-in-250-words). The [wiki]([2] https://github.com/synchrony/smsn/wiki) is thorough and friendly; it even includes demonstration videos.

The software is already powerful. We seek coders who want to make it more powerful yet.

## Languages

The server code is Java. The front end code is Emacs Lisp. They communicate via JSON. We want to incorporate Eta, a flavor of Haskell that compiles to the JVM.

The graph query language is Gremlin, part of Apache Tinkerpop. In fact, the front end is optional: the graph can be directly [accessed via Gremlin Console](https://github.com/synchrony/smsn/wiki/Gremlin-on-the-Graph).

Markdown is becoming critical to the data model.

## Data model in flux

The graph model is expanding from a graph with unlabeled edges to one with optional edge labels. Nodes serve optional double-duty as edge-labels.

Notes used to have to be plain text, but now they can be markdown as well. The graph model and the text model are evolving intertwined: Markdown headings are the vehicle for labeling edges.

The concept of a source of data is expanding, too. It used to have to be a graph, but now it includes git repositories, and more forms are on the way.

## It's not as much code as first appears. 

The only libraries you would need to know in order to radically change the program are [smsn](https://github.com/synchrony/smsn) (the server, in Java) and [smsn-mode](https://github.com/synchrony/smsn-mode) (the Emacs front-end, in Lisp). Moreover, much of smsn is experimental stuff that nobody really uses; exclude those things and it's much smaller.

## Contact us

We would love to hear from you. Find us on [Github](https://github.com/synchrony), [Gitter](https://gitter.im/synchrony), or [Facebook](https://www.facebook.com/semanticsynchrony).
