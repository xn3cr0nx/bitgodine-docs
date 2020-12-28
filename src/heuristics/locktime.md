# Locktime

Timelocks are restrictions on transactions outputs that allow spending after some point in time [1]. The Bitcoin consensus rules define that a transaction with nLockTime field set to n can only be included in a block with a height of n+1 or higher and the most  Bitcoin wallets set the locktime of newly constructed transactions to the current block height [2]. This mechanism limits miners from executing a fee sniping attack. This attack could be attractive in the future when transaction fees will become the main monetary incentive for miners due to block subsidy declining to zero over time. In this attack, a miner with enough hashrate can
produce a block with higher fees and start a block race, splitting the chain, trying to impose the new branch as the main one in order to earn fees from that block. In this case, the miner could even include new blocks to maximize profitability and this behavior could potentially slow down the growth of the chain. Since the protocol cannot enforce a standard fee value, setting locktime to the current block n limits this attack because the transaction can only be included in a block with height at least n+1 and it reduces the incentive to reorg the chain for maximizing profitability. This heuristic suggests that if an output has been spent from a transaction that matches the locktime behavior of the transaction containing the output, it could be the change output.

<br/>
<br/>

*[1] Andreas Antonopoulos - 2017. Mastering Bitcoin. (second edi-tion). O’Reilly Media.* <br/>
*[2] 0xB10C - 2020. The stair-pattern in time-locked bitcoin trans-actions. <https://b10c.me/mempool-observations/1-locktime-stairs/>*
