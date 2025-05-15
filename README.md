# 📱 App: MyWineCellar – Gestione della Cantina Domestica
## 🎯 Obiettivo dell’App
Consentire agli appassionati di vino di gestire facilmente la propria cantina domestica, tenendo traccia di bottiglie, annate, scadenze ottimali di consumo, con funzionalità avanzate come tag NFC/QR Code per inventario rapido ed esportazione in PDF del catalogo.

# 📦 Moduli Principali dell’App
## 1️⃣ Gestione Inventario
Inserimento nuovo vino con dettagli:

Nome, Annata, Tipologia (Rosso, Bianco, Rosato, Spumante, ecc.),

Quantità, Prezzo, Zona di Produzione, Gradazione Alcolica.

Stato: In Cantina / Pronto per Consumo / Bevuto / Esaurito.

Caricamento foto dell’etichetta o generazione di etichetta virtuale.

Countdown al miglior periodo di consumo.

## 2️⃣ Notifiche Intelligenti
Reminder per:

Bottiglie da consumare entro una certa data.

Scadenze su vini delicati (es. bianchi giovani).

Configurabile via WorkManager con notifiche dirette.

## 3️⃣ Inventario Rapido con NFC/QR Code
Generazione QR Code associato a ogni bottiglia (stampabile o salvabile).

Scansione NFC o QR Code per:

Vedere subito la scheda del vino.

Aggiornare lo stato della bottiglia (es. “Bevuta”).

NFC Tagging opzionale (per chi ha hardware compatibile).

## 4️⃣ Esportazione Catalogo PDF
Esportazione totale o filtrata (per tipologia, annata, disponibilità).

Opzioni PDF:

Includere note di degustazione e foto etichette.

Ordinamento personalizzato.

Condivisione diretta del PDF via email, WhatsApp, Drive, ecc.

## 5️⃣ Statistiche e Visualizzazioni
Grafico a torta: % vini per tipologia.

Grafico barre: Quantità di bottiglie per annata.

Countdown circolare per ogni vino con consumo consigliato.

# 📚 Architettura del Progetto

![image](https://github.com/user-attachments/assets/2a977cf0-7d97-41fa-a66d-ea09cffbb2ef)

# 🧩 Tecnologie e Librerie Principali
Jetpack Compose + Material 3: UI moderna.

Room: Local DB per salvataggio inventario.

DataStore: Preferenze utente (notifiche, ordinamenti).

Hilt: Dependency Injection.

ZXing / QRGen: Generazione e lettura QR Code.

PdfDocument API: Creazione PDF nativa (o iText 7 per PDF avanzati).

WorkManager: Notifiche programmate.

NFC API: Scrittura/lettura tag NFC.

# 📲 User Flow Principale
HomeScreen

Vedi elenco vini + countdown consumo.

Grafico rapido disponibilità.

Aggiungi Vino

Inserisci dati base + personalizza etichetta virtuale.

Genera e salva QR Code.

(Facoltativo) Scrivi su NFC.

Inventario Rapido

Scansiona QR o NFC ➔ Apri dettaglio vino immediatamente.

Esporta PDF

Scegli filtro + genera PDF ➔ Salva/Condividi.
