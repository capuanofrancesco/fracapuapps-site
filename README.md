# Fracapu Apps

Portale statico ufficiale di Fracapu Apps.

## Struttura

- `index.html`: home page del sito con intestazione, hero, griglia app, sezione chi siamo, supporto e footer.
- `zefilandya-academy/index.html`: prima pagina dedicata a Zefilandya Academy, collegata dalla scheda app in Home.
- `privacy/index.html`: indice generale delle informative privacy delle applicazioni Fracapu Apps.
- `privacy/zefilandya-academy/index.html`: Privacy Policy italiana dedicata a Zefilandya Academy.
- `privacy/zefilandya-academy/en/index.html`: Privacy Policy di Zefilandya Academy in inglese.
- `privacy/zefilandya-academy/fr/index.html`: Privacy Policy di Zefilandya Academy in francese.
- `privacy/zefilandya-academy/es/index.html`: Privacy Policy di Zefilandya Academy in spagnolo.
- `privacy/zefilandya-academy/pt/index.html`: Privacy Policy di Zefilandya Academy in portoghese.
- `support/index.html`: pagina supporto con indirizzo email ufficiale e indicazioni per inviare richieste di assistenza.
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

Per Zefilandya Academy saranno aggiunti successivamente screenshot e collegamento Google Play.

## Privacy

La cartella `privacy/` contiene il blocco privacy del portale:

- `privacy/index.html` funziona come indice generale delle informative disponibili e future.
- `privacy/zefilandya-academy/index.html` contiene la policy italiana predefinita dedicata a Zefilandya Academy.

URL linguistici della Privacy Policy di Zefilandya Academy:

- `https://fracapuapps.com/privacy/zefilandya-academy/`
- `https://fracapuapps.com/privacy/zefilandya-academy/en/`
- `https://fracapuapps.com/privacy/zefilandya-academy/fr/`
- `https://fracapuapps.com/privacy/zefilandya-academy/es/`
- `https://fracapuapps.com/privacy/zefilandya-academy/pt/`

Le cinque versioni devono restare sincronizzate: ogni modifica a fatti tecnici, SDK, pubblicit&agrave;, dati trattati, conservazione, fornitori o diritti regionali deve essere riportata in tutte le lingue.

Paesi iniziali di distribuzione di Zefilandya Academy:

- Italia
- Francia
- Spagna
- Portogallo
- Brasile
- Stati Uniti
- Regno Unito
- Canada
- Australia
- Irlanda
- Nuova Zelanda

Per aggiungere in futuro la privacy policy di una nuova app:

1. Creare una sottocartella in `privacy/` con lo slug dell'app, per esempio `privacy/nome-app/index.html`.
2. Collegare il CSS condiviso con il percorso relativo corretto, di norma `../../styles.css`.
3. Aggiungere una nuova scheda nell'indice `privacy/index.html`.
4. Collegare la policy dal footer della pagina app e, quando naturale, dalla sezione supporto o informativa finale della pagina app.
5. Collegare la stessa URL anche dentro l'app e nella scheda Privacy della Play Console.

La policy deve essere rivista ogni volta che cambiano SDK, pubblicit&agrave;, dati trattati, servizi tecnici, hosting, normative o requisiti delle piattaforme. Brasile e Australia richiedono un nuovo controllo prima della pubblicazione o quando saranno pubblicate nuove linee guida definitive, in particolare su verifica dell'et&agrave; e codici privacy per minori.

La Privacy Policy deve essere collegata anche dentro l'app e nella Play Console. Le dichiarazioni Data Safety, le impostazioni Play Console e il comportamento reale dell'app devono restare coerenti con il testo pubblicato.

## Pagine previste in futuro

Il portale potra includere successivamente:

- pagine dedicate alle singole app;
- privacy policy separate per ogni app;
- pagine di supporto;
- collegamenti a Google Play;
- screenshot e immagini promozionali;
- eventuali nuove categorie di applicazioni.
