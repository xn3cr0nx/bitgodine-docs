# Heuristics

Graph and cluster analysis are based on a set of widely studied heuristics that allow, under certain circumstances, to extract ad- ditional information from transactions [1, 2]. These heuristics exploit the transaction structure, in order to find relations between inputs and outputs. In particular, depending on the category the heuristic belongs to, we can group a set of addresses or identify which address is the receiver in a transaction. Table 1 summarizes the categories of heuristics that we are going to describe in the following:

- **Common inputs**: the first type of heuristic allows addresses clustering. It is based on the assumption that every input in a transaction is owned by the same user [1]. Although even [Nakamoto states](http://www.bitcoin.org/bitcoin.pdf) some linking is unavoidable, in Section 6 we will explain this is not always true. For our analysis, we rely on this heuristic and consider the inputs spending UTXO from the same wallet are owned by the same entity. In this way we group together all the addresses of spent outputs. This operation can be incrementally extended to others transactions containing common addresses composing large clusters of addresses.

- **Change address** the change output is the output containing the rest of the transaction returned to the sender. We can use the change output as a link to follow user’s coins across transactions. These heuristics can be affected by false positives and one of our goal is exactly to highlight their reliability and take into consider- ation whether some of them could be excluded. Table 2 provides a summary of change address heuristics. In the following, we will describe them and the properties they exploit to identify the change address [1, 3].

In the following we will describe different techniques to identify the change address.

<br/>
<br/>

*[1] Michele Spagnuolo, Federico Maggi, and Stefano Zanero - 2014. Bitiodine: extracting intelligence from the bitcoin net-work. In volume 8437. (March 2014), 457–468.isbn: 978-3-662-45471-8.doi: 10.1007/978-3-662-45472-5_29*<br/>
*[2] Harry A. Kalodner, Steven Goldfeder, Alishah Chator, MalteMöser, and Arvind Narayanan. 2017. Blocksci: design and ap-plications of a blockchain analysis platform.CoRR, abs/1709.02489*<br/>
*[3] Bitcoin wiki privacy. <https://en.bitcoin.it/Privacy>*
