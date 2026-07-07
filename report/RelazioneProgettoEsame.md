---
title: Science & Disinformation Briefs
author: Daniele Del Pozzo 82253A 
date: a.a. 2025/2026
institute: Università degli Studi di Milano
course: Editoria Digitale
tags: tag1, tag2, tag3
version: 0.1
kind: Document
bibliography: bibliografia.bib
csl: IEEE.csl

header-includes:
  - \usepackage{float}
  - \usepackage{graphicx}
---

\begin{center}

\includegraphics[width=3cm]{./logo/minerva.jpg}

\end{center}



## Introduzione


Il progetto nasce con l’obiettivo di realizzare un prodotto editoriale digitale dedicato al tema della disinformazione scientifica, un fenomeno di crescente rilevanza che influenza la diffusione delle informazioni in ambiti quali salute, intelligenza artificiale, politica e sostenibilità. L’obiettivo è fornire contenuti sintetici, affidabili e facilmente consultabili, rivolti a giornalisti, comunicatori della scienza e lettori interessati ad approfondire argomenti di attualità attraverso fonti scientifiche open access.

Per raggiungere tale obiettivo ho sviluppato un sito web statico organizzato in più pagine, nel quale ogni articolo affronta uno specifico aspetto della disinformazione. I contenuti sono redatti in linguaggio divulgativo e accompagnati da riferimenti alle pubblicazioni scientifiche utilizzate, così da garantire trasparenza e verificabilità delle informazioni.

Dal punto di vista tecnico, il progetto è stato realizzato adottando un flusso di produzione documentale basato su Markdown, MkDocs con il tema Material for MkDocs, Git e GitHub Pages. Questa soluzione permette di separare il contenuto dalla presentazione grafica, automatizzare la generazione delle pagine HTML e semplificare gli aggiornamenti futuri del sito.

Particolare attenzione è stata inoltre dedicata all’esperienza di fruizione dei contenuti. Ogni articolo presenta una struttura uniforme, comprensiva della data di pubblicazione e di uno social media snippet finale, pensato per facilitare la diffusione del contenuto attraverso i principali canali social. L’intero progetto è stato sviluppato privilegiando la modularità, la riproducibilità del processo editoriale e la possibilità di estendere facilmente il sito con nuovi articoli e nuovi temi. 

## Ideazione 

### Tema


Il tema scelto per il progetto è la disinformazione scientifica, intesa come la diffusione di informazioni false, fuorvianti o prive di adeguato supporto scientifico riguardanti argomenti di interesse pubblico. Negli ultimi anni questo fenomeno ha assunto un ruolo sempre più rilevante, favorito dalla rapida diffusione dei contenuti attraverso i social media e le piattaforme digitali, con conseguenze significative sulla formazione dell’opinione pubblica e sulla fiducia nei confronti della comunità scientifica.

La scelta di questo argomento è motivata dalla sua forte attualità e dalla crescente necessità di fornire strumenti che consentano di distinguere informazioni affidabili da contenuti non verificati. In particolare, il progetto si propone di offrire una sintesi accessibile di recenti studi scientifici open access, traducendo risultati della ricerca in un linguaggio comprensibile anche a un pubblico non specialistico.

Per evitare una trattazione eccessivamente generica, il tema principale è stato suddiviso in diversi sottotemi, ciascuno affrontato in un articolo dedicato. Questa scelta consente di approfondire differenti manifestazioni della disinformazione, evidenziandone le caratteristiche specifiche e gli effetti nei rispettivi contesti. Ad esempio, gli articoli analizzano fenomeni quali la disinformazione legata all’intelligenza artificiale, la manipolazione dell’informazione in ambito politico, la diffusione di false informazioni in campo sanitario e le possibili strategie di contrasto.

L’organizzazione del sito in articoli indipendenti permette inoltre di aggiornare facilmente i contenuti e di ampliare in futuro il prodotto editoriale con nuovi temi, mantenendo una struttura coerente e facilmente navigabile.




### Destinatari


Il prodotto editoriale è progettato per un pubblico interessato alla divulgazione scientifica e alla verifica delle informazioni, con particolare attenzione a coloro che necessitano di contenuti sintetici, affidabili e facilmente consultabili.

Per definire i requisiti del progetto ho individuato tre principali *personas*.

- **Giornalista scientifico**


