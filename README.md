# HalsteadMetrics4Solidity

HalsteadMetrics4Solidity is a static analysis based Halstead Complexity calculator tool for Solidity smart contract programs. Currently, it supports the extraction of following numbers from solidity programs: 
- {\displaystyle\,\eta _{1} = the number of distinct operators
- {\displaystyle \,\eta _{2}}\,\eta _{2} = the number of distinct operands
- {\displaystyle \,N_{1}}\,N_{1} = the total number of operators
- {\displaystyle \,N_{2}}\,N_{2} = the total number of operands

From these numbers, following metrics are derived:

-  [n] Program vocabulary: {\displaystyle \eta =\eta _{1}+\eta _{2}\,}\eta =\eta _{1}+\eta _{2}\,
-  [N] Program length: {\displaystyle N=N_{1}+N_{2}\,}N=N_{1}+N_{2}\,
-  [V] Volume: {\displaystyle V=N\times \log _{2}\eta }V=N\times \log _{2}\eta 
-  [D] Difficulty : {\displaystyle D={\eta _{1} \over 2}\times {N_{2} \over \eta _{2}}}D={\eta _{1} \over 2}\times {N_{2} \over \eta _{2}}
-  [E] Effort: {\displaystyle E=D\times V}E=D\times V
