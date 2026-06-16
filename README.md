# RedzSoul-OpenTaiko-Skin

Fork di [Moshir's OpenTaiko Skin](https://github.com/MoshirMoshir/Moshir-OpenTaiko-Skin), aggiornato per supportare **OpenTaiko 0.6.0.107** e personalizzato da RedzSoul.

Vedi [CREDITS.md](CREDITS.md) per i crediti completi.

## Requisiti

- **OpenTaiko versione 0.6.0.107** esatta. Versioni diverse (precedenti o successive) potrebbero non essere compatibili: questa skin include fix specifici per bug introdotti in questa versione (sistema `Modules/`, parsing texture). Per controllare la tua versione, guarda il titolo della finestra del gioco o il file `OpenTaiko.log`.

## Come installare

1. Scarica l'ultima release da [Releases](https://github.com/RedzSoul/RedzSoul-OpenTaiko-Skin/releases) (file `.zip`), oppure clicca il bottone verde `Code` → `Download ZIP` su questa pagina.
2. Estrai lo zip. Se hai scaricato dal bottone `Code`, otterrai una cartella tipo `RedzSoul-OpenTaiko-Skin-main`: apri quella cartella, il passo 3 si riferisce al suo **contenuto**, non alla cartella stessa.
3. Copia le seguenti due cose nella cartella di installazione di OpenTaiko:
   - la cartella `System/RedzSoul-OpenTaiko-Skin/` → dentro la cartella `System/` di OpenTaiko (risultato finale: `OpenTaiko/System/RedzSoul-OpenTaiko-Skin/`)
   - il contenuto della cartella `Global/` → dentro la cartella `Global/` di OpenTaiko, **unendo** i file (non sovrascrivere/eliminare quello che già c'è: questa skin aggiunge personaggi e Puchichara extra, non li sostituisce)
4. Avvia OpenTaiko, vai nelle impostazioni e seleziona **RedzSoul-OpenTaiko-Skin** come skin attiva.
5. **Riavvia completamente il gioco** (chiudi e riapri): OpenTaiko richiede un riavvio per applicare correttamente la nuova skin.
6. Enjoy!

### Dove si trova la cartella di OpenTaiko?

Dipende da come hai installato il gioco. Percorsi comuni su Windows:
- `%LocalAppData%\OpenTaiko Hub\OpenTaiko\` (installazione tramite OpenTaiko Hub)
- la cartella dove hai estratto/installato OpenTaiko manualmente

Se non sei sicuro, cerca la cartella che contiene `OpenTaiko.exe` e una sottocartella `System/`: quella è la cartella giusta.

## Risoluzione problemi

| Problema | Causa probabile | Soluzione |
|---|---|---|
| La skin non appare nella lista skin del gioco | Hai copiato l'intera cartella del repository invece di solo `System/RedzSoul-OpenTaiko-Skin/` | Verifica che il percorso finale sia `OpenTaiko/System/RedzSoul-OpenTaiko-Skin/SkinConfig.ini` (non annidato più in profondità) |
| Errori `CLuaModalScript`/`CLuaNamePlateScript` al boot | Stai usando una versione di OpenTaiko diversa da 0.6.0.107 | Verifica/aggiorna la versione del gioco |
| Personaggi o Puchichara extra mancanti | Non hai copiato il contenuto di `Global/` | Ripeti il passo 3, sezione Global |
| Le modifiche alla skin non si vedono dopo un cambiamento | Il gioco non è stato riavviato | Chiudi completamente OpenTaiko e riaprilo |

Per qualsiasi altro problema, apri una [issue](https://github.com/RedzSoul/RedzSoul-OpenTaiko-Skin/issues) con il messaggio di errore esatto (visibile in `OpenTaiko.log`, nella cartella di installazione del gioco).

## FAQ

1. Cosa sono i file `.kra`?
> File di lavoro Krita usati per creare i corrispondenti asset `.png`. Non servono per il funzionamento della skin, sono inclusi per chi vuole modificare gli asset.

## More Information

Per segnalare errori o suggerimenti, apri una issue su questo repository.
<br><br>
Se Namco o i proprietari degli asset hanno problemi con la distribuzione di questa skin o dei loro asset, contattatemi e renderò immediatamente privata la repository.