Il primo destinatario è un giornalista o redattore che si occupa di informazione scientifica e di attualità. Questa figura necessita di comprendere rapidamente i risultati della ricerca scientifica per trasformarli in articoli divulgativi destinati al grande pubblico. Il sito fornisce sintesi chiare, riferimenti ag li articoli originali e collegamenti diretti alle fonti open access, facilitando il processo di verifica delle informazioni.

**Scenario d'uso.** Prima della pubblicazione di un articolo riguardante la disinformazione, il giornalista consulta il sito per individuare studi scientifici recenti e ottenere una panoramica dell'argomento.



- **Studente universitario**


Il secondo destinatario è uno studente universitario interessato ai temi della comunicazione scientifica, dell'informatica, della medicina o delle scienze sociali. Lo studente utilizza il sito come punto di partenza per approfondire un determinato argomento, consultando sia la sintesi divulgativa sia le fonti scientifiche originali.

**Scenario d'uso.** Durante la preparazione di una relazione o di un progetto universitario, lo studente utilizza il sito per orientarsi rapidamente nella letteratura scientifica disponibile.



- **Divulgatore o comunicatore scientifico**


Il terzo destinatario è un divulgatore scientifico, un blogger o un professionista della comunicazione che desidera produrre contenuti accurati e aggiornati. Oltre alla sintesi degli articoli, il sito mette a disposizione uno *social media snippet* per ogni contenuto, facilitando la promozione degli articoli attraverso piattaforme social.

**Scenario d'uso.** Dopo aver letto un articolo, il divulgatore può condividere rapidamente il relativo snippet sui social media, rimandando gli utenti alla versione completa pubblicata sul sito.

La struttura del prodotto editoriale è stata progettata tenendo conto delle esigenze comuni di queste categorie di utenti: navigazione semplice, contenuti organizzati in articoli indipendenti, linguaggio divulgativo ma rigoroso e possibilità di accedere direttamente alle fonti scientifiche originali.


### Requisiti di accettazione


Per garantire che il prodotto editoriale soddisfi gli obiettivi definiti e le necessità dei destinatari individuati, ho stabilito una serie di requisiti funzionali e non funzionali.

Dal punto di vista della fruizione dei contenuti, il prodotto deve garantire una struttura chiara e facilmente navigabile, permettendo agli utenti di accedere rapidamente ai diversi articoli e di individuare le informazioni di interesse. Per questo motivo il sito è stato organizzato in una struttura multi-pagina con una navigazione coerente tra gli articoli.

Un requisito fondamentale riguarda l'affidabilità delle informazioni. Ogni articolo deve essere basato su fonti scientifiche verificabili e, quando possibile, pubblicate con licenza open access. I contenuti devono essere sintetizzati attraverso un linguaggio divulgativo, mantenendo comunque un adeguato livello di accuratezza scientifica.

Dal punto di vista del processo editoriale, il sistema deve permettere aggiornamenti semplici e frequenti. L'utilizzo di Markdown come formato sorgente consente di modificare o aggiungere contenuti senza intervenire direttamente sul codice HTML generato. La struttura modulare permette inoltre di estendere il progetto con nuovi articoli mantenendo la stessa organizzazione.

I principali requisiti di accettazione individuati sono:

- **Navigabilità:** il sito deve offrire una struttura chiara con sezioni e articoli facilmente raggiungibili.
- **Aggiornabilità:** nuovi contenuti devono poter essere aggiunti o modificati rapidamente attraverso file Markdown.
- **Coerenza grafica:** tutte le pagine devono mantenere lo stesso stile editoriale e la stessa struttura.
- **Accessibilità delle fonti:** ogni articolo deve includere riferimenti agli studi scientifici utilizzati.
- **Distribuzione digitale:** il prodotto deve essere pubblicabile sul web attraverso un processo automatizzato.
- **Riutilizzabilità dei contenuti:** gli articoli devono poter essere adattati anche per altri canali digitali, come newsletter o social media, grazie alla presenza di elementi dedicati alla condivisione.

Per quanto riguarda gli standard adottati, il progetto utilizza tecnologie consolidate nell'ambito della pubblicazione digitale: Markdown come formato strutturato dei contenuti, HTML come formato finale di distribuzione e Git come sistema di controllo versione. L'approccio scelto permette di combinare semplicità di gestione editoriale e possibilità di automazione del processo produttivo.



### Canali di distribuzione



