---
############################# Static ############################
layout: "landing"
date: 2024-07-03T19:47:25
draft: false

lang: fr
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Bibliothèque de recherche et d'indexation de texte pour documents, PDF, Office et Web"
head_description: "Solution de recherche de texte avancée pour les applications Node.js permettant de rechercher, d'indexer et de collecter des données à partir de documents : PDF, Word, Excel, présentations, formats de fichiers de courrier électronique et Web."

############################# Header ############################
title: "Rechercher et indexer des documents à l'aide de l'API Node.js"
description: "Améliorez les applications Node.js en implémentant la recherche de texte dans tous les formats de documents populaires."
words:
  for: "pour"

actions:
  main: "Téléchargement gratuit de NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licence"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Prêt à commencer?"
  description: "Essayez GroupDocs.Search fonctionnalités gratuitement ou demandez une licence"

release:
  title: "Version {0} publiée"
  notes: "Regardez ce qu'il y a de nouveau"
  downloads: "Téléchargements"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Rechercher dans le dossier avec JavaScript"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // Création d'un index
    var index = new Index("c:\\MyIndex");

    // Ajout de documents à l'index
    index.addToIndex("c:\\MyDocuments");
    
    // Recherche de différents mots comme
    // 'affect', 'effect', 'principles', 'principally'
    var results = index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search en un coup d'oeil"
  description: "Bibliothèque Node.js JavaScript pour la recherche de texte"
  features:
    # feature loop
    - title: "Node.js Opérations d'indexation et de recherche"
      content: "L'indexation dans GroupDocs.Search for Node.js via Java collecte, stocke et analyse les données pour des opérations de recherche précises et efficaces. Ces index sont fréquemment utilisés pour effectuer des recherches."

    # feature loop
    - title: "Fusionner plusieurs index pour améliorer l'efficacité de la recherche"
      content: "L'API GroupDocs.Search for Node.js via Java permet la fusion de plusieurs index en un seul. Des modifications fréquentes créent plusieurs index delta, ce qui peut ralentir les performances de recherche. Notre solution fusionne ces index delta en un index commun, contenant toutes les informations des index delta fusionnés, améliorant considérablement l'efficacité de la recherche tout en gardant les index delta inchangés. Diverses fonctionnalités peuvent être configurées pour affiner ce processus."

    # feature loop
    - title: "Reconnaître les requêtes de recherche à partir de différentes dispositions de clavier"
      content: "GroupDocs.Search for Node.js via Java reconnaît les requêtes de recherche qui ne correspondent pas à la disposition du clavier. Actuellement, 88 langues et 164 configurations de clavier différentes sont prises en charge."

    # feature loop
    - title: "Recherche à l'aide de formes de mots morphologiques"
      content: "Avec GroupDocs.Search for Node.js via Java, vous pouvez rechercher diverses formes de mots, telles que des noms au singulier et au pluriel, ou toutes les formes d'un verbe. Les langues anglaises et non anglaises peuvent être personnalisées pour des formes de mots spécifiques."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Search for Node.js via Java prend en charge tous les systèmes d'exploitation et gestionnaires de packages courants."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Search for Node.js via Java permet de traiter un large éventail de formats de fichiers. [Explorez la liste complète](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
        ### Formats multimédias
        * **Formats d'images populaires:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Images multipages:** GIF, WEBP, TIFF
        * **l'audio:** MP3, WAV
        * **Vidéo:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Autre
        * **E-mail:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **la toile:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Autres:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java Fonctionnalités"
  description: "Contrôlez le contenu des documents professionnels à l'aide de notre moteur de recherche avancé, prenant en charge les formats de fichiers les plus courants, notamment PDF, DOCX, XLSX, PPTX, etc."

  items:
    # feature loop
    - icon: "document_info"
      title: "Paramètres flexibles"
      content: "Utiliser la plage de dates et la sensibilité à la casse comme paramètres de recherche"

    # feature loop
    - icon: "detect"
      title: "Recherche de vérification orthographique"
      content: "Utilisez des expressions de recherche avec la vérification orthographique et les caractères génériques et ignorez les caractères spéciaux dans les requêtes"

    # feature loop
    - icon: "collect"
      title: "Filtrage des résultats"
      content: "Configurer le filtrage des documents dans les résultats de recherche"

    # feature loop
    - icon: "get"
      title: "Importer / Exporter"
      content: "Effectuer une importation ou utiliser une liste pour modifier des caractères lors de l'indexation et de l'exportation vers un fichier"

    # feature loop
    - icon: "remove"
      title: "Ignorer les données inutiles"
      content: "Ignorer sélectivement l'indexation de fichiers spécifiques et ignorer des mots spécifiques pour indexer plus rapidement"

    # feature loop
    - icon: "style"
      title: "Traitement des URL"
      content: "Extrayez le texte au format HTML dans un fichier et générez une URL pour parcourir les résultats de recherche en HTML"

    # feature loop
    - icon: "detect"
      title: "Recherche rapide"
      content: "Divisez la recherche en morceaux plus petits pour rechercher rapidement des index volumineux"

    # feature loop
    - icon: "manipulate"
      title: "Traitement des flux"
      content: "Indexer des documents à partir de flux et de structures de données"

    # feature loop
    - icon: "compare"
      title: "Gérer les fautes d’orthographe"
      content: "Activer le nombre exact d'occurrences pour chaque mot trouvé afin de proposer des suggestions de mots alternatifs en cas de faute d'orthographe"

    # feature loop
    - icon: "unreadable_characters"
      title: "Prise en charge des archives"
      content: "Indexer les archives compressées dans d'autres archives ZIP et récupérer la liste des fichiers indexés dans une archive"

    # feature loop
    - icon: "hidden_print"
      title: "Économie d'espace disque"
      content: "Économisez de l'espace avec l'indexation compacte et l'indexation des documents sécurisés par mot de passe"

    # feature loop
    - icon: "style"
      title: "Synonymes personnalisés"
      content: "Ajouter des synonymes anglais au dictionnaire de synonymes par défaut"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de codes"
  description: "Explorez les fonctionnalités de GroupDocs.Search for Node.js via Java avec des exemples"
  items:
    # code sample loop
    - title: "Utiliser la recherche floue pour améliorer la productivité"
      content: |
        Profitez de la fonctionnalité flexible GroupDocs.Search for Node.js via Java pour améliorer le contrôle du contenu des documents grâce à des algorithmes de recherche sophistiqués. [En savoir plus](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Comment traiter le résultat de la recherche">}}
        ```javascript {style=abap}
        // Créer un index
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");

        // Configurer les options de recherche
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Rechercher des documents contenant le mot « eau » ou l'expression « Lorem ipsum »
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // Résultat de la recherche de processus
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Les expressions régulières sont disponibles pour les scénarios de recherche avancée"
      content: |
        GroupDocs.Search for Node.js via Java nous permet d'utiliser des expressions régulières afin d'affiner les résultats de recherche. [Plongez dans les techniques de recherche avancées](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Comment effectuer une recherche à l'aide d'expressions régulières">}}
        ```javascript {style=abap}   
        // Créer un index
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");
 
        // Rechercher l'expression sous forme de texte

        // Le premier caractère caret au début indique qu'il s'agit d'une requête de recherche d'expression régulière
        var query = "^^(.)\\1{1,}";
        // Rechercher deux ou plusieurs caractères identiques au début d'un mot
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
