# C#.NEO Smart Contract Developers Guide

[NEO Blockchain C# Center of Excellence](https://github.com/mwherman2000/neo-csharpcoe/blob/master/README.md)

The `neo-csharpcoe` project is an "umbrella" project for several initiatives related to providing tools and libraries (code), frameworks, how-to documentation, and best practices for full-stack development using .NET/C# and C#.NEO and the NEO Blockchain software platform.

The `neo-csharpcoe` is an independent, free, open source project that is 100% community-supported by people like yourself through your contributions of time, energy, passion, promotion, and donations.  To learn more about contributing to the `neo-csharpcoe`, click [here](https://github.com/mwherman2000/neo-csharpcoe/blob/master/CONTRIBUTE.md).  

## Purpose

The purpose of this document is capture the knowledge and best practices for C# smart contract development on the NEO Blockchain platform.

This document is specifically targeted at .NET developers and architects. 

### Caveat

In addition, when the first version of the document was written (February 2018), you will also need to have an [*early adopters*](https://en.wikipedia.org/wiki/Technology_adoption_life_cycle) mind set. It's the early days. You'll be downloading the code for most of the developer tools (aside from Visual Studio) and compiling them yourself. It may not always be fun but I promise it will certainly be rewarding in the end.

## Goals

* Capture basic as well as advanced knowledge related to developing C# smart contracts across the application lifecyle (ALM)
    * Requirements
    * NEO C# Language Considerations
    * NEO System Fees
    * Design Patterns
    * Creating Secure Contracts
    * Implementation
    * Deployment
    * Testing
    * Maintenance
    * Documentation
* Capture recommended best practices for C# smart contract development
* Non-goal: This scope of this document is limited to smart contract development only - not the other components and services of the [NEO Blockchain](../quickstart-csharp/README.md) platform.

## Principles

* Provide reliable documentation: timely, accurate, visual, and complete
* Save as much of a person's time as possible
* Use open source software whenever possible

## Drivers

* Need in the NEO .NET developer community to have concise and easy-to-follow documentation to enable people to get up to speed developing NEO smart contracts in as short a time as possible

## Sections

1. [Getting Started](./en-us/gettingstarted.md)
2. [Blockchain Basic Concepts](./en-us/blockchainbasicconcepts.md)
3. [What is NEO?](./en-us/whatisneo.md)
4. [NEO Development Tools](./en-us/neodevtools.md)
5. [Lab: Writing First C#.NEO Smart Contract: Hello World!](./en-us/labs/lab-helloworld.md)
6. [The C#.NEO Language](./en-us/csharpneointro.md)
7. [Lab: Using NEO Storage: Meetup Attendee Sign-in #1](./en-us/labs/lab-meetup1-storage.md)
8. [Introduction to Entities](./en-us/entitiesintro.md)
9. [Using Other Languages](./en-us/usingotherlanguages.md)
10. [NEO Architecture](./en-us/neocharm.md)
11. [Lab: Edit-Compile-Debug: Meetup Attendee Sign-in #2](./en-us/labs/lab-meetup2-ecd.md)
12. [NEO Persistable Classes Introduction](./en-us/npcintro.md)
13. [Programming with Entities](./en-us/programmingwithentities.md)
14. [Lab: Programming with Entities: Meetup Attendee Sign-in #3](./en-us/labs/lab-meetup3-entities.md)
15. [Off-chain Client Development](./en-us/offchainclientdev.md)
16. [Lab: Off-chain Client Development: Meetup Attendee Sign-in #4](./en-us/labs/lab-meetup4-clientdev.md)
17. [NEP5 Token Standard](./en-u/nep5tokensintro.md)
18. [Lab: NEP5 Tokens: A Meetup Token](./en-us/labs/lab-nep5tokens.md)
19. [Design Patterns](./en-us/designpatterns.md)
19. [Deployment](./en-us/deployment.md)
20. [Testing](./en-us/testing.md)
21. [Maintenance](./en-us/maintenance.md)
22. [Writing Secure Contracts](./en-us/securecontracts.md)
23. [Documentation](./en-us/documentation.md)
24. [Appendix A - NEO Object Model Overview](./en-us/neoobjectmodel.md)
25. [Appendix B - Roadmap](./en-us/guideroadmap.md)
26. [Appendix C - Sample Smart Contracts](./en-us/samplesmartcontracts.md)
27. [Appendix D - NEO System Fees](./en-us/systemfees.md)

## References

* [MSCODINGGUIDE] Microsoft, [C# Coding Conventions (C# Programming Guide)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions) from [https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)
    > The C# Language Specification does not define a coding standard. However, the guidelines in this topic are used by Microsoft to develop samples and documentation. 

    > Coding conventions serve the following purposes:

    > * They create a consistent look to the code, so that readers can focus on content, not layout.

    > * They enable readers to understand the code more quickly by making assumptions based on previous experience.

    > * They facilitate copying, changing, and maintaining the code.

    > * They demonstrate C# best practices.

* [FRAMEWORKGUIDLINES] Microsoft, [Framework Design Guidelines](https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/) from [https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/](https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/)
    > This section provides guidelines for designing libraries that extend and interact with the .NET Framework. ...

    > The guidelines are organized as simple recommendations prefixed with the terms Do, Consider, Avoid, and Do not. 

    >These guidelines are excerpted from the book Framework Design Guidelines: Conventions, Idioms, and Patterns for Reusable .NET Libraries, 2nd Edition, by Krzysztof Cwalina and Brad Abrams.

* [ETHCONCENSYSSECURITY] Concensys, [Smart Contract Security Best Practices (Ethereum)](https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README.md) from [https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README.md](https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README.md)

* [ETHSTYLEGUIDE] Solidity project, [Style Guide (Ethereum)](http://solidity.readthedocs.io/en/latest/style-guide.html) from [http://solidity.readthedocs.io/en/latest/style-guide.html](http://solidity.readthedocs.io/en/latest/style-guide.html)

* [ETHPATTERNS] Solidity project, [Common Patterns](http://solidity.readthedocs.io/en/latest/common-patterns.html) from [http://solidity.readthedocs.io/en/latest/common-patterns.html](http://solidity.readthedocs.io/en/latest/common-patterns.html)

* [ETHSECURITY] Solidity project, [Security Considerations](http://solidity.readthedocs.io/en/latest/security-considerations.html) from [http://solidity.readthedocs.io/en/latest/security-considerations.html](http://solidity.readthedocs.io/en/latest/security-considerations.html)

## Other Good Resources

* TODO


