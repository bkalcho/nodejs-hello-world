# nodejs-hello-world
Simple Node.js app with automated release tagging via github actions

Analyzes commit messages and tags releases with semantic version tags, create
releases with release notes.
Release spec is defined in `.releaserc.yml` in the root of the repo.
GitHub is used as Npm registry which is defined in `package.json`.
Commit messages must use `[conventionalcommits](https://www.conventionalcommits.org/en/v1.0.0/)`
This can be further customized, by mapping commit message format `type`, optional `scope` to release: "patch", "minor", "major".

More info:
- [Conventional Commits Specification](https://www.conventionalcommits.org/en/v1.0.0/)
- [`commit-analyzer` Options](https://github.com/semantic-release/commit-analyzer#options)
- [Angular Commit Message Format *when using Angular format which inherits spec from conventional commit specification*](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit)

