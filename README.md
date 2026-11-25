# .github

Default issue templates for every repository of the `Nosmoht` account that has no issue templates of its own.

## Contents

- `.github/ISSUE_TEMPLATE/issue.md`: decided work (feature, bug or task) with acceptance criteria.
- `.github/ISSUE_TEMPLATE/rfc.md`: proposal for an open decision. The decision leads to follow-up issues.
- `.github/ISSUE_TEMPLATE/config.yml`: disables blank issues in the web UI.

## How GitHub applies these defaults

GitHub uses the files in this repository as [default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file):

- This repository must stay public. The defaults then also apply to private repositories of the account.
- A repository with its own issue templates or its own `config.yml` in `.github/ISSUE_TEMPLATE/` uses none of these defaults. GitHub does not merge the two.
- A label set in a template must exist in each repository where the template is used.

## Limits

- `gh issue create --template "Issue"` inserts a template as starting body text. Nothing checks afterwards that the sections are filled, so a reviewer or agent checks them before work starts.
- AI agents treat the issue body as instructions. Assign an agent only to issues written by someone with write access to the repository.
