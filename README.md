# A scalable sequence encoding for collaborative editing

*Keywords: real-time collaborative editing, optimistic replication, replicated
 sequences*

*Authors: Brice Nédelec, Pascal Molli, Achour Mostéfaoui*


Distributed real-time editors made real-time editing easy for millions of
users. However, main stream editors rely on Cloud services to mediate sessions
raising privacy and scalability issues. Decentralized editors tackle privacy
issues but scalability issues remains. We aim to build a decentralized editor
that allows real-time editing anytime, anywhere, whatever is the number of
participants. In this paper, we propose an approach based on a massively
replicated sequence data structure that represents the shared document. We
establish an original tradeoff on communication, time and space complexity to
maintain this sequence over a network of browsers. We prove a sublinear upper
bound on communication complexity while preserving an affordable time and space
complexity. In order to validate this tradeoff, we built a full working editor
and measured its performance on large scale experiments involving up till 600
participants. As expected, the results show a traffic increasing as O((log I)^2
ln R) where I is the number of insertions in the document, and R the number of
participants.

## Acknowledgments

This work was partially funded by the French ANR project SocioPlug
([ANR-13-INFR-0003](http://www.agence-nationale-recherche.fr/?Projet=ANR-13-INFR-0003)),
and by the DeSceNt project granted by the Labex CominLabs excellence laboratory
([ANR-10-LABX-07-01](http://www.descent.cominlabs.ueb.eu/fr)). Experiments
presented in this paper were carried out using the [Grid’5000
testbed](https://www.grid5000.fr), supported by a scientific interest group
hosted by Inria and including CNRS, RENATER and several Universities as well as
other organizations.