Il prodotto editoriale è stato progettato principalmente per la distribuzione tramite il canale web, con l'obiettivo di fornire un ambiente facilmente accessibile e aggiornabile per la consultazione degli articoli.

Il canale di distribuzione principale è rappresentato dal sito web statico pubblicato tramite **GitHub Pages**. Questa soluzione permette di rendere il contenuto disponibile pubblicamente attraverso un indirizzo web, garantendo allo stesso tempo un processo di aggiornamento semplice grazie all'integrazione con il sistema di versionamento Git.

Il formato sorgente adottato per la produzione dei contenuti è **Markdown**, un formato leggero e strutturato particolarmente adatto alla scrittura editoriale. I file Markdown vengono successivamente trasformati automaticamente in pagine HTML attraverso il framework **MkDocs**, permettendo di separare la fase di produzione dei contenuti dalla fase di presentazione grafica.

La struttura del prodotto è compatibile con diversi scenari di distribuzione digitale:

- **Web:** il sito rappresenta il canale principale, ottimizzato per la lettura online attraverso dispositivi desktop e mobile.
- **Newsletter o blog:** la struttura degli articoli permette un eventuale riutilizzo dei contenuti all'interno di piattaforme editoriali differenti.
- **Social media:** ogni articolo include uno *social media snippet*, ovvero un breve testo riassuntivo pensato per facilitare la condivisione sui social network e indirizzare gli utenti verso il contenuto completo.

Dal punto di vista dell'identità visiva, il progetto è stato sviluppato prendendo ispirazione dalle moderne piattaforme di pubblicazione digitale, in particolare dal modello editoriale adottato da **Substack**, caratterizzato da un'esperienza di lettura focalizzata sul contenuto, una struttura semplice e una forte attenzione alla leggibilità degli articoli.

L'obiettivo è stato ricreare un ambiente simile a una newsletter digitale scientifica, mantenendo però i vantaggi di un sito web strutturato. Per questo motivo sono state adottate alcune scelte stilistiche ispirate a tale modello:

- una colonna centrale ottimizzata per la lettura degli articoli;

- ampio spazio bianco per migliorare la leggibilità;

- utilizzo di font serif per il testo principale, richiamando lo stile editoriale tradizionale;

- gerarchia visiva chiara tra titoli, sezioni e corpo del testo;

- elementi grafici minimali per ridurre la distrazione durante la lettura.

Questa scelta mira a combinare l'affidabilità tipica della comunicazione scientifica con un'esperienza utente più vicina alle moderne piattaforme di divulgazione digitale, rendendo i contenuti più accessibili anche a lettori non specialisti.

## Processo di Produzione

### Aquisizione dei contenuti

Nel progetto sono stati selezionati quattro ambiti rappresentativi del fenomeno della disinformazione scientifica, ognuno analizzato attraverso articoli scientifici recenti.

Il primo articolo analizza il rapporto tra **intelligenza artificiale generativa e produzione automatizzata di disinformazione**. Lo studio di Vykopal et al. (2024), *Disinformation Capabilities of Large Language Models*, pubblicato negli atti della 62nd Annual Meeting of the Association for Computational Linguistics, esamina la capacità di diversi Large Language Models di generare contenuti falsi credibili e coerenti con narrative di disinformazione. La ricerca evidenzia come i modelli linguistici avanzati possano rappresentare un potenziale strumento per amplificare la produzione e diffusione di contenuti manipolativi.

Il secondo articolo affronta il tema della **disinformazione nel dibattito politico**. Lo studio di Domínguez-García, Velasco-Molpeceres e Pérez-Curiel (2024), *Disinformation in the Spanish public debate: an analysis of political speeches in the Congress of Deputies*, analizza il ruolo della comunicazione politica nella diffusione di informazioni fuorvianti, attraverso lo studio dei discorsi parlamentari in Spagna.

Il terzo articolo riguarda la **disinformazione in ambito sanitario**. La ricerca di Aleksandric et al. (2022), *The impact of social media misinformation on public health interventions*, analizza gli effetti della diffusione di informazioni errate sui social media rispetto agli interventi di salute pubblica, evidenziando come la disinformazione possa influenzare comportamenti individuali e collettivi.

Infine, il quarto articolo esplora le possibilità offerte dall'**intelligenza artificiale nel contrasto alla disinformazione**. Lo studio di Pilati e Venturini (2025), *The use of artificial intelligence in counter-disinformation: a world wide (web) mapping*, analizza l'utilizzo di tecniche di intelligenza artificiale per identificare, monitorare e contrastare fenomeni di manipolazione informativa online.

