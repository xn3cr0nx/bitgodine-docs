# Peeling Chain

Describes a specific transaction pattern, defined by a chain of one input and two outputs transactions. This pattern has been largely used by mixing services to obfuscate transactions [1] splitting outputs in smaller amounts to increase tracing. The heuristic considers the smaller output the change output because the the goal of this pattern is to proper "peel" a larger amount.

<br/>
<br/>

*[1] Michele Spagnuolo, Federico Maggi, and Stefano Zanero - 2014. Bitiodine: extracting intelligence from the bitcoin net-work. In volume 8437. (March 2014), 457–468.isbn: 978-3-662-45471-8.doi: 10.1007/978-3-662-45472-5_29*