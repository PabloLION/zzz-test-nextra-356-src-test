# zzz-test-nextra-356-src-test

Testing [shuding/nextra#356](https://github.com/shuding/nextra/issues/356)

## Repro

1. `pnpm create next-app`
2. `pnpm add next nextra react react-dom nextra-theme-docs`
3. `pnpm add @mdx-js/loader typescript webpack` (cannot run with some simple examples. I didn't install `nextra-theme-docs`)
4. `pnpm add nextra@2.0.0-beta.10 nextra-theme-docs@2.0.0-beta.10`