La selezione di questi contributi permette quindi di rappresentare il fenomeno della disinformazione da prospettive complementari: la generazione automatica tramite AI, la dimensione politica, l'impatto sulla salute pubblica e le strategie tecnologiche di contrasto.


### Gestione documentale

Il flusso di gestione documentale adottato per questo progetto segue sette fasi principali, dalla selezione della fonte scientifica fino alla pubblicazione multi-canale.

**(i) Raccolta dei contenuti**
La fonte primaria di ogni articolo è un paper scientifico peer-reviewed, recente e ad accesso aperto, individuato tramite ricerca mirata (Google Scholar e verifica diretta su repository come ACL Anthology, Frontiers, PubMed Central). Per ciascun tema editoriale (intelligenza artificiale, disinformazione politica, salute pubblica, counter-disinformation) è stato selezionato un paper rappresentativo dell'argomento.

**(ii) Valutazione dei diritti**
Ogni fonte è stata verificata per la licenza di distribuzione prima dell'utilizzo: tutti i paper selezionati sono pubblicati con licenza Creative Commons Attribution (CC BY), che ne consente la libera consultazione, la sintesi divulgativa e la citazione con link diretto.

**(iii) Trasformazione dei formati**
Il contenuto sorgente (PDF accademico, spesso strutturato secondo il formato IMRaD) è stato trasformato in prosa giornalistica in formato Markdown, il formato intermedio scelto per la sua portabilità: lo stesso file `.md` alimenta sia la pubblicazione web (tramite MkDocs) sia il riutilizzo diretto su blog e newsletter, senza necessità di riconversioni.

**(iv) Strutturazione dei contenuti**
Ogni articolo segue una struttura fissa e ripetibile: titolo giornalistico, introduzione contestuale, sintesi divulgativa dei risultati della ricerca, sezione "perché interessa a chi fa informazione", citazione della fonte con link diretto, e infine uno snippet ottimizzato per la condivisione social. Questa struttura standardizzata rende il processo scalabile a nuovi temi.

**(v) Applicazione dello stile grafico**
Lo stile visivo del sito è stato definito tramite il tema MkDocs Material, personalizzato con un foglio di stile CSS dedicato (`substack.css`) che riproduce l'estetica di una newsletter editoriale (font serif per il corpo del testo, colonna di lettura stretta, header minimale), distinguendolo dal tema di documentazione tecnica di default.

**(vi) Generazione dei metadati**
Ogni articolo include metadati editoriali minimi ma essenziali per un formato blog/newsletter: data di pubblicazione visibile, titolo, e struttura di navigazione definita nel file di configurazione `mkdocs.yml`, che genera automaticamente il menu e l'indice del sito.

**(vii) Distribuzione dei contenuti**
La distribuzione avviene attraverso una pipeline automatizzata: ogni modifica ai file sorgente Markdown, anche effettuata direttamente dall'interfaccia web di GitHub, attiva un workflow di GitHub Actions che compila il sito con MkDocs e lo pubblica su GitHub Pages, rendendo il processo di aggiornamento immediato (1-2 minuti) e senza necessità di intervento manuale da terminale.

**Fasi di revisione e controllo**
Il controllo qualità è stato realizzato in due momenti: (a) verifica del rispetto dei limiti di sintesi e parafrasi rispetto alla fonte originale, per garantire un uso corretto del materiale protetto da copyright anche in presenza di licenza aperta; (b) verifica tecnica del deploy tramite il log del workflow GitHub Actions, che segnala esplicitamente eventuali errori di build prima della pubblicazione, fungendo da controllo di approvazione automatico prima che il contenuto raggiunga il sito pubblico.




\begin{figure}[H]
\centering
\includegraphics[width=\textwidth]{./logo/mermaid2.png}
\caption{Flusso di produzione documentale}
\end{figure}






### Tecnologie adottate


Per la realizzazione del prodotto editoriale sono state adottate diverse tecnologie con l'obiettivo di creare un flusso di produzione semplice, riproducibile e facilmente aggiornabile. Le tecnologie utilizzate coprono le diverse fasi del processo, dalla gestione dei contenuti alla generazione del sito web finale e alla distribuzione online.

**Markdown**

