# Address Type

This heuristic is based on the assumption that if all inputs addresses are of the same type, the change output is alike (<https://en.bitcoin.it/Privacy#Sending_to_a_different_script_type>). For example, if a transaction is composed by three P2PKH (Pay to Public Key Hash) type inputs and two outputs, a P2PKH type and a P2SH (Pay to Script Hash) type, the change address will be the P2PKH one.
