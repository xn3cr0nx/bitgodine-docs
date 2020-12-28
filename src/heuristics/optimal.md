# Optimal Change

The heuristic checks if an output amount is less than all input amounts. In this case, the output is very likely the change because if it would be the recipient, fewer inputs would have been enough to cover the amount, as explained in [1]. For example, we can consider a transaction composed by two inputs, respectively 2 and 3 Bitcoins, and two outputs, respectively 4 and 1 Bitcoin. Based on this heuristic, the change output is the one corresponding to 1 Bitcoin, because if the sender wanted to send 1 Bitcoin, only one the inputs would have been enough.

<br/>
<br/>

*[1] Jonas David Nick. 2015.Data-Driven De-Anonymization inBitcoin. en. Master’s thesis. ETH Zurich, Zürich.doi: 10.3929/ethz-a-010541254. Master’s Thesis, Distributed ComputingGroup Computer Engineering and Networks Laboratory,ETH Zürich, August 9, 2015*