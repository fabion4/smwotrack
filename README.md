# смвотрак — smwotrack

### Smart Working Tracker

> **smwotrack** /smvɔ'trak/ — dal russo **смотреть** _(smotrét' = osservare, monitorare)_ + **track** _(traccia)_.
> Sistema di pianificazione personale ispirato alla precisione dei piani quinquennali sovietici, ma con meno gulag e più Google Calendar.

---

Un calendario visuale per monitorare le giornate di Smart Working e Ferie. Gira interamente nel browser, senza server, senza account, senza raccolta dati. I tuoi dati non lasciano mai il tuo dispositivo.

## Funzionalità

- **Click ciclico a 3 stati**: vuoto → Smart Working → Ferie → vuoto
- **Contatori in tempo reale** con massimali editabili e residui (diventano rossi se sfori)
- **Festivi italiani** preconfigurati e personalizzabili nel codice
- **Salvataggio CSV** bidirezionale (salva e ricarica)
- **Esportazione ICS** per Google Calendar, Apple Calendar, Outlook
- **Importazione ICS** per ripristinare dati da un file calendario
- **Zero dipendenze server** — un singolo file HTML statico

## Come usarlo

1. Apri la [dashboard online](https://fabion4.github.io/smwotrack/) oppure scarica `index.html` e aprilo in locale
2. Clicca sui giorni per segnare Smart Working o Ferie
3. Salva il tuo lavoro con "Salva CSV"
4. Se vuoi vederlo nel calendario, usa "Esporta .ics"

## Personalizzazione dei festivi

Apri `index.html` con un editor di testo e cerca `const HOLIDAYS`:

```javascript
const HOLIDAYS = {
  '2026-04-06': 'Lunedì dell\'Angelo',
  '2026-04-25': 'Festa della Liberazione',
  '2026-05-01': 'Festa dei Lavoratori',
  '2026-06-02': 'Festa della Repubblica',
  // Aggiungi il patrono della tua città:
  // '2026-06-24': 'San Giovanni (Torino)',
  // '2026-06-29': 'Santi Pietro e Paolo (Roma)',
};
```

## Privacy

Questa app non raccoglie dati personali. Tutto (selezioni, CSV, ICS) resta nel tuo browser.

L'unico script esterno è [GoatCounter](https://goatcounter.com), un contatore di visite anonimo che non usa cookie, non traccia utenti e non richiede consenso GDPR.

## Contesto

Lo smart working nella Pubblica Amministrazione italiana sta attraversando una fase di forte ridimensionamento — in alcuni ministeri fino al 50% — proprio mentre la ricerca europea ([progetto REMAKING](https://lentepubblica.it/personale-e-previdenza/smart-working-nella-pa-la-ricerca-europea-remaking-conferma-benefici-per-lavoratori-e-territori/), Horizon) dimostra che il modello ibrido regolato è il più efficace per produttività, benessere e conciliazione vita-lavoro.

Questo strumento nasce da un'esigenza pratica: quando il tuo budget di giornate SW cambia da ufficio a ufficio e le regole non sono sempre chiare, serve un modo semplice per tenere il conto.

## Licenza

**[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.it)** — Creative Commons Attribution 4.0 International

Libero per qualsiasi uso, anche commerciale. L'unico obbligo è **citare l'autore originale**:

```
Based on Smart Working Tracker by FC
```
oppure
```
Derived from Smart Working Tracker (https://github.com/fabion4/smwotrack) by FC
```

Questo vale anche per versioni pesantemente modificate. Se il tuo progetto è basato su o ispirato da questo lavoro, cita l'originale.

---

© 2026 FC — Товарищ, контролируй свои дни. _(Compagno, tieni il conto dei tuoi giorni.)_
