# Segretario — release

Qui ci sono solo gli **installer** di Segretario per Windows e il file `latest.json` che l'app usa per aggiornarsi da sola. Il codice sorgente non è pubblico.

## Installare

1. Apri l'ultima [release](https://github.com/VarTommaso/segretario-releases/releases/latest).
2. Scarica `Segretario_<versione>_x64-setup.exe` ed eseguilo. L'installazione è per il tuo utente: non servono diritti di amministratore.
3. Al primo avvio Windows SmartScreen può mostrare "Windows ha protetto il PC", perché l'installer non ha una firma Authenticode. Scegli **Ulteriori informazioni → Esegui comunque**.

Requisiti: Windows 10 o 11 a 64 bit. Il runtime WebView2 è già incluso in Windows 11; su Windows 10 l'installer lo scarica se manca.

## Aggiornamenti

L'app controlla una volta al giorno se c'è una versione nuova e propone *Installa e riavvia*. In Impostazioni → Questo dispositivo puoi anche cercare un aggiornamento a mano.

Ogni aggiornamento è firmato con la chiave dell'autore: l'app rifiuta un file che non corrisponde alla firma.

## Cosa contiene ogni release

| File | A cosa serve |
|---|---|
| `Segretario_<versione>_x64-setup.exe` | installer NSIS per Windows x64 |
| `latest.json` | versione, note e firma, letti dall'updater dell'app |
