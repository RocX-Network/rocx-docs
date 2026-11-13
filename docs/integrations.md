# Integration direction

**Planning document.** No public RocX reputation endpoint, MCP server, SDK package, or ERC deployment is released by this repository. Concrete URLs, schemas, authentication requirements, network addresses, and package versions will be documented with each release.

## Interfaces

| Interface | Intended role | Initial boundary |
| --- | --- | --- |
| REST API | Let external products query scoped reputation assessments and supporting evidence | Versioned read access with declared source coverage and permissions |
| MCP | Let agents inspect evidence, fit, and eligibility through tools | Read-only; no implied authority to select providers, fund jobs, or release payments |
| SDK | Make the released API and workflow integrations easier to adopt | Distributed after interfaces stabilize and partner demand is validated |

The API and MCP interfaces should use the same assessment policies and access scopes. MCP is a delivery interface, not a separate source of reputation. Billable usage definitions and pricing will be published separately when available.

## Standards alignment

| Reference | Standard's role | RocX's planned use |
| --- | --- | --- |
| [ERC-8004: Trustless Agents](https://eips.ethereum.org/EIPS/eip-8004) | Agent identity, feedback, and validation registries | Associate an agent record with relevant feedback and task evidence; provide contextual assessment and explanation |
| [ERC-8183: Agentic Commerce](https://eips.ethereum.org/EIPS/eip-8183) | Evaluator-based job escrow and settlement | Connect reviewed job results to RocX work history and reputation |

Both EIP pages were marked **Draft** when reviewed on November 13, 2026. Interfaces may change. These references do not establish that RocX has deployed compatible contracts, completed an audit, or partnered with the standards' authors.

ERC-8004 already includes a reputation registry. RocX's intended role is the evidence, context, aggregation policy, and application experience around trust decisions. It is not a claim that agent reputation is absent from the standard.

## RocX matching and ACP

“RocX ACP” refers here to the planned RocX matching and paid-work workflow. RocX does not claim ownership of external Agent Commerce Protocol infrastructure. Any implementation against ERC-8183 or another ACP deployment must identify that integration explicitly.

## Before a production integration

A release should specify its supported scope, authentication and authorization model, data provenance, rate limits, error behavior, change policy, and security status. Contract integrations also require published network addresses, job rules, evaluator assumptions, and an explicit review of the implementation.
