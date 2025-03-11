
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: fr
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Rechercher PDF dans .NET en utilisant des opérateurs booléens"
head_description: "L'API GroupDocs.Search for .NET permet aux développeurs C# de rechercher le contenu des documents à l'aide d'opérateurs booléens tels que AND, OR et NOT."

############################# Header ############################
title: "Recherche textuelle de logique booléenne" 
description: "GroupDocs.Search for .NET facilite la création de requêtes de recherche avancées utilisant des opérateurs booléens (AND, OR, NOT) dans vos applications .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Search?"
    link: "/search/net/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) est une bibliothèque complète pour rechercher et indexer du texte dans des documents. Elle prend en charge plus de 70 formats de fichiers, tels que PDF, Word, PowerPoint, Excel, images et fichiers ZIP, permettant un traitement efficace de grandes quantités d'informations.

############################# Steps ############################
steps:
    enable: true
    title: "Comment rechercher le contenu d'un document PDF en utilisant la logique booléenne"
    content: |
      [GroupDocs.Search](/search/net/) rend la recherche du contenu d'un document PDF directe. Il fournit des conditions de recherche logique booléenne pour affiner les résultats dans les applications .NET.
      
      1. Spécifiez le dossier pour stocker l'index de recherche.
      2. Choisissez le dossier contenant les fichiers PDF.
      3. Exécutez la recherche et récupérez les résultats.
      4. Traitez les résultats.
   
    code:
      platform: "net"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Définir le chemin vers le dossier d'index
        Index index = new Index("c:/MyIndex");

        // Spécifiez le dossier contenant les documents à rechercher
        index.Add("c:/MyDocuments");

        // Exécuter une recherche à l'aide d'une requête complexe
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Découvrez des fonctionnalités avancées pour la recherche et l'indexation de documents"
  description: "La bibliothèque GroupDocs.Search for .NET simplifie la recherche et l'indexation de texte pour plus de 70 formats de fichiers. Localisez et gérez efficacement les informations avec des outils de recherche avancés."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Principales fonctionnalités de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de texte puissante"
      content: "Recherchez du texte à travers divers types de fichiers, y compris des PDF, des documents Word, des présentations PowerPoint et des tableurs. Utilisez des fonctionnalités telles que les correspondances exactes, les recherches floues et les jokers pour affiner les résultats."

    # feature loop
    - title: "Indexation de grandes quantités de données"
      content: "Créez et maintenez des index pour des recherches plus rapides. L'indexation structure et organise les données, facilitant ainsi la recherche dans d'importantes collections de documents."

    # feature loop
    - title: "Prise en charge de plusieurs langues"
      content: "Recherchez des documents en plus de 80 langues, avec un support pour différents types de claviers et formes morphologiques des mots afin d'améliorer la précision de la recherche."

    # feature loop
    - title: "Options de recherche personnalisables"
      content: "Ajustez les paramètres de recherche avec des fonctionnalités telles que la sensibilité à la casse, des filtres de plage de dates et la possibilité d'exclure des mots ou des données spécifiques lors de l'indexation."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilisation de requêtes de recherche booléennes avancées"
      content: |
        Cet exemple démontre comment appliquer des requêtes booléennes pour rechercher des documents PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Définir le dossier pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Spécifiez le chemin vers les documents à rechercher
          index.Add("c:/MyDocuments");

          // Créez une requête de recherche en utilisant la logique booléenne
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Récupérez les résultats de la recherche
          SearchResult result = index.Search(booleanQuery);
          
          // Traitez les résultats de recherche
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Copier"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pdf"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Search gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement de Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez les fonctionnalités clés"
    exclude: "boolean"
    description: "Explorez des fonctionnalités de recherche avancées et efficaces."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Rechercher à travers des formats de documents populaires"
    exclude: "PDF"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers. Personnalisez les règles de recherche et exploitez l'indexation pour économiser temps et effort."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---