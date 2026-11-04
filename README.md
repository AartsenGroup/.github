# aartsengroup/.github

Organisation-wide defaults for the **aartsengroup** GitHub organisation.

> [!IMPORTANT]
> This repository is **public**. Never add internal project names, hostnames,
> credentials or other internal information. Internal content belongs in
> `aartsengroup/.github-private`.

## What is in here

| Path | Purpose |
| --- | --- |
| `profile/README.md` | Public organisation profile shown on github.com/aartsengroup |
| `SECURITY.md`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SUPPORT.md` | Default community health files for every repo that does not have its own |
| `.github/ISSUE_TEMPLATE/`, `PULL_REQUEST_TEMPLATE.md` | Default issue forms and PR template |
| `workflow-templates/` | Starter workflows shown under **Actions → New workflow** in org repos |

## Workflow templates

The templates in [`workflow-templates/`](workflow-templates/) are thin callers
of the reusable workflows in the internal `aartsengroup/shared-workflows`
repository. They have to live here, because GitHub only reads starter
workflows from the organisation's `.github` repository.

When `shared-workflows` releases a new **major** version, update the `@vN`
reference in the templates.
