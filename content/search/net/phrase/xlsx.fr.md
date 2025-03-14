
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: fr
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Recherche de phrases dans XLSX utilisant .NET"
head_description: "GroupDocs.Search for .NET enrichit les applications C# avec des capacités de recherche de phrases puissantes pour le contenu des documents."

############################# Header ############################
title: "Rechercher des phrases dans des documents" 
description: "Trouvez rapidement des phrases spécifiques avec GroupDocs.Search for .NET. Intégrez une fonctionnalité de recherche efficace dans vos applications .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Fonctionnalités de GroupDocs.Search"
    link: "/search/net/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) est une bibliothèque puissante pour indexer et rechercher du texte dans des documents. Elle supporte plus de 70 formats de fichiers, y compris les PDF, les documents Word, les feuilles Excel, les images et les fichiers ZIP, permettant d'obtenir des résultats de recherche rapides et précis.

############################# Steps ############################
steps:
    enable: true
    title: "Comment rechercher des phrases dans des documents XLSX"
    content: |
      [GroupDocs.Search](/search/net/) simplifie la recherche dans des documents XLSX. Utilisez différentes options pour affiner les résultats de recherche dans les applications .NET.
      
      1. Configurer le dossier de l'index de recherche.
      2. Spécifiez le dossier contenant les fichiers XLSX.
      3. Configurer les paramètres de recherche.
      4. Récupérer et traiter les résultats de recherche.
   
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
        // Chemin pour stocker l'index de recherche
        Index index = new Index("c:/MyIndex");

        // Dossier contenant des documents
        index.Add("c:/MyDocuments");

        // Configurer les options de recherche
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Exécuter la recherche
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Découvrez le moteur de recherche de documents .NET"
  description: "GroupDocs.Search for .NET permet des recherches par phrase à travers plus de 70 formats de fichiers. Localisez et gérez les données avec des capacités de recherche avancées."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de phrases"
      content: "Recherchez des phrases exactes dans des documents professionnels, y compris les PDF, les fichiers Word, les présentations et les feuilles de calcul. Utilisez des caractères génériques et d'autres options si la phrase exacte est inconnue."

    # feature loop
    - title: "Indexation des données efficace"
      content: "Créez et réutilisez des index de recherche pour accélérer les recherches de documents. L'indexation structure les données de manière efficace, rendant les recherches de phrases plus rapides."

    # feature loop
    - title: "Support multilingue"
      content: "Recherchez des documents dans plus de 80 langues. Supporte différents agencements de clavier et formes morphologiques pour une meilleure précision de recherche."

    # feature loop
    - title: "Options de recherche flexibles"
      content: "Personnalisez les recherches avec des fonctionnalités telles que la sensibilité à la casse, la recherche floue et homophone, le filtrage de documents et plus encore."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilisation de techniques de recherche avancées"
      content: |
        Apprenez à créer des requêtes pour rechercher dans XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Spécifiez le dossier pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Définissez le chemin vers les documents pour la recherche
          index.Add("c:/MyDocuments");

          // Créez une requête pour une phrase spécifique
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Récupérez les résultats de recherche
          SearchResult result = index.Search(query);
          
          // Traitez et utilisez les résultats
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Fonctionnalités avancées"
    exclude: "phrase"
    description: "Tirez parti de fonctionnalités de recherche puissantes et efficaces."
    items: 
          
        # operation loop 1
        - name: "Recherche par condition"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Trouvez des informations dans les documents en utilisant des conditions booléennes"

        # operation loop 2
        - name: "Recherche sensible à la casse"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Améliorez la précision de la recherche en tenant compte de la casse"

        # operation loop 3
        - name: "Indexation de documents"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Indexez les documents une fois et réutilisez l'index pour plusieurs recherches"

        # operation loop 4
        - name: "Filtres de recherche"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Utilisez des filtres pour affiner les données traitées"

        # operation loop 5
        - name: "Phrase exacte"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Recherchez une phrase ou une expression spécifique"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Recherche de phrases dans des documents professionnels"
    exclude: "XLSX"
    description: "GroupDocs.Search prend en charge les recherches dans plus de 70 formats de documents. Utilisez des options avancées et l'indexation pour rationaliser votre processus de recherche."
    items: 
        # format loop 1
        - name: "Recherche de phrase dans DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Recherche de phrase dans PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Recherche de phrase dans PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Recherche de phrase dans TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Recherche de phrase dans XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---