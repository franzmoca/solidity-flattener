# solidity-flattener

[![npm](https://img.shields.io/npm/v/truffle-flattener.svg)](https://www.npmjs.com/package/truffle-flattener)

This is a fork of [nomiclabs/truffle-flattener](https://github.com/nomiclabs/truffle-flattener) that adds support to any project with a `contracts` directory. Thanks to the hardwork put together in the original repository.

Truffle Flattener concats solidity files from Truffle and Buidler projects 
with all of their dependencies.

This tool helps you to verify contracts developed with Truffle and Buidler 
on [Etherscan](https://etherscan.io), or debugging them on
[Remix](https://remix.ethereum.org), by merging your files and their
dependencies in the right order.

If you are still using Truffle, we recommend you try [Buidler](https://github.com/nomiclabs/buidler), 
our Ethereum development environment, which is much faster and flexible.

# Installation

`npm install @zemse/solidity-flattener -g`

# Usage

Just intall it with npm in your truffle project and run
`solidity-flattener <solidity-files>`.

# Limitations

Aliased imports (eg: `import {symbol1 as alias, symbol2} from "filename";`) are
not supported by `solidity-flattener`.

