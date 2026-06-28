# Dipartimento: Software & Automation

App, plugin, workflow e automazioni sviluppate per risolvere problemi reali in contesti aziendali.
Non teoria — strumenti usati in produzione ogni giorno.

---

## Excel & VBA — Automazioni Aziendali

### After Sales — Gestione Claim
Tool Excel/VBA per la gestione del reparto after sales.
Tracciamento dei claim con apertura automatica via e-mail a tutti gli interessati, con tutte le informazioni precompilate. Eliminato il processo manuale completamente.

### Produzione Porte — Tracking Commesse
Excel per tracciare le commesse e i loro dettagli produttivi.
Quando lo studio tecnico completava il pacchetto, il sistema inviava automaticamente notifica alla produzione con tutto il necessario per partire. Zero comunicazioni manuali, zero errori di passaggio.

---

## Plugin Revit — Studio Tecnico SHD

Un sistema integrato di tre plugin che copre l'intera filiera progetto → produzione → cantiere.

### Plugin 1 — Referenziazione Pannelli
Assegna una referenza univoca a ogni pannello esistente nel progetto Revit.
Base del sistema: senza referenze univoche, niente può essere tracciato a valle.

### Plugin 2 — Abachi per Produzione e Acquisti
Genera automaticamente gli abachi completi per ogni locale, con tutte le referenze e le informazioni necessarie a ufficio acquisti e produzione.
Su commesse con centinaia di pannelli, eliminato completamente il lavoro manuale — operazione che richiedeva giorni, ora eseguita in secondi.

### Plugin 3 — Tavole per Installatori
Crea i prospetti di ogni locale con le referenze dei pannelli posizionate direttamente sulla tavola.
L'installatore in cantiere guarda la tavola e sa esattamente dove va ogni singolo pannello — il pannello 103 va lì, il 104 va là. Zero ambiguità, zero errori di montaggio.

**Il sistema nel suo insieme:** dal modello Revit al cantiere, ogni pannello ha un'identità, una destinazione e una tavola che la mostra. Progettato e sviluppato interamente da Simone.

---

## IoT — Sistema Smart Room
Sistema IoT completo per la camera personale.
Digital twin con calcolo consumi energetici in tempo reale, controllo remoto di luci LED via relay, monitoraggio temperatura e umidità con display fisico su ESP.
Accessibile e controllabile da qualsiasi dispositivo, ovunque.
Stack: ESP32/8266, Arduino, sensori DHT, relay, schermo OLED.

---

### Software Esterno — Generatore DWG di Produzione
Il tool più avanzato del sistema. Lavora a valle degli abachi Revit.

**Input:** tabella Excel con gli abachi dei pannelli
**Elaborazione:**
- Ricostruisce la modulazione geometrica della stanza da zero
- Applica la logica di posizionamento fori su ogni pannello (basata su altezza e vincoli tecnici specifici)
- Calcola i tagli dei profili strutturali dietro ai pannelli, incorporando tutte le regole produttive

**Output:** file DWG di ogni singolo pannello con forature corrette + lista tagli profili — pronti per andare direttamente in produzione

Quello che normalmente richiederebbe un disegnatore tecnico per ogni pannello, su ogni commessa, viene eseguito automaticamente. Sviluppato interamente da Simone, incorporando la conoscenza tecnica del prodotto e delle logiche di produzione.

---

## Asset da caricare
<!-- Screenshot tool Excel, demo plugin Revit, video sistema IoT -->
