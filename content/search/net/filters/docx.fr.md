
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: fr
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Recherche dans les documents DOCX avec .NET"
head_description: "GroupDocs.Search for .NET améliore les applications C# avec une recherche textuelle efficace à travers divers formats de documents commerciaux."

############################# Header ############################
title: "Rechercher du texte dans les documents commerciaux" 
description: "GroupDocs.Search for .NET permet des recherches textuelles puissantes et flexibles dans vos documents. Intégrez facilement la fonctionnalité de recherche dans les applications .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Téléchargez gratuitement"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Search?"
    link: "/search/net/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) est une bibliothèque puissante pour une recherche textuelle efficace et l'indexation de documents. Elle prend en charge plus de 70 formats de fichiers, y compris des documents à normes industrielles tels que PDF, Word, Excel et PowerPoint. Améliorez les performances de recherche avec des résultats rapides et précis.

############################# Steps ############################
steps:
    enable: true
    title: "Comment rechercher des données dans DOCX"
    content: |
      [GroupDocs.Search](/search/net/) permet des recherches textuelles efficaces dans les documents DOCX, ce qui le rend idéal pour les applications .NET.
      
      1. Configurez un dossier pour stocker l'index de recherche.
      2. Sélectionnez le dossier contenant vos fichiers.
      3. Configurez les options de recherche pour traiter uniquement les documents DOCX.
      4. Exécutez la recherche et récupérez les résultats.
   
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
        // Chemin pour stocker l'index de recherche réutilisable
        Index index = new Index("c:/MyIndex");

        // Dossier contenant des documents
        index.Add("c:/MyDocuments");

        // Rechercher uniquement dans des formats de fichiers spécifiques
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".docx");

        // Récupérer les résultats de recherche
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fonctionnalités avancées de recherche"
  description: "GroupDocs.Search for .NET permet des recherches textuelles sophistiquées à travers plus de 70 formats de fichiers. L'indexation améliore l'efficacité de la recherche et aide à gérer le contenu des documents de manière efficace."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Fonctionnalités principales de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche textuelle avancée"
      content: "Extraire du texte pertinent de documents commerciaux populaires, y compris des PDF, des fichiers Word, des présentations et des tableurs. Prend en charge plusieurs techniques de recherche telles que la recherche floue, la détection d'homophones et les caractères génériques."

    # feature loop
    - title: "Indexation optimisée pour des recherches plus rapides"
      content: "Créez et réutilisez des index de recherche pour améliorer la vitesse de recherche. L'indexation optimise les performances lors de la recherche à travers de grandes collections de documents."

    # feature loop
    - title: "Support pour plusieurs langues"
      content: "Effectuez des recherches dans des documents écrits en plus de 80 langues. Détecte différents claviers et variations de mots pour améliorer la précision."

    # feature loop
    - title: "Paramètres de recherche flexibles"
      content: "Affinez les résultats de recherche avec des options personnalisables, y compris des filtres, des expressions régulières et des paramètres de sensibilité à la casse."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrer les documents à traiter"
      content: |
        Apprenez à affiner les recherches de documents à l'aide de filtres
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Configurez un index qui exclut certains formats de fichiers
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Spécifiez le répertoire des documents
          index.Add("c:/MyDocuments");

          // Récupérez les résultats de recherche
          SearchResult result = index.Search("Lorem");
          
          // Traitez et utilisez le résultat de la recherche
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
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "Fonctionnalités clés"
    exclude: "filters"
    description: "Effectuez des recherches de données précises et efficaces."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Trouvez des données dans vos documents commerciaux"
    exclude: "DOCX"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers, permettant un traitement et une recherche efficaces de documents de bureau populaires."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---