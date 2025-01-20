---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: it

############################# Head ############################
head_title: "Ricerca e indicizzazione del testo dei documenti | API e Web App gratuite"
head_description: "Esegui ricerche di testo e indicizzazione dei dati in PDF, MS Office, OpenDocument e altri formati di file popolari utilizzando le nostre API o l'app gratuita per la ricerca dei documenti."

############################# Header ############################
title: "Soluzione completa per la ricerca e l'indicizzazione dei documenti"
description:  |
  Esegui ricerche di testo e indicizzazione su PDF, Microsoft Office, OpenOffice e molti altri formati di file documentali.

  Trova rapidamente informazioni in ampie collezioni di documenti con avanzate capacità di ricerca full-text.

  Personalizza le funzionalità di ricerca come sinonimi, ricerca fuzzy e stemming per migliorare l'accuratezza e i risultati.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Scegli la tua piattaforma"
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Search è compatibile con i seguenti sistemi operativi e framework:"
  details_link_title: "Scopri di più"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualsiasi altro editor di testo
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Caratteristiche principali di GroupDocs.Search"
  description: "GroupDocs.Search offre strumenti potenti per indicizzare e ricercare testo in formati di documenti popolari. Semplifica e migliora la gestione dei documenti con funzionalità di ricerca avanzate."

  items:
    # items loop
    - icon: "view"
      title: "Ricerca testuale avanzata"
      content: "Esegui ricerche di testo rapide e accurate su documenti indicizzati."

    # items loop
    - icon: "manipulate"
      title: "Opzioni di ricerca personalizzabili"
      content: "Utilizza funzionalità come ricerca fuzzy, sinonimi e stemming per risultati più precisi."

    # items loop
    - icon: "merge"
      title: "Supporto per più formati"
      content: "Indicizza e cerca contenuti in Microsoft Office, PDF, OpenOffice e altri formati comuni."

    # items loop
    - icon: "additional"
      title: "Indicizzazione efficiente"
      content: "Crea e mantieni rapidamente indici per ampie collezioni di documenti."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ricerca di testo in formati di documenti popolari"
  description: "GroupDocs.Search esempi di codice"
  items:
    # code sample loop
    - title: "Ricerca di testo"
      content: |
       GroupDocs.Search è uno strumento potente per trovare testo nei documenti. Puoi cercare attraverso più documenti in vari formati memorizzati in una cartella specifica. I risultati della ricerca vengono salvati in una cartella separata, consentendoti di accedervi e riutilizzarli senza dover eseguire nuovamente la ricerca.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Crea un'istanza della classe Index, specificando la cartella per memorizzare gli indici.
            Index index = new Index("\\Index Folder");

            //Specifica il percorso ai documenti in cui verrà eseguita la ricerca.
            index.Add("\\Documents Folder");

            //Crea un'istanza dell'oggetto SearchOptions.
            SearchOptions options = new SearchOptions();

            //Esegui la ricerca per il testo desiderato.
            SearchResult result = index.Search("ipsum dolor", options);

            //Gestisci e elabora i risultati della ricerca.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Crea un'istanza della classe Index, specificando la cartella per memorizzare gli indici.
            Index index = new Index("\\Index Folder");

            //Specifica il percorso ai documenti in cui verrà eseguita la ricerca.
            index.add("\\Documents Folder");

            //Crea un'istanza dell'oggetto SearchOptions.
            SearchOptions options = new SearchOptions();

            //Esegui la ricerca per il testo desiderato.
            SearchResult result = index.search("ipsum dolor", options);

            //Gestisci e elabora i risultati della ricerca.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Crea un'istanza della classe Index, specificando la cartella per memorizzare gli indici.
            const index = new searchLib.Index('\\Index Folder');

            //Specifica il percorso ai documenti in cui verrà eseguita la ricerca.
            index.add('\\Documents Folder');

            //Crea un'istanza dell'oggetto SearchOptions.
            const options = new searchLib.SearchOptions();

            //Esegui la ricerca per il testo desiderato.
            const result = index.search('ipsum dolor', options);

            //Gestisci e elabora i risultati della ricerca.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Supporta oltre 70 formati di file"
  description: "GroupDocs.Search supporta quasi tutti i formati di file ampiamente utilizzati."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistiche del nostro prodotto"
  description: "Scopri le metriche chiave che mostrano le nostre prestazioni, portata e crescita."

  items:
    # items loop
    - number: "70+"
      title: "Formati supportati"
      content: "Forniamo compatibilità con oltre 70 formati di documenti popolari."

    # items loop
    - number: "500k"
      title: "Download NuGet"
      content: "GroupDocs.Search per .NET è stato scaricato più di 500.000 volte su NuGet."

    # items loop
    - number: "12k"
      title: "Download Maven"
      content: "Gli sviluppatori Java hanno scaricato GroupDocs.Search oltre 12.000 volte da Maven."

    # items loop
    - number: "150+"
      title: "Clienti soddisfatti"
      content: "Sviluppatori e aziende leader in tutto il mondo si affidano ai nostri prodotti per soluzioni innovative."


############################# Customers ###############################
customers:
  enable: true
  title: "I nostri clienti soddisfatti"
  description: "Le librerie GroupDocs sono fidate da marchi e organizzazioni leader a livello mondiale."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Inizia il tuo viaggio oggi!"
  description: "Sperimenta GroupDocs.Search gratuitamente sulla tua piattaforma preferita."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Domande frequenti"
  description: "Trova risposte a domande comuni su GroupDocs.Search."

  items:
    # items loop
    - question: "Richiede GroupDocs.Search strumenti esterni per cercare documenti?"
      answer: "No, GroupDocs.Search funziona come soluzione autonoma e non necessita di strumenti o software aggiuntivi come Adobe Acrobat o Microsoft Office per eseguire ricerche."

    # items loop
    - question: "Posso testare GroupDocs.Search prima di acquistarlo?"
      answer: "Sì, puoi! GroupDocs.Search offre una prova gratuita. Puoi esplorare le sue funzionalità, anche se la versione di prova può includere limitazioni come filigrane o funzionalità restrittive. Per sbloccare tutte le funzionalità, puoi richiedere una licenza temporanea gratuita di 30 giorni. Scopri di più nella pagina [licenza temporanea](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quali opzioni di licenza sono disponibili?"
      answer: "Forniamo diversi modelli di licenza per GroupDocs.Search, adattati a diverse esigenze. Scegli una licenza in base alla dimensione del tuo team, allo scenario d'uso, o se hai bisogno dell'SDK/API per la distribuzione ai clienti. Per un uso flessibile, considera una licenza a consumo in cui paghi in base all'uso effettivo. Scopri di più sulle tue opzioni nella pagina [prezzi](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Web Apps"
  description: "Esplora GroupDocs.Search con la nostra applicazione web gratuita. Esegui ricerche di testo e indicizzazione su oltre 70 formati di file popolari direttamente nel tuo browser—completamente gratuito."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Cerca all'interno di PDF, Excel, Word, PowerPoint e altri tipi di file direttamente dal tuo browser."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Carica DOCX per eseguire ricerche di testo avanzate senza bisogno di installare software."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Metti alla prova le capacità di indicizzazione e recupero di PDF su vari formati gratuitamente."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---