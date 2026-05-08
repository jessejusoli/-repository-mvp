# API Documentation Guidance

This project should maintain API documentation when it exposes an API to users, services, agents, CLIs, or automation systems.

## API Source of Truth

| Area | Current Value |
| --- | --- |
| API style | `[API_STYLE]` |
| Contract file | `[OPENAPI_CONTRACT_PATH]` |
| Public docs URL | `[PUBLIC_API_DOCS_URL]` |
| Internal docs URL | `[INTERNAL_API_DOCS_URL]` |
| Owner | `[API_OWNER]` |

## OpenAPI Expectations

When the project exposes HTTP APIs, create and maintain an OpenAPI contract. The contract should support documentation viewers such as:

- Swagger UI;
- Scalar;
- Redoc.

The project should eventually define:

- where the OpenAPI contract lives;
- how the contract is generated or validated;
- how breaking changes are reviewed;
- how examples and error responses are documented;
- how API documentation is published.

## Contract Rules

- API behavior must not exist only in source code.
- Public endpoints must have documented request and response shapes.
- Error responses must be documented.
- Authentication and authorization expectations must be documented.
- Versioning and deprecation rules must be explicit before public release.

## Future API Checklist

| Item | Status | Notes |
| --- | --- | --- |
| Select API style | Proposed | REST, GraphQL, RPC, events, or another explicit style. |
| Add OpenAPI contract | Proposed | Required for HTTP APIs. |
| Add API docs viewer | Proposed | Swagger UI, Scalar, Redoc, or another selected viewer. |
| Add contract validation | Proposed | Should run in CI/CD once a contract exists. |
