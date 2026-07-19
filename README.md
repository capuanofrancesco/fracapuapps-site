# Fracapu Apps

Portale statico ufficiale di Fracapu Apps.

## Struttura

- `index.html`: home page del sito con intestazione, hero, griglia app, sezione chi siamo, supporto e footer.
- `zefilandya-academy/index.html`: prima pagina dedicata a Zefilandya Academy, collegata dalla scheda app in Home.
- `styles.css`: stili globali, variabili CSS e componenti riutilizzabili per sezioni, pulsanti e schede app.
- `assets/.gitkeep`: cartella predisposta per futuri screenshot, immagini promozionali e asset delle applicazioni.

## Apertura locale

Il sito non usa framework, JavaScript, CDN o dipendenze esterne.

Per aprirlo localmente:

1. Aprire la cartella `fracapuapps-site`.
2. Aprire `index.html` con un browser moderno.

## Collegare una nuova pagina app alla Home

Per aggiungere una pagina dedicata a una nuova app:

1. Creare una cartella con slug leggibile, per esempio `nome-app/`, contenente `index.html`.
2. Collegare il CSS condiviso dalla pagina app con `../styles.css`.
3. In `index.html`, dentro `<div class="app-grid">`, aggiungere o aggiornare la scheda dell'app.
4. Usare un link con classe `button button-secondary` verso la cartella della pagina app.

Esempio di pulsante attivo nella scheda Home:

```html
<a class="button button-secondary" href="nome-app/">Scopri l'app</a>
```

Le classi `app-grid`, `app-card`, `app-card-top`, `app-icon`, `badge`, `app-meta`, `status-dot` e `button` sono pensate per essere riutilizzate senza aggiungere stili inline.

Per Zefilandya Academy saranno aggiunti successivamente screenshot, icona ufficiale, collegamento Google Play e privacy policy dedicata.

## Pagine previste in futuro

Il portale potra includere successivamente:

- pagine dedicate alle singole app;
- privacy policy separate per ogni app;
- pagine di supporto;
- collegamenti a Google Play;
- screenshot e immagini promozionali;
- eventuali nuove categorie di applicazioni.
