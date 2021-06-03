
# Awesome Plutus [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of amazingly awesome Plutus libraries, resources and shiny things.

Plutus is the new smart contract language for the Cardano blockchain.

This is intended to give the first waves of Plutus developers the best and most comprehensive information and tools for using plutus as fast as possible.

- [FAQ](#faq)
- [Official](#official)
- [Guides](#guides)
- [Videos](#videos)
- [Code Examples](#code-examples)
- [Testing](#testing)
- [Formal Specification Documents](#formal-specification-documents)

## FAQ

Q: Where can I find haskell libraries I can use with plutus.
A: We recommend https://hoogle.haskell.org - which allows you to search for functions by type.
   Please keep in mind that Plutus on-chain code will only support a subset of haskell.
   You might also want to take a look at [awesome-haskell](https://github.com/krispo/awesome-haskell#readme)

Q: How can I write/run plutus code today?
A: (As of may 19, 2021) - currently plutus does not have a public test net, plutus can run in a simulated chain using the Plutus Application backend, or PAB, which is available in the plutus monorepo.


## Official
- [Plutus Monorepo](https://github.com/input-output-hk/plutus) - the place to get started, depend on this repo to start a Plutus project
- [The Plutus Playground](https://playground.plutus.iohkdev.io)  - allows a Plutus script to be compiled and evaluated online
- [Official Plutus Tutorial](https://docs.cardano.org/projects/plutus/en/latest/plutus/tutorials/index.html) - a great starting place to get the foundations of Plutus
- [Plutus GHC Plugin Errors - Troubleshooting guide](https://alpha.marlowe.iohkdev.io/doc/plutus/troubleshooting.html) - the official guide to troublshooting Plutus plugin & Plutus Core generation issues.
- [How to Use Hoogle with the Plutus Monorepo](https://gist.github.com/t1lde/5649d86c97367f95bb026c23511249d5) - allows you to run Haskell's searchable documentation database, with the plutus library included

## Community Tutorials

- [The UTXO model explained with examples](https://bikemonkey.tech/the-utxo-model-explained-with-examples/) - since the Plutus smart contract platform uses an extended UTXO model, it is good to have a solid understanding of how this model works and how it is different from the Ethereum Account model.
- [Introduction to the Cardano blockchain ledger and smart contracts](https://apfelmus.nfshost.com/articles/cardano-ledger-intro.html) - a general introduction to the mechanics of smart contracts in the Cardano ecosystem

## Videos
- Plutus Pioneer Program Lectures - this is the first formal education program intended for the first wave of plutus developers
  - [Lecture #1](https://www.youtube.com/watch?v=igV7kMXcdpw)
  - [Lecture #2](https://www.youtube.com/watch?v=E5KRk5y9KjQ)
  - [Lecture #3](https://www.youtube.com/watch?v=Lk1eIVm_ZTQ)
  - [Lecture #4](https://www.youtube.com/watch?v=6Reuh0xZDjY)
  - [Lecture #5](https://www.youtube.com/watch?v=6VbhY162GQA)
  - [Lecture #6](https://www.youtube.com/watch?v=wY7R-PJn66g&t=2832s)
  - [Lecture #7](https://www.youtube.com/watch?v=oJupInqvJUI)
  - [Lecture #8](https://www.youtube.com/watch?v=JMRwkMgaBOg)
  - [Lecture #9](https://www.youtube.com/watch?v=-RpCqHuxfQQ)

## Code Examples
- [Plutus Use Cases](https://github.com/input-output-hk/plutus/tree/master/plutus-use-cases) - the first toy applications developed in plutus as proof of concept for industrial projects. a great reference including example test suites

## Testing
 the plutus monorepo currently provides two libraries that can be used to write effective tests for your plutus contract:
 
- [Wallet Emulator](https://github.com/input-output-hk/plutus/tree/master/plutus-contract/src/Wallet/Emulator) - can easily run tests in an emulated environment.
- [PAB Simulator](https://github.com/input-output-hk/plutus/blob/master/plutus-pab/src/Plutus/PAB/Simulator.hs) - can easily run tests or live interaction via http with a simulated local blockchain which supports Plutus

## Formal Specification Documents
- [The EUTXO Spec](https://github.com/hydra-supplementary-material/eutxo-spec/blob/master/extended-utxo-specification.pdf) - specification for extensions on the UTXO model, as used in Cardano, defines many of the base data types used in Plutus
- [The Plutus Platform Technical Report (DRAFT)](https://hydra.iohk.io/build/5735420/download/1/plutus.pdf) - a general overview of Plutus as a language and smart contract platform.
- [Plutus Core Formal Specification](https://hydra.iohk.io/build/5988492/download/1/plutus-core-specification.pdf) - the specification for the serializable core language built on system F which is used for the on-chain portion of Plutus.
