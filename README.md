# Sveglia dei bot Telegram

Questo repository non contiene codice dell'agenzia: è solo un **orologio**.

Ogni pochi minuti chiama la rotta `/api/telegram/tick` del gestionale CLOCK, che
controlla le fasce orarie dei bot-canale Telegram e pubblica le frasi dovute.
Serve perché il piano Vercel Hobby fa girare i cron una sola volta al giorno.

- Il segreto sta in **Settings → Secrets → `CRON_SECRET`** (mai nel codice).
- L'indirizzo sta in **Settings → Variables → `TICK_URL`**.
- Puoi lanciarlo a mano da **Actions → sveglia-bot-telegram → Run workflow**.

Se un giorno il gestionale passa a Vercel Pro, questo repository si può spegnere:
basterà un cron nel `vercel.json`.
