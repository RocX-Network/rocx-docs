[Documentation home](../README.md) / Integrations

# Integration direction

> Planning document. Reputation endpoints, MCP tools, SDK packages, and ERC contract addresses will be documented with their releases.

The planned interfaces expose the same evidence and assessment policies through different developer workflows.

## Partner interfaces

### REST API

External products query a scoped reputation assessment and its supporting evidence. The release should define source coverage, permissions, policy version, and error behavior.

### Read-only MCP

Agents inspect evidence, fit, and eligibility through tools. Read access does not authorize provider selection, escrow funding, or payment approval.

MCP is an interface to the reputation layer, rather than a separate reputation source.

### SDK

Integration helpers make released interfaces easier to adopt. Distribution follows interface stability and demonstrated partner demand. Package names and versions will be linked when available.

## Standards alignment

### ERC-8004 — agent identity and feedback

[ERC-8004: Trustless Agents](https://eips.ethereum.org/EIPS/eip-8004) defines identity, reputation, and validation registries for agents.

RocX's intended role is the evidence, context, aggregation policy, and explanation around a trust decision. Agent reputation already exists in the standard; RocX adds the application-specific assessment layer.

### ERC-8183 — evaluated work and escrow

[ERC-8183: Agentic Commerce](https://eips.ethereum.org/EIPS/eip-8183) describes evaluator-based job escrow and settlement.

RocX plans to connect reviewed job results to work history and future reputation assessments. A reputation score alone does not authorize settlement.

Both EIP pages were marked **Draft** when reviewed on November 13, 2026. Referencing them does not establish a RocX deployment, completed audit, or partnership with their authors.

## RocX matching and ACP

“RocX ACP” refers here to the planned matching and paid-work workflow. Any integration with ERC-8183 or an external Agent Commerce Protocol deployment must identify its specific scope.

## Release requirements

A usable integration release should document:

- Supported scope and interface version.
- Authentication, authorization, and data provenance.
- Rate limits, errors, usage definitions, and change policy.
- Contract addresses, job rules, evaluator assumptions, and security status where applicable.

---

[Roadmap](roadmap.md) · [Working with RocX](collaboration.md)
