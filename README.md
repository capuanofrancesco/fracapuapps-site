# Fracapu Apps

Portale statico ufficiale di Fracapu Apps.

## Struttura

- `index.html`: home page del sito con intestazione, hero, griglia app, sezione chi siamo, supporto e footer.
- `styles.css`: stili globali, variabili CSS e componenti riutilizzabili per sezioni, pulsanti e schede app.
- `assets/.gitkeep`: cartella predisposta per futuri screenshot, immagini promozionali e asset delle applicazioni.

## Apertura locale

Il sito non usa framework, JavaScript, CDN o dipendenze esterne.

Per aprirlo localmente:

1. Aprire la cartella `fracapuapps-site`.
2. Aprire `index.html` con un browser moderno.

## Aggiungere una nuova scheda app

In `index.html`, dentro il blocco:

```html
<div class="app-grid">
```

aggiungere un nuovo elemento seguendo la struttura delle schede esistenti:

```html
<article class="app-card">
  <div class="app-card-top">
    <div class="app-icon" aria-hidden="true">A</div>
    <span class="badge">Android</span>
  </div>
  <h3>Nome app</h3>
  <p>Descrizione breve dell'app.</p>
  <div class="app-meta">
    <span class="status-dot" aria-hidden="true"></span>
    <span>Stato o disponibilita</span>
  </div>
  <button class="button button-secondary" type="button" disabled>Scopri l'app</button>
</article>
```

Le classi `app-grid`, `app-card`, `app-card-top`, `app-icon`, `badge`, `app-meta`, `status-dot` e `button` sono pensate per essere riutilizzate senza aggiungere stili inline.

## Pagine previste in futuro

Il portale potra includere successivamente:

- pagine dedicate alle singole app;
- privacy policy separate per ogni app;
- pagine di supporto;
- collegamenti a Google Play;
- screenshot e immagini promozionali;
- eventuali nuove categorie di applicazioni.
