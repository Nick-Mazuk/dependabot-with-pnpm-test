# dependabot-with-pnpm-test

Does dependabot work with pnpm? Yes.

## Methodology

To test, I installed an old version of a package and setup a simple dependabot.yml file. I pushed the code to Github. If dependabot updates the outdated package, then it must work with pnpm.

## Dependabot.yml

Here's what the `.github/dependabot.yml` file looked like. I've removed the file from this repo so dependabot doesn't update this every day.

```yml
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "daily"
```
