---
"@spacethree/evalite": major
---

Initial release of `@spacethree/evalite`, the SpaceThree fork of [evalite](https://github.com/mattpocock/evalite). The fork adds a Postgres storage adapter (`@spacethree/evalite/postgres-storage`) for persisting eval results to PostgreSQL — includes optional `postgres` peer dependency, configurable schema/table names, and conditional test coverage via `EVALITE_TEST_POSTGRES_URL`. Renamed from `evalite` to `@spacethree/evalite` so it can be published to GitHub Packages while we wait on upstream PR review.
