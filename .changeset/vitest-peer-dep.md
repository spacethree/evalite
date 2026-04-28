---
"@spacethree/evalite": patch
---

Declare `vitest@^4` as a peer dependency. The package imports `vitest/node` directly but never listed `vitest` in its deps — only `@vitest/runner` and `@vitest/utils`. In a pnpm workspace where the root package has a different vitest version, evalite would walk up Node's module resolution and pick up the wrong vitest, failing with "No test files found" because the v2 vitest API differs from what evalite expects. Declaring it as a peer makes the requirement explicit and lets pnpm resolve it correctly from the consumer.
