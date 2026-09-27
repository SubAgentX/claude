# Project Bootstrap Playbook — source

`playbook.html` is the source of the playbook published as a Claude Artifact:

**https://claude.ai/artifact/UAeGHcB6XzXqgRdZovspCw**

The artifact is the copy you read; this file is the copy you edit. The page is
private to the Claude account that published it, so the link works for its
owner and anyone it has been shared with.

## What it covers

Every command needed to create a project from
[SubAgentX/project-template](https://github.com/SubAgentX/project-template),
with macOS, Linux and Windows commands switchable on the page.

## Editing it

It is a single self-contained HTML file — no build step, no dependencies. Open
it in a browser to preview:

```bash
# macOS
open playbook/playbook.html

# Linux
xdg-open playbook/playbook.html
```

```powershell
# Windows
Start-Process playbook\playbook.html
```

To publish an edit, ask Claude to republish this file to the artifact URL
above. Publishing without that URL creates a second, unrelated artifact.

## Keep it in step with the template

The playbook hard-codes commands from `project-template`. When any of these
change, update the matching step here:

| Changed in the template | Update in the playbook |
| :--- | :--- |
| `scripts/init.sh` / `init.ps1` arguments | Part two, step 3 |
| `scripts/lint.*` / `test.*` names | Part two, steps 5 and 6 |
| `.github/workflows/ci.yml` matrix | Part two step 7, and the CI cost note in part four |
| Repository name or owner | Every `gh` and `degit` command |
