# HalsteadMetrics4Solidity

HalsteadMetrics4Solidity is a static analysis based Halstead Complexity calculator tool for Solidity smart contract programs. Currently, it supports the extraction of following numbers from solidity programs: 
-  η<sub>1</sub> = the number of distinct operators
-  η<sub>2</sub> = the number of distinct operands
-  N<sub>1</sub> = the total number of operators
-  N<sub>2</sub> = the total number of operands

From these numbers, following metrics are derived:

-  [η] Program vocabulary: η = η<sub>1</sub> + η<sub>2</sub>\,
-  [N] Program length: N = N<sub>1</sub> + N<sub>2</sub>\,
-  [V] Volume: V = N * ln (η) , 
-  [D] Difficulty : D = (η<sub>1</sub> / 2) * (N<sub>2</sub> / η<sub>2</sub>)
-  [E] Effort: E = D * V 
