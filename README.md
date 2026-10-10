# reminder-ntfy

Schickt alle 15 Minuten eine laute ntfy-Benachrichtigung mit dem Titel **21** aufs iPhone – außer von 1 bis 8 Uhr (deutsche Zeit).

- Zeitplan und Nachricht: [.github/workflows/reminder.yml](.github/workflows/reminder.yml)
- Das ntfy-Topic liegt als Repo-Secret `NTFY_TOPIC` vor, nicht im Code.
- Pausieren: Actions-Tab → „Reminder 21“ → „…“ → „Disable workflow“.

Das Repo ist öffentlich, deshalb kosten die Läufe keine GitHub-Actions-Minuten. Damit GitHub den Zeitplan nicht nach 60 Tagen ohne Aktivität abschaltet, aktiviert sich der Workflow bei jedem Lauf selbst neu (Keepalive-Schritt).
