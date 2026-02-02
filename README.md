# Welfare as a Service per i Comuni – (WaaS per i Comuni)

Questo repository contiene le specifiche tecniche per le API di popolamento del  
**SIUSS – Sistema Informativo Unitario dei Servizi Sociali**  
([Sistema Informativo Unitario dei Servizi Sociali](https://www.inps.it/it/it/dati-e-bilanci/siuss--ex-casellario-dell-assistenza.html))  
da parte dei Comuni aderenti al progetto **Welfare as a Service (WaaS)**.

---

## Procedura di adesione al servizio

A partire dal 2025, l’attivazione del servizio di **Alimentazione WAAS-SIUSS** è supportata da un  
**template eService PDND** predisposto dall’INPS, denominato:

**`Consultazione Flussi SIUSS - WaaS`**

Il template consente agli Enti di pubblicare l’eService su PDND in modo standardizzato, riducendo la complessità di configurazione e garantendo coerenza con le specifiche del servizio.

Il template è attualmente disponibile sia in **ambiente di collaudo** che in **ambiente di produzione** e costituisce la modalità di adesione di riferimento.

👉 Le istruzioni operative dettagliate per l’utilizzo del template sono disponibili nella documentazione di dettaglio del repository.

---

## Passi per l’adesione

Per abilitare il servizio di alimentazione, l’Ente aderente deve:

1. Implementare l’API di alimentazione in accordo alle specifiche  
   [OpenAPI del servizio](https://github.com/INPS-it/WaaS.Comuni/blob/main/002%20-%20OpenAPI/api-comuni.yaml);
2. Aderire alla piattaforma PDND, se non già effettuato, secondo la  
   [guida all’adesione PagoPA](https://docs.pagopa.it/interoperabilita-1/manuale-operativo/guida-alladesione);
3. Pubblicare l’eService di Alimentazione SIUSS su PDND tramite il **template eService INPS**;
4. Inviare una richiesta di adesione a **progettowelfareasaservice@inps.it** indicando:
   - nome dell’Ente;
   - codice Belfiore;
   - IP o range di IP di erogazione del servizio (collaudo e produzione);
5. Accettare la richiesta di fruizione del servizio da parte di INPS sull’ambiente di Collaudo;
6. Dare seguito alle eventuali segnalazioni tecniche inviate da INPS ai contatti dell’Ente;
7. Accettare la richiesta di fruizione del servizio da parte di INPS sull’ambiente di Produzione.

Gli Enti che hanno già pubblicato autonomamente l’eService prima dell’introduzione del template possono continuare a utilizzare le erogazioni già attive.

---

## Struttura del repository

### Documentazione tecnica

Il repository contiene:
- gli schemi **`.xsd`** che descrivono i flussi SIUSS;
- la specifica **OpenAPI** in formato **`.yaml`** per le API esposte dai Comuni su PDND.

---

## Licenze

- I file **`.xsd`** e **`.yaml`** sono rilasciati con licenza **MIT**.
- Il file **`.pdf`** di descrizione del progetto è rilasciato con licenza **CC-BY 4.0**.
