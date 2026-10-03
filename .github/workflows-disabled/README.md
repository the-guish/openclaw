# Disabled workflows

This fork runs only `.github/workflows/sonarqube.yml`. The upstream OpenClaw
workflows were moved here, where GitHub Actions ignores them. They stay in Git
so merges from upstream apply cleanly, and any of them can be restored with:

```sh
git mv .github/workflows-disabled/<name>.yml .github/workflows/
```

Workflows added by future upstream merges land in `.github/workflows/` and run
until they are moved here as well.
