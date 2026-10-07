# Device Manager per Windows: rilasci

> **Device Manager ora si chiama Unusable.** Le versioni nuove escono in
> [giacomofuria/unusable-releases](https://github.com/giacomofuria/unusable-releases):
> installa Unusable una volta da lì, e riprende impostazioni, device e accesso
> all'account. Qui restano le versioni di Device Manager fino alla 3.0.17.

Qui ci sono solo l'installer e gli aggiornamenti di Device Manager: l'app per
gestire iPad, iPhone e device Android collegati al PC (WebDriverAgent, schermo
dal vivo, ispettore, team con i colleghi). L'app installata scarica da qui le
versioni nuove.

## Installare

1. Scarica **[DeviceManager-win-Setup.exe](https://github.com/giacomofuria/device-manager-releases/releases/latest/download/DeviceManager-win-Setup.exe)**
   dall'ultima release e avvialo.
2. L'installer non è firmato: se Windows mostra "PC protetto da Windows",
   scegli **Ulteriori informazioni → Esegui comunque**.
3. Si installa per il tuo utente, senza privilegi, e installa da sé il
   .NET 10 Desktop Runtime se manca. Alla fine apre l'app.

L'app parte sempre come amministratore (serve al tunnel iOS): a ogni avvio
Windows chiede la conferma UAC.

Requisiti: Windows 10 o 11 a 64 bit. Per iPad e iPhone servono anche i driver
Apple (app "Dispositivi Apple" dal Microsoft Store) e go-ios; per Android i
platform-tools (adb).

## Aggiornamenti

Sono automatici: l'app controlla da sola, scarica in sottofondo e mostra
**Aggiorna a x.y.z** in alto. Con la conferma si chiude e si riapre aggiornata;
altrimenti si aggiorna al prossimo avvio.

## Disinstallare

Impostazioni di Windows → App → Device Manager.

## Senza installare

`DeviceManager-win-Portable.zip`, nella stessa release: si estrae in una
cartella e si avvia.
