# Semantic Synchrony: An invitation to coders

Semantic Synchrony serves a knowledge graph to an Emacs front-end running smsn-mode. Your graph can be selectively shared as a set of Git repositories; if so, their full git history is available in the front-end. The graph can be viewed as trees, traversed stepwise, and searched for keywords using boolean logic, using the Apache Lucene query language. More front-ends are possible; it communicates with the server using simple JSON.

The graph can also be directly [accessed via Gremlin Console](https://github.com/synchrony/smsn/wiki/Gremlin-on-the-Graph). Gremlin is a metalanguage for graph programming, part of Apache Tinkerpop. (If they change the details of Neo4j or Titan, and you write something in Gremlin, your code is safe.)

Here is a brief sample of Semantic Synchrony's many [cool features](https://github.com/synchrony/smsn/wiki/SmSn's-features-in-250-words). The [wiki](https://github.com/synchrony/smsn/wiki) is thorough and friendly; there are even demonstration videos.

## Languages

The server code is Java. The front-end code is Emacs Lisp. Those two communicate via JSON. We want to incorporate Eta, a flavor of Haskell that compiles to the JVM.

The graph query language is Gremlin.

Markdown is becoming critical to the data model, as is described next.

## Data model in flux

The model is expanding from a graph with unlabeled edges to one with optional edge labels. Nodes can serve double-duty as edge-labels.

Nodes used to have to be plain text, but now they can be markdown as well. The graph model and the text model are evolving intertwined: Markdown headings are a vehicle for labeling edges.

The concept of a source of data is expanding. It used to have to be a graph, but now it includes git repositories, and more forms are on the way.

## It's not as much code as it appears

The Emacs client, [smsn-mode](https://github.com/synchrony/smsn-mode), is small. The server, [smsn](https://github.com/synchrony/smsn), looks big, but much of smsn is experimental stuff that nobody really uses.

## Contact us

We would love to hear from you. Find us on [Github](https://github.com/synchrony), [Gitter](https://gitter.im/synchrony), or [Facebook](https://www.facebook.com/semanticsynchrony).
