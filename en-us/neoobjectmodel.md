# C# Smart Contract Developers Guide

[NEO Blockchain C# Center of Excellence](https://github.com/mwherman2000/neo-csharpcoe/blob/master/README.md)

The `neo-csharpcoe` project is an "umbrella" project for several initiatives related to providing tools and libraries (code), frameworks, how-to documentation, and best practices for full-stack development using .NET/C# and C#.NEO and the NEO Blockchain software platform.

The `neo-csharpcoe` is an independent, free, open source project that is 100% community-supported by people like yourself through your contributions of time, energy, passion, promotion, and donations.  To learn more about contributing to the `neo-csharpcoe`, click [here](https://github.com/mwherman2000/neo-csharpcoe/blob/master/CONTRIBUTE.md).

## Appendix - NEO Object Model Overview

### Purpose

TODO

### Goals, Non-Goals and Assumptions

TODO

### Principles

TODO

### Drivers

TODO

## NEO Object Model Overview

### NEO Blockchain Architecture Reference Model

The NEO .NET namespaces are illustrated below.

![NEO Blockchain Architecture Reference Model (.NET namespaces)](../neo-charm/diagrams/neo-charm-1-0-2.png)
Figure A.1. NEO Blockchain Architecture Reference Model (.NET namespaces)

The architecture of the NEO environment is illustrated in the following diagram. This diagram was inspired by the [Relfos/neo-debugger-tools](https://github.com/Relfos/neo-debugger-tools) project.

![NEO Blockchain Architecture Reference Model (subsystems)](../neo-charm/diagrams/neo-charm-2-0-1-annotated.png)
Figure A.2. NEO Blockchain Architecture Reference Model (subsystems)

### NEO Developer Environment

The following table describes the key components of the NEO developer environment.

| Mark | Name | Description |
|:----:|:--------------- | ----------------------------------------|
| ![A](../../images/balls/A32.png) | HelloWorld.cs | Smart contract source (example) 
| ![B](../../images/balls/B32.png) | csc.exe | C# Compiler
| ![C](../../images/balls/C32.png) | HelloWorld.dll | Smart contract compiled assembly (MSIL)
| ![D](../../images/balls/D32.png) | neon.exe |NEO Transcompiler (debugger version)
| ![E](../../images/balls/E32.png) | HelloWorld.avm | NEO VM script file (NEO byte code script)
| ![F](../../images/balls/F32.png) | neo-gui (developer) | Smart contract deployment and testing tool
| ![V](../../images/balls/V32.png) | Visual Studio | Microsoft .NET/C# IDE
| ![W](../../images/balls/W32.png) | neo-debugger | Interactive source and byte code level debugger

Table A.1. NEO Developer Environment

### NEO Virtual Machine

| Mark | Name | Description | Namespaces/APIs Callable by a Smart Contract |
|:----:|:--------------- |:--------------- | ----------------------------------------|
| ![G](../../images/balls/G32.png) | NEO VM | Virtual machine major components and services | -
| ![H](../../images/balls/H32.png) | ApplicationEngine | Execution enging components | -
| ![I](../../images/balls/I32.png) | CurrentContext | Execution engine current context | -
| ![J](../../images/balls/J32.png) | InstructionPointer | Execution engine current instruction pointer | -
| ![K](../../images/balls/K32.png) | Script | Current smart contract script being executed | `Neo.SmartContract.Framework.SmartContract`
| ![L](../../images/balls/L32.png) | ExecutionStack | Execution engine data stack | -
| ![M](../../images/balls/M32.png) | VMState | Virtual machine current state (HALT, FAULT, BREAK) | -
| ![N](../../images/balls/N32.png) | ScriptTable | Virtual machine script table of callable scripts | -
| ![O](../../images/balls/O32.png) | InteropService | Interop service layer for everything that isn't one of the basic execution engine capabilities (see above) | -
| ![P](../../images/balls/P32.png) | Account Service | Account service | `Neo.SmartContract.Framework.Services.Neo.Account`
| ![Q](../../images/balls/Q32.png) | Asset Service | Asset service | `Neo.SmartContract.Framework.Services.Neo.Asset`
| ![R](../../images/balls/R32.png) | Block Service | Block service | `Neo.SmartContract.Framework.Services.Neo.Block`
| ![S](../../images/balls/S32.png) | Blockchain Service, Header Service | Blockchain and Header services | `Neo.SmartContract.Framework.Services.Neo.Blockchain`, `Neo.SmartContract.Framework.Services.Neo.Header`
| ![T](../../images/balls/T32.png) | Contract Service | Contract service | `Neo.SmartContract.Framework.Services.Neo.Contract`
| ![U](../../images/balls/U32.png) | Runtime Service | Runtime service | `Neo.SmartContract.Framework.Services.Neo.Runtime`
| ![X](../../images/balls/X32.png) | Storage Service | Storage service | `Neo.SmartContract.Framework.Services.Neo.Storage`
| ![Y](../../images/balls/Y32.png) | Validator Service | Validator service | `Neo.SmartContract.Framework.Services.Neo.Validator`
| ![Z](../../images/balls/Z32.png) | Blockchain State | Distributed ledger | -

Table A.2. NEO Virtual Machine

TODO 

## References

[NEOARM] mwherman200, [NEO Blockchain Architecture Reference Model](https://github.com/mwherman2000/neo-windocs/blob/master/windocs/neo-charm/README.md#neo-blockchain-architecture-reference-model) from [https://github.com/mwherman2000/neo-windocs/blob/master/windocs/neo-charm/README.md#neo-blockchain-architecture-reference-model](https://github.com/mwherman2000/neo-windocs/blob/master/windocs/neo-charm/README.md#neo-blockchain-architecture-reference-model)


