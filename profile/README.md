<div align="center">
<h1>Full stack typesafe API-first development for REST</h1>

[![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/anttiviljami/openapi-stack/blob/master/LICENSE)
[![npm downloads](https://img.shields.io/npm/dw/openapi-backend)](https://www.npmjs.com/package/openapi-backend)
[![npm downloads](https://img.shields.io/npm/dw/openapi-client-axios)](https://www.npmjs.com/package/openapi-client-axios)
[![Buy me a coffee](https://img.shields.io/badge/donate-buy%20me%20a%20coffee-orange)](https://buymeacoff.ee/anttiviljami)

</div>

**openapi-stack** is a collection of open source libraries and tools for full stack software development using [OpenAPI specification](https://www.openapis.org/) with an API Design First philosophy.

The goal is to unlock great developer experience and full stack type safety for software teams using REST; inspired by tools like [GraphQL](https://graphql.org/) and [tRPC](https://trpc.io).

## Packages part of openapi-stack:

- [openapistack/openapi-backend ![GitHub Repo stars](https://img.shields.io/github/stars/anttiviljami/openapi-backend?style=social)](https://github.com/anttiviljami/openapi-backend)
- [openapistack/openapi-client-axios ![GitHub Repo stars](https://img.shields.io/github/stars/anttiviljami/openapi-client-axios?style=social)](https://github.com/anttiviljami/openapi-client-axios)
- [openapistack/openapicmd ![GitHub Repo stars](https://img.shields.io/github/stars/anttiviljami/openapicmd?style=social)](https://github.com/anttiviljami/openapicmd)

## Features

- [x] 🚀 Battle-tested in production. High test coverage.
- [x] 🤝 Built with TypeScript, types included with full autocomplete support
- [x] 🥃 Framework agnostic – works with your stack
- [x] 🏎 Lightweight - small frontend bundle + optimized for serverless cold starts
- [x] 🧙‍♂️ No code generation – we only generate types
- [x] ❤️ OpenAPI 3.x support
- [x] 👀 [Samples](https://openapistack.co/docs/examples/boilerplate/) included

<details>
<summary><b>How does openapi-stack compare to <i>GraphQL</i>?</b></summary>

[*GraphQL*](https://graphql.org/) is a query language for APIs developed by Facebook. It gives API clients full control over the data they query, making it extremely flexible and efficient for client-centric use cases.

Similar to [OpenAPI specification](https://www.openapis.org/), GraphQL APIs define a strongly typed schema for the data and mutations they support which makes them discoverable and intuitive to develop against.

OpenAPI stack achieves the same type safety and great developer experience by using the OpenAPI specification as a single source of truth for the API contract, used to generate types for both client and server side and utilising it for routing and validation during runtime.

Both GraphQL and openapi-stack encourage an [API First](https://openapistack.co/docs/api-first/) approach where the API contract is treated as a first class citizen in software design instead of treating it as merely documentation.

While REST APIs don't generally provide the same level of control to clients as GraphQL, many times this could be seen as a benefit especially in scenarios where strict control over data access and operations is crucial.

Many organizations choose REST over GraphQL due to more established conventions, simplicity, and the ability to leverage standard HTTP features directly. Widespread knowledge around REST contribute to its choice among organizations looking for a tried-and-tested approach to building APIs.
</details>

<details>
<summary><b>How does openapi-stack compare to <i>tRPC</i>?</b></summary>

[tRPC](https://trpc.io/) is a *Remote Procedure Call* (RPC) library for Typescript to build and consume typesafe APIs.

Designed for full-stack Typescript applications, tRPC allows direct sharing of types between both the client and server, without relying on code generation.

Unlike GraphQL and REST, tRPC doesn't expose a standard machine-readable API schema to be consumed by clients, instead taking a more straightforward approach of exposing endpoints or *procedures*, essentially [*"just functions"*](https://trpc.io/docs/concepts#its-just-functions) invoked by the client to the server.

OpenAPI stack achieves type safety using a similar workflow to tRPC's procedures with [*OpenAPI operations*](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md#operation-object), also avoiding code generation by only generating types from OpenAPI spec and using the machine readable contract in the runtime for routing and validation.

While the lightweight tRPC approach is optimal for teams just looking to build full stack applications, teams looking to build robust APIs are better served by the API design first approach of openapi-stack or GraphQL.

</details>

## API First Cycle

![API First Cycle](https://github.com/openapistack/docs/blob/main/static/img/openapi-stack.drawio.png?raw=true)

[Why API First?](https://openapistack.co/docs/api-first)
