# Diez

Ten Spanish reading lessons, ten minutes each. Built to be installed on a phone
and worked through whenever, offline.

**https://olga-pyatokha.github.io/diez/**

Each lesson runs in four steps:

1. **Palabras** — meet the six new words first, with meaning, example and a
   memory hook. No typing. Inferring a new word from a single context gets it
   wrong more often than right, and a wrong guess sticks as firmly as a right
   one, so the word is met correctly before it is met in prose.
2. **Leer** — the passage, read for comprehension rather than guesswork.
   Support words above the working band are glossed; the translation stays
   behind a toggle so it cannot spoil the reading.
3. **Tarjetas** — retrieval, one card at a time. Nothing reveals until you have
   typed something, and the answer, translation and hook arrive immediately.
4. **Huecos** — cloze sentences that do not appear in the passage, checked
   ignoring accents.

Progress is stored in `localStorage` on the device. Nothing is uploaded. The
**Exportar respuestas** button dumps what you typed as JSON for grading.

Reminders: the page can raise a notification while it is open or backgrounded,
but a page cannot wake itself once the OS has frozen it, so the dependable daily
nudge is the generated `.ics` calendar event.

This repository holds only the built page — `index.html` is generated, do not
edit it here. Source and builder live in a separate private repo
(`spanish-learning`: `app/paquete_lecciones.json` + `scripts/make_package.py`).
