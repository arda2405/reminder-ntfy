# reminder-ntfy

Schickt alle 15 Minuten eine laute ntfy-Benachrichtigung mit dem Titel **21** aufs iPhone – außer von 1 bis 8 Uhr (deutsche Zeit).

- Ausgelöst wird der Workflow alle 15 Minuten von cron-job.org über die GitHub-API (`workflow_dispatch`). Die Nachtpause prüft der Workflow selbst.
- Nachricht und Pause: [.github/workflows/reminder.yml](.github/workflows/reminder.yml)
- Das ntfy-Topic liegt als Repo-Secret `NTFY_TOPIC` vor, nicht im Code.
- Pausieren: den Job bei cron-job.org deaktivieren.

Das Repo ist öffentlich, deshalb kosten die Läufe keine GitHub-Actions-Minuten.
