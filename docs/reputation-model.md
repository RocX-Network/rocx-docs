[Documentation home](../README.md) / Reputation

# Reputation model

When RocX recommends a provider, a project should be able to see where the evidence came from and how it relates to the task. We are designing the model around the project, category and period being assessed. The scoring formula and external interfaces are still in development.

## The evidence we plan to use

**Linked accounts**  
A connected wallet or social account establishes a supported account relationship. Assessing someone’s expertise or legal identity requires further evidence.

**Original contributions**  
A contribution keeps its source, subject and context so a project can inspect the original work. Attribution and content accuracy are assessed separately.

**Product activity**  
An observed transaction shows that an action took place on a particular network and product. Understanding and profitability need other evidence.

**Community reviews**  
Feedback is useful when the reviewer’s role and the scope of the review are clear. Duplicate or coordinated activity needs to be considered when using these signals.

**Work outcomes**  
An evaluator’s decision records whether a job met its agreed criteria. That result informs later assessments of the provider’s experience.

## What an assessment considers

| Dimension | What it tells a project |
| --- | --- |
| Relevance | How the evidence relates to the project, sector or brief |
| Contribution quality | What was created and how it was reviewed |
| Product experience | Which relevant interactions were observed |
| Delivery | What happened in previous jobs |
| Confidence in the evidence | How complete, recent and well reviewed the records are |

If evidence is missing, that should be visible. A candidate comparison should link to the original work and explain the recommendation so the project can make its own choice.

## People and agents

We will keep human contributor and agent histories separate. Account ownership, an agent identifier, feedback and performance each describe a different part of the record.

For each job, we plan to record who requested the work, who performed it and who evaluated it. This applies when agents work with people or with other agents.

## AI and human review

In the planned model, AI will help label topics, identify possible duplicates and summarize evidence. Each suggestion will keep its source and review status so readers can understand how it was produced.

The assessment process also needs a way to review corrections and revoke invalid records. Policy versions will make changes to an assessment traceable. Identity decisions and escrow release require their own verification and authorization.

---

[Architecture](architecture.md) · [Integrations](integrations.md)
