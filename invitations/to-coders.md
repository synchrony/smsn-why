# A Semantic Synchrony pre-release invitation to coders

Semantic Synchrony is a knowledge graph server with an Emacs front end. Here[1] is a brief list of some of its many cool features. The wiki[2] is well-documented and friendly; it even includes demonstration videos. The server code is Java, and the front end code is Emacs Lisp. We want to incorporate Eta, a flavor of Haskell that compiles to the JVM.

The data model is in flux, currently expanding from an unlabeled graph to a labeled graph, where nodes can serve double-duty as edge-labels. Also the concept of a source of data is expanding; it used to have to be a graph, but now it includes git repositories, and more forms are on the way.

The software is already powerful, and we are looking for coders who want to make it more powerful yet. You can find us on Git[3] and Gitter[4].

It's not as much code as it first appears. The only libraries you would need to know in order to radically change the program are [smsn](https://github.com/synchrony/smsn) (the server, in Java) and [smsn-mode](https://github.com/synchrony/smsn-mode) (the Emacs front-end, in Lisp). Moreover, much of smsn is experimental stuff that nobody really uses; exclude those things and it's smaller yet.

[1] https://github.com/synchrony/smsn/wiki/SmSn's-features-in-250-words
[2] https://github.com/synchrony/smsn/wiki
[3] https://github.com/synchrony
[4] https://gitter.im/synchrony
