# Noise vs. sunlight: A technological solution to the fake news problem

Humanity -- not just the internet, but academia, science, governments, the press -- are in a crisis of trust. Trust is a network effect. For most of history the authorities were unassailable, because most people were unable to broadcast. Someone in the 80s could shout that the world was flat, but nobody would hear him, and the idea wouldn't take off. Now it can.

The ability to broadcast is not going away; our new democratic noise is probably permanent. I propose that we counter it with more information, in a more organized state.


## The tech ideas: cryptography, digital identity and knowledge (hyper)graphs

Cryptography allows the owner of an online identity to prove that they are responsible for a message.

Investing in a digital identity in a robust network can be expensive. Creating a fake Facebook identity, for example, requires substantial resources. It is doable, but for many purposes it is not worth the cost.

Knowledge graphs are what power search engines; they are a structure for storing disparate kinds of information. In a vanilla graph there are two kinds of things: nodes ("objects") and edges ("relationships") between pairs of nodes. A knowledge graph could encode information like "birds are animals", "animals need oxygen", and "combustion consumes oxygen". Traversing that graph can then allow someone to infer further information, like "combustion threatens birds".

A hypergraph extends the expressivity of a graph, enabling relationships with more than two members, and relationships among relationships. Examples include Datalog, HypergraphDB and Grakn. (Note that the term "hypergraph" is more inclusive among computer scientists than it is among mathematicians.)


## Using hypergraphs to navigate across authors

The internet's fantastic power is hampered by two problems: (1) Noise, and (2) Limits on our ability to query. They're really the same problem.

Noise comes in a few flavors: idiots, liars, and perfectly fine people writing things you don't care about.

Were there no limits on our ability to query, noise would not be a problem. We could simply ask for a view that did not include noise. We actually have the technology to pose that kind of query already, but we don't have the data -- we would need some objective measure of information quality.

There are feasible queries, however, that could approximate it. "Show me posts only from authors I trust", or "from friends of friends of friends", or "that have received X number of likes", or "from authors with a PhD (according to accreditation body X) in subject Y", or "from authors who have published articles on X, Y and Z," or "from people with at least 100 online relationships that are at least 5 years old" ... *Any* criteria you can verbalized could be made into a hypergraph query.

Hypergraphs allow the encoding of arbitrary metadata. It is standard to think of search engines as attaching information like author and topic to articles. It is not (yet?) standard to think of other authors as attaching information to that article. They could, though -- and often would like to. We would like to attach reviews of the article, or of the author. We would like to attach information to fragments of the article -- definitions, examples, motivations, applications, supporting evidence, contradictory evidence, personal reactions ...

Facebook collects a tiny shadow of this kind of information -- likes, hearts, etc. YCombinator and Reddit allow user sentiment to usefully reshape their data. Wikis are the current extreme of democratized content.

Hypergraphs could be like quantum wikis: Everyone's contributions could coexist. In linear text, keeping everyone's contributions would quickly create an unreadable mess, but a graph, like a tree, provides a navigable order.

The full potential hypergraph -- everything everyone's said about anything including other stuff other people have said -- would be a lot of data. It wouldn't have to stay on a single server. There already exist distributed search engines.


## Building an online identity

Cryptography could allow us to be sure of which digital entity has said what. They only need to sign everything they write. And authors would *want* to sign everything they write, if the hypergraph search engine took their entire publication history into account.

If users could take an author's online history into account when querying, the expense of creating an online identity would make it hard for fake identities to get traction. Writing under a pseudonym would remain possible, and identities could be merged (though not split) -- if your pseudonym becomes famous, and you want to claim its works as your own, you can.
