# Email Signature

Four HTML email signatures, derived from the same source of truth as the CV and
business card ([`../BACKGROUND.yaml`](../BACKGROUND.yaml)) and sharing the
business card's palette.

| File | Style | When to use |
| --- | --- | --- |
| [`signature-1-minimal.html`](signature-1-minimal.html) | Text hierarchy, one hairline rule | Default. Most robust across clients. |
| [`signature-2-accent-bar.html`](signature-2-accent-bar.html) | Green rule down the left edge | A little brand colour, still restrained. |
| [`signature-3-terminal.html`](signature-3-terminal.html) | fastfetch key/value block, monospace | Engineering correspondence; matches the card front. |
| [`signature-4-monogram.html`](signature-4-monogram.html) | "LS" tile plus hairline divider | The most designed option. |

[`preview.html`](preview.html) renders all four side by side — open it in a
browser to compare.

## Palette

Inherited from [`../business_card/card.tex`](../business_card/card.tex), so the
signature, the card and the CV read as one system.

| Token | Hex | Contrast vs `#FFFFFF` | Used for |
| --- | --- | --- | --- |
| Accent | `#1A7F37` | 5.08 | Links, keys, monogram fill |
| Body | `#1F2328` | 15.80 | Name, primary text |
| Muted | `#656D76` | 5.25 | Secondary lines |
| Rule | `#D0D0D0` | — | Hairlines (decorative) |

Accent and muted both clear the 4.5:1 WCAG AA threshold for body text.

## Email HTML constraints

These files deliberately avoid things that break in mail clients:

- **Tables, not flexbox or grid.** Outlook renders through Word, which supports
  neither.
- **Inline styles only.** Gmail strips `<style>` blocks in some contexts and
  external stylesheets always.
- **No images.** Clients block remote images by default on a first message from
  an unknown sender, and a signature that depends on one arrives broken. The
  accent bar is a cell border and the monogram is a filled cell, both for this
  reason.
- **System font stacks.** Web fonts do not load in most clients; every stack
  ends in a guaranteed family.
- **Explicit link colours.** Without them, clients apply their own blue, and
  some auto-link and restyle bare addresses.

## Installing

**Gmail** — open `preview.html` (or the individual file) in a browser, select
the rendered signature, copy, then paste into Settings → See all settings →
General → Signature. Pasting rendered output preserves the formatting; pasting
the raw markup does not.

**Apple Mail** — Settings → Signatures, create one, then paste the rendered
signature. If Mail strips the styling, quit Mail, replace the relevant
`~/Library/Mail/V*/MailData/Signatures/*.mailsignature` file with the markup
below its existing header lines, and make the file read-only.

**Outlook (web)** — Settings → Mail → Compose and reply, then paste the
rendered signature.

**Thunderbird** — Account Settings → check "Use HTML", or attach the `.html`
file directly via "Attach the signature from a file".

## Customising

- The email address is `lluc@lluc.sh` in every file, matching the business card.
  Replace it with `lluc.santa@gmail.com` to route replies there instead.
- Each file carries a commented-out phone block. Uncomment it to show
  `+34 639 41 25 89`; it is hidden by default, consistent with the CV and card.
- When the role or company changes, update `../BACKGROUND.yaml` first, then
  these files, per the repository convention.
