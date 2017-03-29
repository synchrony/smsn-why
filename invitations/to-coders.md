Semantic Synchrony is a knowledge graph server with an Emacs front end. Here[1] is a brief list of some of its many cool features. The wiki[2] is well-documented and friendly; it even includes demonstration videos. The server code is Java, and the front end code is Emacs Lisp. We want to add to it using Eta, a flavor of Haskell that compiles to the JVM. The software is already powerful, and we are looking for coders who want to make it more powerful yet. You can find us on Git[3] and Gitter[4].

If you pursue the code, the only libraries you would need to know in order to radically change the program are smsn (the server, in Java) and smsn-mode (the Emacs front-end, in Lisp). Moreover, much of smsn is experimental stuff that nobody really uses; exclude those things and it's a much smaller program.

[1] https://github.com/synchrony/smsn/wiki/SmSn's-features-in-250-words
[2] https://github.com/synchrony/smsn/wiki
[3] https://github.com/synchrony
[4] https://gitter.im/synchrony
