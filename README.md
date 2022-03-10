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
-  [MI] Maintainability Index: MI = 171 - 5.2 * ln(V) - 0.23 (McCC) - 16.2 * ln(LOC)

# Building the tool 
You can build the tool with Maven to get an executable jar file: 
```
mvn package 
```
Using the tool 
The built jar is executable. It requires two parameters: 
1. A Solidity file or a directory containing Solidity files.
2. An output CSV file path.
```
java -jar Halstead4Sol-1.0.jar --inputFile [<filename>] --outFile [<filename>]
```

#Publications
This tool was built to aid an empirical analysis - Noama Fatima Samreen, Manar H. Alalfi, "Towards Analyzing correlation betwwen complexity landscape, security and maintainability of Solidity based DApps"

#Output
The output is a CSV file containing the values of the calculated halstead metrics for calculating the maintainability index of soldity smart contracts. 
