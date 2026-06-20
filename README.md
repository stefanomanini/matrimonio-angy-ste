# Sito matrimonio Ste & Angy

Sito vetrina statico multi-pagina per il matrimonio di Ste & Angy, pronto per il deploy gratuito su GitHub Pages.

Il progetto non usa backend, database, framework pesanti o build Node. Funziona aprendo `index.html` in locale e puo essere pubblicato dalla branch `main`, cartella `/root`.

## Struttura del progetto

- `index.html`: home page, gia nella root del progetto.
- `storia.html`, `programma.html`, `location.html`, `rsvp.html`, `menu.html`, `info.html`, `lista-nozze.html`, `foto.html`, `privacy.html`, `404.html`: pagine statiche collegate con percorsi relativi.
- `assets/css/style.css`: stile del sito.
- `assets/js/main.js`: menu mobile e voce di navigazione attiva.
- `assets/img/`: immagini placeholder, favicon e immagine Open Graph.
- `.nojekyll`: indica a GitHub Pages di servire il sito come statico puro.

## Aprire il sito in locale

1. Apri la cartella del progetto.
2. Fai doppio clic su `index.html`.
3. Naviga tra le pagine dal menu.

Non serve installare nulla e non serve avviare un server.

## Pubblicare gratis con GitHub Pages

### 1. Creare una repository GitHub

1. Vai su [GitHub](https://github.com/).
2. Accedi al tuo account.
3. Clicca su `New repository`.
4. Inserisci un nome, per esempio `matrimonio-angy-ste`.
5. Scegli `Public` se vuoi usare GitHub Pages gratis in modo semplice.
6. Clicca su `Create repository`.

### 2. Caricare i file

Puoi caricare i file dal sito GitHub:

1. Entra nella repository appena creata.
2. Clicca su `Add file` > `Upload files`.
3. Trascina dentro tutti i file e le cartelle di questo progetto.
4. Verifica che `index.html` sia nella root della repository, non dentro una sottocartella.
5. Clicca su `Commit changes`.

In alternativa puoi usare Git da terminale:

```bash
git init
git add .
git commit -m "Pubblica sito matrimonio"
git branch -M main
git remote add origin https://github.com/NOME-UTENTE/matrimonio-angy-ste.git
git push -u origin main
```

Sostituisci `NOME-UTENTE` e `matrimonio-angy-ste` con i dati reali della repository.

### 3. Andare su Settings > Pages

1. Apri la repository su GitHub.
2. Clicca su `Settings`.
3. Nel menu laterale clicca su `Pages`.

### 4. Scegliere Deploy from a branch

Nella sezione `Build and deployment`, alla voce `Source`, seleziona:

```text
Deploy from a branch
```

### 5. Selezionare branch main e cartella /root

1. Alla voce `Branch`, scegli `main`.
2. Nel menu della cartella scegli `/root`.
3. Clicca su `Save`.

### 6. Ottenere il link pubblico del sito

Dopo il salvataggio, GitHub Pages impiega di solito qualche minuto per pubblicare il sito.

Torna in `Settings` > `Pages`: quando il deploy e pronto, GitHub mostra un messaggio con il link pubblico, simile a:

```text
https://NOME-UTENTE.github.io/matrimonio-angy-ste/
```

## Dove modificare il sito

- Testi: modifica i file `.html` nella root.
- Colori: modifica le variabili in `assets/css/style.css`, dentro `:root`.
- Foto: sostituisci i file in `assets/img/` mantenendo gli stessi nomi, oppure aggiorna i percorsi `src` negli HTML.
- RSVP: in `rsvp.html` sostituisci `https://forms.google.com/` con il link del Google Form ufficiale. Puoi anche cambiare l'indirizzo nel link `mailto:`.
- Mappa: in `location.html` sostituisci il link Google Maps con quello definitivo della location.
- Open Graph: modifica `assets/img/og-ste-angy.svg` o i meta tag `og:*` nelle pagine HTML.

## Checklist deploy

- `index.html` e nella root.
- I link interni usano percorsi relativi, per esempio `programma.html`.
- CSS collegato con `assets/css/style.css`.
- JavaScript collegato con `assets/js/main.js`.
- Nessun backend richiesto.
- RSVP gestito tramite Google Form o email precompilata.

