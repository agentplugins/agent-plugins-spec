# Contributing to Agent Plugins

Agent Plugins defines a small, portable interoperability contract for plugin authors and client implementers. Changes to that contract succeed only when the relevant implementers can adopt them consistently.

## Specification Proposals

Start a [GitHub Discussion](https://github.com/agentplugins/agent-plugins-spec/discussions) before opening a pull request for a new feature or a material behavior change. A proposal should explain:

- the concrete implementation or interoperability problem;
- which plugin authors or client implementers encounter it;
- why the problem belongs in the portable specification rather than client policy or a client-specific extension; and
- which implementers are prepared to adopt the proposed behavior.

A technically complete pull request is not, by itself, evidence of implementor consensus or adoption. Maintainers may close proposals that have not established a concrete portability need or sufficient implementor support. When in doubt, begin with a Discussion rather than investing in a specification patch.

## Bugs and Editorial Corrections

Use [GitHub Issues](https://github.com/agentplugins/agent-plugins-spec/issues) for concrete defects such as contradictions, broken references, schema mismatches, or unclear requirements that can lead to incompatible implementations. Small, self-contained editorial corrections may be submitted directly as pull requests.

## Pull Requests

Keep each pull request focused on one independently reviewable change. When a change affects the portable contract, update every relevant surface together, including normative prose, schemas, examples, canonical identifiers, references, and the conformance checklist.

Describe the interoperability problem and the resulting contract in the pull request. Include the validation performed and link the prior Discussion or Issue when one exists.
