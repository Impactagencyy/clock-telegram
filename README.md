# Sveglia

Un cron che chiama un indirizzo HTTP ogni 5 minuti. Nient'altro.

L'indirizzo sta in *Settings → Variables* (`TICK_URL`), la chiave in
*Settings → Secrets* (`CRON_SECRET`): nessuno dei due è nel codice.

Esecuzione manuale: *Actions → sveglia-bot-telegram → Run workflow*.
