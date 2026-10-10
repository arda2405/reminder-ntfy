# reminder-ntfy

Schickt alle 15 Minuten eine laute ntfy-Benachrichtigung mit dem Titel **21** aufs iPhone – außer von 1 bis 8 Uhr (deutsche Zeit).

- Zeitplan und Nachricht: [.github/workflows/reminder.yml](.github/workflows/reminder.yml)
- Das ntfy-Topic liegt als Repo-Secret `NTFY_TOPIC` vor, nicht im Code.
- Pausieren: Actions-Tab → „Reminder 21“ → „…“ → „Disable workflow“.

Jeder Lauf kostet eine GitHub-Actions-Minute (privates Repo): 68 Läufe pro Tag ≈ 2.100 Minuten im Monat.
