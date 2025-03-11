
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: fr
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Recherche de documents PDF dans .NET avec GroupDocs.Search"
head_description: "Utilisez GroupDocs.Search for .NET pour effectuer des recherches textuelles efficaces dans divers formats de documents avec C#."

############################# Header ############################
title: "Recherche avancée de texte dans les documents" 
description: "GroupDocs.Search for .NET facilite la recherche de texte dans des formats de documents populaires, vous permettant de créer des requêtes de recherche puissantes dans vos applications .NET."
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
    title: "Qu'est-ce que GroupDocs.Search ?"
    link: "/search/net/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) est une bibliothèque puissante conçue pour la recherche en texte intégral et l'indexation dans les documents. Elle prend en charge plus de 70 formats de fichiers, y compris PDF, Word, PowerPoint, Excel, images et fichiers ZIP, garantissant des résultats de recherche rapides et précis.

############################# Steps ############################
steps:
    enable: true
    title: "Comment effectuer une recherche textuelle dans des documents PDF"
    content: |
      [GroupDocs.Search](/search/net/) permet des opérations de recherche de contenu avancées dans des documents PDF, permettant des résultats de recherche affinés dans les applications .NET.
      
      1. Configurez le dossier pour stocker l'index de recherche.
      2. Choisissez le dossier contenant les fichiers PDF.
      3. Configurez les options de recherche supplémentaires.
      4. Effectuez la recherche et examinez les résultats.
   
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
        // Définir le chemin pour l'index de recherche
        Index index = new Index("c:/MyIndex");

        // Sélectionnez le dossier contenant les documents à rechercher
        index.Add("c:/MyDocuments");

        // Activez la recherche de mots homophones pour trouver des mots ayant des sonorités similaires
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Exécutez une requête de recherche complexe
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fonctionnalités avancées de recherche et d'indexation"
  description: "GroupDocs.Search for .NET améliore la recherche de texte et l'indexation sur plus de 70 formats de fichiers, fournissant des outils efficaces pour localiser et gérer l'information."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de texte puissante"
      content: "Recherchez du texte à travers plusieurs types de documents, y compris les PDF, documents Word, présentations PowerPoint et tableurs. Utilisez des fonctionnalités telles que les correspondances exactes, la recherche floue et les jokers pour affiner les résultats."

    # feature loop
    - title: "Indexation rapide pour de grands ensembles de données"
      content: "Créez et gérez des index de recherche pour une récupération rapide de l'information. L'indexation optimise les recherches à travers de vastes collections de documents."

    # feature loop
    - title: "Support multilingue"
      content: "Effectuez des recherches dans plus de 80 langues, avec un support pour différents claviers et variations de mots pour améliorer la précision."

    # feature loop
    - title: "Paramètres de recherche personnalisables"
      content: "Affinez les paramètres de recherche avec des options telles que la sensibilité à la casse, les filtres de plage de dates et l'exclusion de mots pour de meilleurs résultats."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exécution de requêtes de recherche avancées"
      content: |
        Cet exemple démontre comment appliquer des requêtes de recherche pour des documents PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Définissez le dossier pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Spécifiez le chemin vers les fichiers de document
          index.Add("c:/MyDocuments");

          // Fournissez un mot de passe pour les documents protégés
          index.Dictionaries.DocumentPasswords.Add("protected.pdf", "123456");

          // Activez la recherche floue pour trouver des mots similaires
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Récupérez les résultats de la recherche
          SearchResult result = index.Search("Loarem", options);
          
          // Traitez la sortie de recherche
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "Explorez les fonctionnalités clés"
    exclude: "document"
    description: "Profitez de fonctionnalités de recherche avancées et performantes."
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
    title: "Recherchez dans vos documents d'entreprise"
    exclude: "PDF"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers, notamment les documents de bureau, permettant des recherches rapides et efficaces avec des capacités d'indexation."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---