---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: fr
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Solution de recherche et d'indexation de documents Java pour PDFs, fichiers de bureau et contenu web"
head_description: "Recherche de texte puissante et indexation pour les applications Java. Recherchez et organisez facilement des données dans des PDFs, Word, Excel, présentations, e-mails et formats web."

############################# Header ############################
title: "Recherche et indexation de documents efficaces avec l'API Java"
description: "Renforcez les applications Java avec des fonctionnalités de recherche de texte robustes à travers tous les formats de documents populaires."
words:
  for: "pour"

actions:
  main: "Téléchargez Maven gratuitement"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Commencez votre expérience dès aujourd'hui !"
  description: "Explorez les capacités de GroupDocs.Search gratuitement ou obtenez une licence pour débloquer son plein potentiel."

release:
  title: "Version {0} publiée"
  notes: "Voir les nouveautés"
  downloads: "Téléchargements"

code:
  title: "Trouver du texte dans des fichiers avec Java"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Créez un index pour vos documents
    Index index = new Index("c:/MyIndex");

    // Ajoutez des documents à l'index pour une recherche efficace
    index.add("c:/MyDocuments");
    
    // Recherchez des mots ou des phrases spécifiques, tels que
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Aperçu de GroupDocs.Search"
  description: "Découvrez les puissantes capacités de recherche de texte de la bibliothèque Java Java."
  features:
    # feature loop
    - title: "Opérations d'indexation et de recherche dans Java"
      content: "Avec GroupDocs.Search for Java, vous pouvez collecter, stocker et analyser des données de manière efficace pour créer des index détaillés pour des recherches plus rapides et plus précises."

    # feature loop
    - title: "Optimisez la recherche en fusionnant des index"
      content: "Combinez facilement plusieurs index avec GroupDocs.Search for Java pour rationaliser les recherches. Réduisez l'impact des petits index de delta en les consolidant en un seul index performant."

    # feature loop
    - title: "Support pour les mises en page de clavier multilingues"
      content: "Recherchez à travers différentes langues et mises en page de clavier avec GroupDocs.Search for Java. Il prend en charge 88 langues et 164 configurations de clavier pour une polyvalence inégalée."

    # feature loop
    - title: "Capacités de recherche morphologique"
      content: "Trouvez différentes formes de mots comme les noms singuliers/pluriels ou les variations verbales avec GroupDocs.Search for Java. Personnalisez les options de recherche pour l'anglais et d'autres langues."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Search for Java est compatible avec les principaux systèmes d'exploitation et gestionnaires de packages."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    Travaillez avec une large gamme de formats de fichiers en utilisant GroupDocs.Search for Java. [Consultez la liste complète](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formats de bureau populaires
        * **Portable:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Texte:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formats multimédia
        * **Formats d'image populaires:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Images multipages:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Vidéo:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Autres
        * **E-mail:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Autres:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Fonctionnalités de GroupDocs.Search for Java"
  description: "Gérez efficacement le contenu des documents avec des capacités de recherche avancées prenant en charge des formats tels que PDF, DOCX, XLSX, PPTX, et plus encore."

  items:
    # feature loop
    - icon: "document_info"
      title: "Paramètres de recherche personnalisables"
      content: "Affinez vos recherches en utilisant des plages de dates et des filtres de sensibilité à la casse."

    # feature loop
    - icon: "detect"
      title: "Vérification orthographique avancée"
      content: "Recherchez efficacement avec vérification orthographique, caractères génériques et en ignorant des caractères spéciaux."

    # feature loop
    - icon: "collect"
      title: "Résultats de recherche filtrés"
      content: "Appliquez des filtres pour affiner les résultats de recherche en fonction de types de documents spécifiques ou de critères."

    # feature loop
    - icon: "get"
      title: "Importation et exportation des données d'index"
      content: "Importez facilement des données pour l'indexation ou exportez les résultats vers des fichiers pour une utilisation ultérieure."

    # feature loop
    - icon: "remove"
      title: "Ignorer les fichiers non nécessaires"
      content: "Optimisez l'indexation en excluant des fichiers spécifiques ou des mots."

    # feature loop
    - icon: "style"
      title: "Traitement HTML et URL"
      content: "Extrayez le contenu HTML vers des fichiers et générez des URL pour naviguer dans les résultats de recherche."

    # feature loop
    - icon: "detect"
      title: "Recherche rapide dans de grands index"
      content: "Accélérez les opérations de recherche en divisant de grands index en morceaux gérables."

    # feature loop
    - icon: "manipulate"
      title: "Indexation basée sur des flux"
      content: "Indexez les données directement à partir de flux ou de structures de données."

    # feature loop
    - icon: "compare"
      title: "Gérer les requêtes mal orthographiées"
      content: "Détectez les fautes d'orthographe et suggérez des mots alternatifs pour une meilleure précision de recherche."

    # feature loop
    - icon: "unreadable_characters"
      title: "Support complet des archives"
      content: "Indexez les archives imbriquées et récupérez des listes détaillées de fichiers dans des fichiers ZIP."

    # feature loop
    - icon: "hidden_print"
      title: "Indexation économe en espace"
      content: "Compressez les index pour économiser de l'espace disque et traiter des fichiers protégés par mot de passe."

    # feature loop
    - icon: "style"
      title: "Support de synonymes personnalisés"
      content: "Étendez le dictionnaire de synonymes pour améliorer la précision des recherches avec des options personnalisées."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Essayez les fonctionnalités de GroupDocs.Search for Java avec ces exemples de code."
  items:
    # code sample loop
    - title: "Améliorez la précision de la recherche avec un matching flou"
      content: |
        Explorez la flexibilité de GroupDocs.Search for Java pour gérer le contenu avec des capacités avancées de recherche floue. [En savoir plus](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Comment traiter le résultat de la recherche">}}
        ```java {style=abap}
        // Créez un index
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Configurez les options de recherche
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Recherchez des documents contenant le mot 'eau' ou la phrase 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Traitez le résultat de la recherche
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Affinez les résultats avec des expressions régulières"
      content: |
        Utilisez des expressions régulières dans GroupDocs.Search for Java pour créer des résultats de recherche précis et détaillés. [Découvrez des techniques avancées](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Comment rechercher avec des expressions régulières">}}
        ```java {style=abap}   
        // Créez un index
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Recherchez la phrase sous forme de texte

        // Le premier caractère de caret au début indique qu'il s'agit d'une requête de recherche d'expressions régulières
        String query = "^^(.)\\1{1,}";
        // Recherchez deux caractères identiques ou plus au début d'un mot
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
