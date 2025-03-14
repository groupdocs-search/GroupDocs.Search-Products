
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: fr
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Recherche sensible à la casse dans PPTX avec .NET"
head_description: "L'API GroupDocs.Search for .NET permet aux développeurs C# d'effectuer des recherches sensibles à la casse à travers divers documents."

############################# Header ############################
title: "Recherche Sensible à la Casse" 
description: "GroupDocs.Search for .NET facilite la création de requêtes de recherche avancées sensibles à la casse au sein de vos applications .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger Gratuitement"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Search ?"
    link: "/search/net/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) est une bibliothèque robuste pour la recherche et l'indexation de texte dans les documents. Elle prend en charge plus de 70 formats de fichiers, y compris PDF, Word, PowerPoint, Excel, images et fichiers ZIP, assurant une gestion efficace de grands volumes de données.

############################# Steps ############################
steps:
    enable: true
    title: "Comment Effectuer une Recherche Sensible à la Casse dans des Documents PPTX"
    content: |
      [GroupDocs.Search](/search/net/) facilite la recherche sensible à la casse dans les documents PPTX. Utilisez-le pour affiner les résultats dans les applications .NET.
      
      1. Définir le dossier pour stocker l'index de recherche.
      2. Choisir le dossier contenant les fichiers PPTX.
      3. Exécuter la recherche et récupérer les résultats.
      4. Traiter les résultats.
   
    code:
      platform: "net"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Résultat de la recherche"
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

        // Spécifier le dossier contenant les documents à rechercher
        index.Add("c:/MyDocuments");

        // Activer la recherche sensible à la casse dans les options
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Exécuter la recherche
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fonctionnalités Avancées pour la Recherche et l'Indexation de Documents"
  description: "La bibliothèque GroupDocs.Search for .NET simplifie la recherche de texte et l'indexation à travers plus de 70 formats de fichiers. Localisez et gérez facilement les informations grâce à des outils de recherche puissants."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Fonctionnalités Clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de Texte Avancée"
      content: "Recherchez du texte dans divers formats de fichiers, y compris PDF, documents Word, tableurs et présentations. Utilisez des options comme les correspondances exactes, la recherche approximative et les jokers pour des résultats précis."

    # feature loop
    - title: "Indexer de Grands Ensembles de Données"
      content: "Créez et maintenez des index pour des recherches plus rapides. Une indexation organisée simplifie la recherche dans des collections étendues de documents."

    # feature loop
    - title: "Support Multilingue"
      content: "Recherchez dans des documents dans plus de 80 langues, avec prise en charge de différentes dispositions de clavier et formes de mots pour des résultats plus précis."

    # feature loop
    - title: "Options de Recherche Personnalisables"
      content: "Personnalisez les paramètres de recherche avec sensibilité à la casse, filtres de date et la possibilité d'exclure des mots ou des données spécifiques lors de l'indexation."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilisation des Requêtes de Recherche Sensibles à la Casse"
      content: |
        Cet exemple montre comment utiliser des requêtes sensibles à la casse pour rechercher des documents PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Définir le dossier pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Spécifier le chemin vers les documents à rechercher
          index.Add("c:/MyDocuments");

          // Créer une requête de recherche
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Activer les options de recherche sensibles à la casse
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Rechercher du texte dans les documents
          SearchResult result = index.Search(wordQuery, options);
          
          // Traiter les résultats de recherche
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
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    - title: "Téléchargement Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Découvrez les Fonctionnalités Clés"
    exclude: "case-sensitive"
    description: "Explorez les fonctionnalités de recherche avancées et efficaces."
    items: 
          
        # operation loop 1
        - name: "Recherche par condition"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "Trouvez des informations dans les documents en utilisant des conditions booléennes"

        # operation loop 2
        - name: "Recherche sensible à la casse"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "Améliorez la précision de la recherche en tenant compte de la casse"

        # operation loop 3
        - name: "Indexation de documents"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "Indexez les documents une fois et réutilisez l'index pour plusieurs recherches"

        # operation loop 4
        - name: "Filtres de recherche"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "Utilisez des filtres pour affiner les données traitées"

        # operation loop 5
        - name: "Phrase exacte"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "Recherchez une phrase ou une expression spécifique"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Rechercher des Formats de Document Populaires"
    exclude: "PPTX"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers. Personnalisez les règles de recherche et utilisez l'indexation pour gagner du temps et de l'effort."
    items: 
        # format loop 1
        - name: "Recherche sensible à la casse dans DOCX"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Recherche sensible à la casse dans PDF"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Recherche sensible à la casse dans PPTX"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Recherche sensible à la casse dans TXT"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Recherche sensible à la casse dans XLSX"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---