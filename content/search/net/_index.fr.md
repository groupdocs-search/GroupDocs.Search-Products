---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: fr
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: "Bibliothèque de recherche et d'indexation de documents .NET pour PDF, fichiers bureautiques et plus"
head_description: "Solution puissante .NET pour la recherche de texte et l'indexation dans des documents comme PDFs, Word, Excel, présentations, e-mails et formats web."

############################# Header ############################
title: "Recherche et indexation de documents avancées avec l'API .NET"
description: "Améliorez les applications .NET avec des capacités de recherche de texte à la pointe de l'industrie à travers des formats de documents populaires."
words:
  for: "pour"

actions:
  main: "Téléchargez Nuget gratuitement"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Commencez votre expérience dès aujourd'hui !"
  description: "Explorez les capacités de GroupDocs.Search gratuitement ou obtenez une licence pour débloquer son plein potentiel."

release:
  title: "Version {0} publiée"
  notes: "Voir les nouveautés"
  downloads: "Téléchargements"

code:
  title: "Rechercher du texte dans des fichiers d'annuaire"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Créez un index pour vos documents
    Index index = new Index("c:/MyIndex");

    // Ajoutez des documents à l'index pour une recherche efficace
    index.Add("c:/MyDocuments");
    
    // Recherchez des mots ou des phrases spécifiques, tels que
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Aperçu de GroupDocs.Search"
  description: "Découvrez la bibliothèque .NET C# pour une recherche et une indexation de texte robustes."
  features:
    # feature loop
    - title: "Fonctionnalités d’indexation et de recherche .NET"
      content: "Indexez, stockez et traitez efficacement les données documentaires avec GroupDocs.Search for .NET pour des opérations de recherche très précises et rapides."

    # feature loop
    - title: "Combiner les index pour une meilleure vitesse de recherche"
      content: "GroupDocs.Search for .NET vous permet de fusionner plusieurs index afin d'optimiser les performances. Réduisez l'impact des index de delta en les combinant en un index complet pour des recherches plus fluides."

    # feature loop
    - title: "Rechercher à travers différents formats de clavier"
      content: "Gérez facilement les requêtes de recherche à travers 88 langues et 164 mises en page de clavier grâce à la reconnaissance intelligente de GroupDocs.Search for .NET."

    # feature loop
    - title: "Recherche de mots morphologiques"
      content: "GroupDocs.Search for .NET prend en charge la recherche de variations de mots comme les noms singuliers/pluriels et les différentes formes verbales, personnalisables pour plusieurs langues."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Search for .NET fonctionne sans problème sur les principaux systèmes d'exploitation et gestionnaires de packages."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    Traitez une vaste gamme de formats de fichiers avec GroupDocs.Search for .NET. [Consultez tous les formats pris en charge](https://docs.groupdocs.com/search/net/supported-document-formats/).
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
  title: "Fonctionnalités clés de GroupDocs.Search for .NET"
  description: "Rationalisez la gestion des documents avec des capacités de recherche avancées dans des formats populaires tels que PDF, DOCX, XLSX, PPTX, et plus encore."

  items:
    # feature loop
    - icon: "document_info"
      title: "Paramètres de recherche flexibles"
      content: "Utilisez des filtres comme les plages de dates et la sensibilité à la casse pour affiner votre recherche."

    # feature loop
    - icon: "detect"
      title: "Vérification orthographique intelligente"
      content: "Recherchez des phrases avec correction orthographique, caractères génériques et caractères spéciaux ignorés."

    # feature loop
    - icon: "collect"
      title: "Résultats de recherche filtrés"
      content: "Personnalisez et filtrez les résultats de recherche par type de document ou critères."

    # feature loop
    - icon: "get"
      title: "Importation et exportation d'index"
      content: "Importez des données, modifiez les paramètres d'indexation et exportez les résultats indexés."

    # feature loop
    - icon: "remove"
      title: "Exclure les données non pertinentes"
      content: "Optimisez l'indexation en ignorant des fichiers spécifiques ou des mots."

    # feature loop
    - icon: "style"
      title: "Extraction d'URL"
      content: "Transformez le texte au format HTML en fichiers et générez des liens pour les résultats de recherche."

    # feature loop
    - icon: "detect"
      title: "Recherche à grande vitesse"
      content: "Divisez de grands index en parties plus petites pour un traitement plus rapide."

    # feature loop
    - icon: "manipulate"
      title: "Gestion des données rationalisée"
      content: "Indexez les documents directement à partir des flux de données et des structures."

    # feature loop
    - icon: "compare"
      title: "Détection de fautes d'orthographe"
      content: "Suggérez des mots alternatifs et suivez les occurrences pour améliorer la précision."

    # feature loop
    - icon: "unreadable_characters"
      title: "Support pour les archives"
      content: "Indexez les archives ZIP imbriquées et récupérez les détails des fichiers à l'intérieur."

    # feature loop
    - icon: "hidden_print"
      title: "Indexation efficace"
      content: "Économisez de l'espace disque avec une indexation compacte et traitez des documents protégés par mot de passe."

    # feature loop
    - icon: "style"
      title: "Synonymes personnalisés"
      content: "Ajoutez et gérez des synonymes pour des résultats de recherche sur mesure."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Découvrez les capacités puissantes de GroupDocs.Search for .NET avec des exemples pratiques."
  items:
    # code sample loop
    - title: "Améliorez votre productivité avec la recherche approximative"
      content: |
        Exploitez GroupDocs.Search for .NET pour un contrôle de contenu flexible et précis grâce à des algorithmes de recherche avancés. [Découvrez-en plus](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Comment traiter le résultat de la recherche">}}
        ```csharp {style=abap}
        // Créez un index
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Configurez les options de recherche
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Recherchez des documents contenant le mot 'eau' ou la phrase 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Traitez le résultat de la recherche
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Recherche avancée avec des expressions régulières"
      content: |
        GroupDocs.Search for .NET prend en charge les expressions régulières pour des recherches précises. [Apprenez des techniques avancées](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Comment rechercher avec des expressions régulières">}}
        ```csharp {style=abap}   
        // Créez un index
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Recherchez la phrase sous forme de texte

        // Le premier caractère de caret au début indique qu'il s'agit d'une requête de recherche d'expressions régulières
        string query = "^^(.)\\1{1,}";
        // Recherchez deux caractères identiques ou plus au début d'un mot
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
