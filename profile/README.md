# Ziggurat
> Earthquake testing blockchain networks

<p align="center">
    <img src="https://github.com/runziggurat/.github/blob/main/profile/assets/logo.png" height="300px">
</p>

Like the multi-stepped pyramids of antiquity, Ziggurat stands to provide multiple layers of stability for your peer-to-peer network. By reverse-engineering the network protocol and using lightweight "synthetic" nodes, Ziggurat provides blockchain node developers with the foundation of reliability, performance, and scalability needed to realize their true potential.

Our coverage so far includes ZCash, Aleo, Algorand, and the XRP Ledger. More are on the way.

## Coverage Details

Ziggurat started with the three single-node layers of testing - Conformance, Performance, and Resistance (CPR). However, we are now exploring (and in some cases performing) network-wide analysis and testing.

## Single Node Tests

The CPR test suite has become a staple of any Ziggurat implementation:

1. **Conformance** to the network specification
   1. Does a network spec exist?[^1]
   2. Do all clients exhibit the same networking behavior?
   3. Do any inconsistencies cause incompatibility between clients?
2. **Performance** under scale
   1. Does your node experience slowdowns under increased load?
   2. ...heavy load? _Very_ heavy load?
   3. What factors of your node's engineering lead to performance bottlenecks?
3. **Resistance** to bad actors.
   1. How does your node respond to unexpected messages?
   2. Does your node inadvertendly allow malicious or unexpected behaviors?

## Network-wide

1. Network Crawler
   1. How many nodes are running on your network?
   2. How many are running _well_?
   3. What versions of clients and network protocols are out there?
   4. What other analytics can we gather from the peer-to-peer network?
2. Data analytics and visualization
<!-- 2. Testnet Red-Teaming (coming soon!) -->
<!-- 2. DoS protection (coming soon!) -->

## Development Cycle

Ziggurat is compatible with networks at any phase of deployment. For example - the CPR tests can be run during development or pre-deployment, and the network-wide tests can be run on devnet, testnet, or even mainnet.

[^1]: Sometimes, the Ziggurat test suite _becomes_ the de-facto networking spec

# Coverage

|  Network           | Spec Conformance | Fuzzing | Crawler | Malicious Actor Modeling | Visualization | Performance Benchmarking |
|--------------------|------------------|---------|---------|--------------------------|---------------|--------------------------|
| [ZCash]            | Yes              | Yes     | WIP     | Yes                      | WIP           | Yes                      |
| [XRP Ledger]       | WIP              | WIP     | No      | WIP                      | WIP           | WIP                      |
| [Algorand]         | WIP              | No      | No      | WIP                      | No            | No                       |
| Aleo               | No               | No      | WIP     | No                       | WIP           | No                       |  
| Polkadot           | No               | No      | No      | No                       | No            | No                       |

[ZCash]: https://github.com/runziggurat/zcash
[XRP Ledger]: https://github.com/runziggurat/xrpl
[Algorand]: https://github.com/runziggurat/algorand

# Contributing

Feedback and contributions from the open source community are welcome. If you have any queries, you can open an issue in the relevant repository and our team will take it from there.
