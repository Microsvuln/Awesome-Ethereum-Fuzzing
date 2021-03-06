# Awesome-Ethereum-Fuzzing
A curated list for fuzzing ethereum

- [FuzzyVM](https://github.com/MariusVanDerWijden/FuzzyVM) - Implementation of a differential fuzzer for Ethereum Virtual Machines by [Marius van der Wijden](https://github.com/MariusVanDerWijden)
  - A framework to fuzz Ethereum Virtual Machine implementations. FuzzyVM uses two different processes. One process generates test cases and the other one executes them on different EVM implementations. 

- [Fluffy](https://github.com/snuspl/fluffy) - [Finding Consensus Bugs in Ethereum via Multi-transaction Differential Fuzzing](https://www.usenix.org/system/files/osdi21-yang.pdf) by [John Youngseok Yang](https://github.com/johnyangk)
  - Ethereum is the second-largest blockchain platform next to Bitcoin. In the Ethereum network, decentralized Ethereum clients reach consensus through transitioning to the same blockchain states according to the Ethereum specification. Consensus bugs are bugs that make Ethereum clients transition to incorrect blockchain states and fail to reach consensus with other clients. Consensus bugs are extremely rare but can be exploited for network split and theft, which cause reliability and security-critical issues in the Ethereum ecosystem. We describe Fluffy, a multi-transaction differential fuzzer for finding consensus bugs in Ethereum. First, Fluffy mutates and executes multi-transaction test cases to find consensus bugs which cannot be found using existing fuzzers for Ethereum. Second, Fluffy uses multiple existing Ethereum clients that independently implement the specification as cross-referencing oracles. Compared to a state-of-the-art fuzzer, Fluffy improves the fuzzing throughput by 510× and the code coverage by 2.7× with various optimizations: in-process fuzzing, fuzzing harnesses for Ethereum clients, and semantic-aware mutation that reduces erroneous test cases. Fluffy found two new consensus bugs in the most popular Geth Ethereum client which were exploitable on the live Ethereum mainnet. Four months after we reported the bugs to Geth developers, one of the bugs was triggered on the mainnet, and caused nodes using a stale version of Geth to hard fork the Ethereum blockchain. The blockchain community considers this hard fork the greatest challenge since the infamous 2016 DAO hack. We have made Fluffy publicly available at https://github.com/snuspl/fluffy to contribute to the security of Ethereum.

- [EVMFuzzer](https://github.com/renardbebe/EVMFuzzer) - [EVMFuzzer: Detect EVM Vulnerabilities via Fuzz Testing](http://wingtecher.com/themes/WingTecherResearch/assets/papers/fse19demo.pdf) by [Meng Ren](https://github.com/renardbebe)
  - Ethereum Virtual Machine (EVM) is the run-time environment for smart contracts and its vulnerabilities may lead to serious problems to the Ethereum ecology. With lots of techniques being continuously developed for the validation of smart contracts, the testing of EVM remains challenging because of the special test input format and the absence of oracles. In this paper, we propose EVMFuzzer, the first tool that uses differential fuzzing technique to detect vulnerabilities of EVM. The core idea is to continuously generate seed contracts and feed them to the target EVM and the benchmark EVMs, so as to find as many inconsistencies among execution results as possible, eventually discover vulnerabilities with output cross-referencing. Given a target EVM and its APIs, EVMFuzzer generates seed contracts via a set of predefined mutators, and then employs dynamic priority scheduling algorithm to guide seed contracts selection and maximize the inconsistency. Finally, EVMFuzzer leverages benchmark EVMs as cross-referencing oracles to avoid manual checking. With EVMFuzzer, we have found several previously unknown security bugs in four widely used EVMs, and 5 of which had been included in Common Vulnerabilities .

- [manticore](https://github.com/trailofbits/manticore) by [TrailOfBits](https://github.com/trailofbits)
  - Manticore is a symbolic execution tool for analysis of smart contracts and binaries.   

- [rattle](https://github.com/crytic/rattle) by [TrailOfBits](https://github.com/trailofbits)
  - Rattle is an EVM binary static analysis framework designed to work on deployed smart contracts. Rattle takes EVM byte strings, uses a flow-sensitive analysis to recover the original control flow graph, lifts the control flow graph into an SSA/infinite register form, and optimizes the SSA – removing DUPs, SWAPs, PUSHs, and POPs. The conversion from a stack machine to SSA form removes 60%+ of all EVM instructions and presents a much friendlier interface to those who wish to read the smart contracts they’re interacting with.

- [echidna](https://github.com/crytic/echidna) by [TrailOfBits](https://github.com/trailofbits)
  -  Echidna is a Haskell program designed for fuzzing/property-based testing of Ethereum smarts contracts. It uses sophisticated grammar-based fuzzing campaigns based on a contract ABI to falsify user-defined predicates or Solidity assertions. We designed Echidna with modularity in mind, so it can be easily extended to include new mutations or test specific contracts in specific cases.
  
-  [mythril](https://github.com/ConsenSys/mythril) by [ConsenSys](https://github.com/ConsenSys)
    - Mythril is a security analysis tool for EVM bytecode. It detects security vulnerabilities in smart contracts built for Ethereum, Hedera, Quorum, Vechain, Roostock, Tron and other EVM-compatible blockchains. It uses symbolic execution, SMT solving and taint analysis to detect a variety of security vulnerabilities. It's also used (in combination with other tools and techniques) in the MythX security analysis platform.   

- [ethersplay](https://github.com/crytic/ethersplay) by [TrailOfBits](https://github.com/trailofbits)
  - Binary Ninja plugin which enables an EVM disassembler and related analysis tools.

- [octopus](https://github.com/pventuzelo/octopus) by [Patrick Ventuzelo](https://github.com/pventuzelo)
  - Security Analysis tool for WebAssembly module (wasm) and Blockchain Smart Contracts (BTC/ETH/NEO/EOS)  

- [oyente](https://github.com/enzymefinance/oyente) by [Enzyme Finance](https://github.com/enzymefinance)
  - We built a symbolic execution tool called Oyente to find potential security bugs in contracts written by developers for the existing Ethereum system. Our objective for Oyente is to increase the security of the smart contracts by identifying vulnerabilities which will allow developers to mitigate the identified risks. Of the 19,366 existing Ethereum contracts, Oyente flags 8,833 of them as vulnerable, including the DAO bug which led to a USD 60 million loss in June 2016.

- [MAIAN](https://github.com/ivicanikolicsg/MAIAN) by [Ivica Nikolic](https://github.com/ivicanikolicsg)  
  - automatic tool for finding trace vulnerabilities in Ethereum smart contracts 

  
