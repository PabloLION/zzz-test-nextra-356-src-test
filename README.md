# zzz-test-nextra-356-src-test

Testing [shuding/nextra#356](https://github.com/shuding/nextra/issues/356)

## Feedback

- In repro (6.) and (7.), with `beta.10` and `beta.9` respectively, the layout like header and sidebar is missing.
- In repro (6.) and (7.), with `beta.10` and `beta.9`, the markdown (`.md`) files can be rendered correctly.

## Repro

1. `pnpm create next-app`
2. `pnpm add next nextra react react-dom nextra-theme-docs`
3. `pnpm add @mdx-js/loader typescript webpack` (cannot run with some simple examples. I didn't install `nextra-theme-docs`)
4. move "pages/" to "src/pages/"
5. `pnpm add nextra@2.0.0-beta.10 nextra-theme-docs@2.0.0-beta.10`
6. move "pages/" back from "src/pages/" (no layout like header and sidebar)
7. downgrade to beta9 `pnpm add nextra@2.0.0-beta.9 nextra-theme-docs@2.0.0-beta.9` (no layout like header and sidebar). No commit for this step.
8. downgrade to stable version `pnpm add nextra@latest nextra-theme-docs@latest`, the sidebar is back.