Il formato principale utilizzato per la produzione dei contenuti è **Markdown**. Questa tecnologia è stata scelta come formato sorgente degli articoli perché permette di separare il contenuto dalla presentazione grafica, rendendo più semplice la scrittura, modifica e aggiornamento degli articoli.

Ogni articolo è memorizzato come file Markdown indipendente, permettendo di aggiungere nuovi contenuti senza modificare la struttura generale del sito. Questo approccio risponde alle esigenze dei destinatari individuati, in particolare giornalisti e comunicatori scientifici, che possono aggiornare rapidamente il prodotto editoriale concentrandosi sul contenuto.

**MkDocs**

Il framework utilizzato per la trasformazione dei contenuti Markdown in un sito web statico è **MkDocs**. Questo strumento automatizza il processo di generazione delle pagine HTML, mantenendo separata la fase editoriale dalla fase di pubblicazione.

La configurazione del sito è definita attraverso il file `mkdocs.yml`, nel quale vengono specificati il titolo del progetto, la struttura di navigazione, il tema grafico e le personalizzazioni. Questa soluzione permette di mantenere una struttura coerente tra tutti gli articoli e facilita l'estensione futura del prodotto.

**Material for MkDocs e personalizzazione grafica**

Per la presentazione dei contenuti è stato adottato il tema **Material for MkDocs**, successivamente personalizzato tramite CSS.

La personalizzazione grafica è stata sviluppata con l'obiettivo di creare un'esperienza di lettura simile alle piattaforme editoriali digitali moderne, in particolare ispirata al modello di **Substack**. Sono stati modificati elementi come tipografia, spaziatura, layout della colonna principale e stile dei collegamenti, con particolare attenzione alla leggibilità degli articoli.

Questa scelta contribuisce al raggiungimento degli scenari d'uso perché permette agli utenti di concentrarsi sul contenuto scientifico senza una struttura grafica complessa o dispersiva.

**Git e GitHub**

Il controllo del progetto è stato gestito attraverso **Git**, utilizzato come sistema di versionamento dei file sorgente. La repository GitHub contiene i contenuti Markdown, la configurazione del sito e gli elementi necessari alla riproduzione del processo produttivo.

L'utilizzo di Git permette di mantenere uno storico delle modifiche, facilitare la revisione dei contenuti e collaborare eventualmente con altri autori o redattori.

**GitHub Pages e automazione del deploy**

La distribuzione finale del prodotto avviene tramite **GitHub Pages**, che permette di pubblicare gratuitamente il sito web statico generato da MkDocs.

Il processo di pubblicazione può essere automatizzato tramite GitHub Actions: a seguito di un aggiornamento della repository, il sistema può generare automaticamente il sito e pubblicare la nuova versione online. Questa soluzione riduce le operazioni manuali necessarie e rende il prodotto adatto a un processo editoriale aggiornabile nel tempo.

Nel complesso, l'insieme delle tecnologie adottate permette di realizzare un flusso editoriale leggero ma completo, in cui la produzione dei contenuti, la gestione della struttura, l'applicazione dello stile grafico e la distribuzione finale risultano integrate in un unico processo riproducibile.

### Esecuzione del flusso
Il repository documentale del progetto è disponibile pubblicamente all'indirizzo:

