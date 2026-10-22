# Bathys

Pianificatore di decompressione da usare a terra: Bühlmann ZHL-16C con gradient factors, circuito aperto (aria, nitrox, trimix, gas deco) e CCR con setpoint, bailout, contingenze, consumo gas e una modalità sperimentale con idrogeno.

**Non è un computer subacqueo** e non segue l'immersione reale. Le immersioni con decompressione, trimix e rebreather richiedono una formazione specifica.

## Pubblicare su GitHub Pages

1. Crea un repository, per esempio `bathys`, e carica tutti i file di questa cartella (compreso `.nojekyll`).
2. Su GitHub: **Settings → Pages → Build and deployment → Deploy from a branch**, branch `main`, cartella `/ (root)`.
3. Dopo un minuto l'app è su `https://<tuo-utente>.github.io/bathys/`.

## Installarla sul telefono

- **Android (Chrome):** apri l'indirizzo, menu ⋮ → **Installa app** (o "Aggiungi a schermata Home").
- **iPhone (Safari):** tasto Condividi → **Aggiungi alla schermata Home**.

Dopo la prima apertura funziona anche offline.

## Aggiornare

1. Sostituisci `index.html` su GitHub con la nuova versione.
2. In `sw.js` cambia `VERSION` (per esempio `bathys-v1.0`).

L'app si aggiorna da sola: quando il telefono è online scarica sempre prima la versione su GitHub e usa la copia salvata solo offline. Quattro secondi dopo l'avvio controlla anche se c'è una versione nuova e, se la trova, propone di aggiornare. Puoi forzare il controllo da Impostazioni → **Cerca aggiornamenti**.

Su iPhone l'app installata può restare aperta in memoria: se non vedi la novità, chiudila dal multitasking e riaprila.

## File

- `index.html`: l'app completa (motore di calcolo incluso).
- `manifest.webmanifest`, `icon-*.png`: installazione come app.
- `sw.js`: funzionamento offline.

I dati (impostazioni, gas, bombole, preset) restano solo sul telefono, nella memoria del browser.
