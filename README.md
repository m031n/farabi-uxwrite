# skills
AI skills designed and developed to improve Product Designer workflows

## Available skills

- [`persian-writing`](./persian-writing) — general Persian/Farsi writing, orthography, register, humanization, cleanup, spell-checking, and RTL document guidance, synced from [ali2000hos/persian-writing](https://github.com/ali2000hos/persian-writing).
- [`farabi-writer`](./farabi-writer) — Persian product and Farabi writing guidance, composed with the general `persian-writing` rules.
- [`farsi-trading-ux-writing`](./farsi-trading-ux-writing) — professional Persian UX copy for trading apps, including personas, risk context, dialogs, errors, empty states, toasts, and terminology consistency.

## How the skills compose

Use `persian-writing` as the foundation whenever the task contains Persian text:
it governs register, naturalness, orthography, نیم‌فاصله, Persian punctuation and
digits, and RTL output. Use `farabi-writer` for product-interface copy and
`farsi-trading-ux-writing` for trading-specific copy. The more specific skill
adds product context; it does not override the general Persian-writing rules
unless the product has an explicitly approved term or exact value.

The bundled `persian-writing` package retains its upstream MIT license and
maintenance guidance. If its `SKILL.md` or references change, regenerate its
single-file edition with `python3 persian-writing/scripts/build_universal.py`.