**Repository**: [github.com/danieledelpozzo/editoria](https://github.com/danieledelpozzo/editoria)

**Sito pubblicato**: [danieledelpozzo.github.io/editoria](https://danieledelpozzo.github.io/editoria/)

Il repository contiene tutti i materiali necessari a riprodurre integralmente il flusso di produzione documentale descritto in questo documento:

\begin{figure}[H]
\centering
\includegraphics[width=\textwidth]{./logo/repo.png}
\caption{Struttura della repository GitHub}
\end{figure}

Per ciascuno dei quattro temi editoriali previsti (intelligenza artificiale, disinformazione politica, salute pubblica, contrasto alla disinformazione tramite IA) è stato prodotto un prototipo completo e pubblicato, a dimostrazione della riproducibilità del flusso su temi diversi. La struttura è pensata per essere facilmente estesa a nuovi temi: è sufficiente aggiungere un nuovo file Markdown seguendo il formato già stabilito e referenziarlo nella sezione `nav` di `mkdocs.yml`, senza modificare il resto della configurazione.

La riproducibilità del flusso è garantita dall'automazione della pubblicazione: ogni modifica ai contenuti in `docs/` innesca automaticamente, tramite GitHub Actions, la rigenerazione e la pubblicazione del sito su GitHub Pages, senza richiedere strumenti installati localmente da parte di chi aggiorna i contenuti.

### Utilizzo di intelligenza artificiale generativa

L'intelligenza artificiale generativa è stata integrata in alcune fasi del flusso di gestione documentale come strumento di supporto alla produzione editoriale, con l'obiettivo di ridurre i tempi di elaborazione dei contenuti e migliorare la qualità della comunicazione scientifica.

L'AI non è stata utilizzata come sostituto del processo di selezione e verifica delle fonti, ma come strumento di assistenza nelle attività redazionali che richiedono rielaborazione linguistica e organizzazione delle informazioni.

### Fasi di utilizzo dell'AI generativa
| Fase del flusso | Applicazione dell'AI generativa | Obiettivo |
|-----------------|----------------------------------|-----------|
| Analisi delle fonti | Supporto nella comprensione degli articoli scientifici e nell'individuazione dei concetti principali. | Accelerare l'analisi di pubblicazioni scientifiche complesse. |
| Produzione dei contenuti | Supporto nella sintesi e nella riformulazione dei contenuti scientifici in linguaggio divulgativo. | Rendere le informazioni accessibili a giornalisti e comunicatori non specialisti. |
| Revisione editoriale | Controllo della struttura dei testi, chiarezza espositiva e coerenza dello stile. | Migliorare leggibilità e qualità comunicativa degli articoli. |
| Progettazione del prodotto digitale | Supporto nell'organizzazione della struttura del sito e nella definizione delle soluzioni grafiche. | Creare un prodotto editoriale coerente con modelli digitali moderni. |

### Approccio di prompt engineering

L'utilizzo dell'AI è stato basato su prompt strutturati con indicazioni specifiche riguardanti il ruolo da assumere, il pubblico di riferimento e il tipo di trasformazione richiesta.

In particolare, i prompt hanno richiesto di:

- adottare uno stile divulgativo rivolto a lettori non specialisti;

- mantenere fedeltà alle informazioni presenti nelle fonti scientifiche originali;

- evitare semplificazioni che potessero introdurre interpretazioni errate;

- organizzare le informazioni secondo una struttura adatta alla pubblicazione digitale.

### Validazione degli output generati

Gli output prodotti dall'intelligenza artificiale sono stati sottoposti a revisione manuale prima dell'integrazione nel prodotto finale.

La verifica ha riguardato principalmente:

- correttezza delle informazioni scientifiche rispetto agli articoli originali;

- assenza di modifiche del significato delle fonti;

- chiarezza del linguaggio utilizzato;

- coerenza con l'obiettivo di contrastare la disinformazione attraverso informazioni affidabili.

### Valutazione del contributo dell'AI

L'utilizzo dell'intelligenza artificiale generativa ha permesso una riduzione dei tempi nelle attività di analisi, rielaborazione e revisione dei contenuti. Inoltre, ha facilitato la trasformazione di materiali scientifici complessi in contenuti più accessibili per un pubblico editoriale.

Tuttavia, sono emersi alcuni limiti: l'AI può produrre sintesi incomplete o interpretazioni non corrette se non adeguatamente guidata e verificata. Per questo motivo il controllo umano rimane una fase fondamentale, soprattutto in un progetto dedicato alla comunicazione scientifica e al contrasto della disinformazione.

## Valutazione dei risultati raggiunti

### Valutazione del flusso di produzione

Il flusso di produzione realizzato ha permesso di integrare in un unico ambiente le diverse fasi necessarie alla creazione e distribuzione di un prodotto editoriale digitale: raccolta delle fonti, produzione dei contenuti, strutturazione dei documenti, applicazione dello stile grafico e pubblicazione online.

Dal punto di vista della gestione documentale sono stati ottenuti i seguenti risultati:

| Aspetto valutato | Risultato raggiunto |
|------------------|---------------------|
| Riduzione dei tempi di gestione documentale | L'utilizzo di Markdown come formato sorgente e MkDocs come sistema di generazione automatica ha ridotto il tempo necessario per aggiornare e pubblicare nuovi contenuti, evitando modifiche manuali alle pagine web. |
| Riduzione degli errori | La struttura standardizzata degli articoli e la configurazione centralizzata tramite `mkdocs.yml` riducono il rischio di incoerenze tra le diverse pagine del prodotto editoriale. |
| Miglioramento della qualità dei documenti | La separazione tra contenuto e presentazione permette di concentrarsi maggiormente sulla qualità editoriale, mentre il tema Material for MkDocs e il CSS personalizzato garantiscono una presentazione coerente. |
| Miglioramento dell'accettazione della tecnologia | L'utilizzo di strumenti diffusi e accessibili come Markdown, Git e MkDocs rende il flusso facilmente comprensibile e replicabile anche da utenti con competenze tecniche limitate. |
| Nuovi canali di distribuzione | La pubblicazione tramite GitHub Pages permette di distribuire il prodotto tramite il web, rendendo gli articoli facilmente accessibili e condivisibili. |
| Soddisfacimento degli scenari d'uso | Il prodotto risponde alle esigenze di giornalisti e comunicatori scientifici fornendo contenuti sintetici, aggiornabili e basati su fonti scientifiche verificabili. |

### Confronto con lo stato dell'arte

Il confronto tra un processo tradizionale (AS-IS) e il flusso proposto (TO-BE) evidenzia i vantaggi introdotti dalle tecnologie adottate.

| Aspetto | AS-IS | TO-BE |
|---------|-------|--------|
| Produzione | Aggiornamento manuale delle pagine. | File Markdown modulari. |
| Struttura | Layout HTML modificato manualmente. | Generazione automatica con MkDocs. |
| Stile grafico | Coerenza gestita manualmente. | Tema e CSS centralizzati. |
| Pubblicazione | Caricamento manuale. | Deploy automatico con GitHub Actions. |
| Collaborazione | Storico modifiche limitato. | Versionamento con Git. |

Il flusso proposto migliora quindi la scalabilità del processo editoriale, permettendo di aggiungere nuovi articoli mantenendo la stessa struttura e identità visiva.

### Limiti emersi

Nonostante i risultati raggiunti, il progetto presenta alcuni limiti.

Un primo limite riguarda il livello di automazione: la selezione delle fonti scientifiche, la valutazione della qualità degli articoli e la verifica delle informazioni rimangono attività che richiedono un intervento umano. Questo aspetto è particolarmente rilevante in un progetto dedicato alla disinformazione, dove l'affidabilità delle fonti rappresenta un requisito fondamentale.

Un secondo limite riguarda la trasformazione automatica dei contenuti: strumenti come MkDocs semplificano la pubblicazione web, ma non gestiscono automaticamente tutti i possibili formati editoriali (ad esempio ePub o versioni ottimizzate per social media), che richiederebbero ulteriori processi di conversione.

Infine, l'utilizzo dell'intelligenza artificiale generativa, pur offrendo vantaggi nella sintesi e revisione dei contenuti, richiede sempre una fase di controllo umano per evitare errori, semplificazioni e interpretazioni non corrette.

## Conclusioni

Il progetto ha raggiunto gli obiettivi iniziali attraverso la realizzazione di un prodotto editoriale digitale dedicato alla comunicazione scientifica e al contrasto della disinformazione.

La combinazione di Markdown, MkDocs, Material for MkDocs, Git e GitHub Pages ha permesso di creare un flusso produttivo leggero, riproducibile e facilmente aggiornabile. La scelta di un'interfaccia ispirata a piattaforme editoriali digitali come Substack ha inoltre contribuito a migliorare la leggibilità e l'esperienza di fruizione dei contenuti.

Gli aspetti maggiormente soddisfacenti riguardano la separazione tra contenuto e presentazione, la semplicità di aggiornamento degli articoli e la possibilità di distribuire rapidamente nuovi contenuti online.

Le principali limitazioni emerse riguardano invece la necessità di mantenere un controllo umano sulle fasi editoriali più delicate e la mancanza di una completa automazione della pipeline, soprattutto per quanto riguarda la selezione delle fonti e la generazione di formati multipli.

Nel complesso, il progetto dimostra come strumenti digitali aperti e facilmente accessibili possano supportare un processo editoriale scientifico più efficiente, trasparente e scalabile.





## Bibliografia e sitografia

I quattro articoli editoriali pubblicati nel sito si basano sui seguenti paper scientifici open access: [@vykopal-etal-2024-disinformation; @dominguez-garcia2024disinformation; @aleksandric2022impact; @pilati2025counter].