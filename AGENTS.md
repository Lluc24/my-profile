# AGENTS.md

Instructions for AI coding agents working in this repository.

## Attribution

Lluc Santamaria Riba is the author and owner of this repository. Any commit or
pull request an agent creates here is collaborative work and must credit him as
a co-author.

**Every commit** must end with this trailer, verbatim:

```
Co-Authored-By: Lluc Santamaria Riba <lluc.santa@gmail.com>
```

**Every pull request** description must credit him the same way — add the
trailer as the last line of the PR body:

```
Co-Authored-By: Lluc Santamaria Riba <lluc.santa@gmail.com>
```

Notes:

- The trailer goes in the commit message body, separated from the prose by a
  blank line, alongside any other trailers (an agent's own `Co-Authored-By`,
  session links, and so on). Git treats each `Co-Authored-By` line as a
  separate co-author, so multiple lines are fine and expected.
- This applies to every commit, including small fixes, amends, and merge
  commits an agent authors.
- Do not substitute another address. The work-email address is for identifying
  Lluc as a user; commit attribution in this repository uses
  `lluc.santa@gmail.com`.

## Repository conventions

- `BACKGROUND.yaml` is the single source of truth for the professional profile.
  Update it first; the CV and business card are derived views.
- After editing `cv/*.tex` or `business_card/*.tex`, recompile and commit the
  regenerated PDF so the checked-in PDFs always match their source. The CV needs
  two `pdflatex` passes and must stay one page.
