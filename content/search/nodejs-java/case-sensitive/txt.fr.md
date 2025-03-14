
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: fr
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Effectuer des recherches sensibles à la casse dans TXT avec Node.js"
head_description: "L'API GroupDocs.Search for Node.js via Java permet aux développeurs JavaScript d'exécuter des recherches sensibles à la casse sur différents types de documents."

############################# Header ############################
title: "Recherche Sensible à la Casse" 
description: "GroupDocs.Search for Node.js via Java vous permet d'implémenter des fonctionnalités de recherche avancées sensibles à la casse dans vos applications Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger Gratuitement"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) est une bibliothèque puissante pour la recherche et l'indexation de texte dans les documents. Elle prend en charge plus de 70 formats, y compris les PDFs, Word, Excel, PowerPoint, les images et les fichiers ZIP, permettant ainsi de gérer efficacement de grandes quantités de données.

############################# Steps ############################
steps:
    enable: true
    title: "Étapes pour Effectuer des Recherches Sensibles à la Casse dans des Fichiers TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilite la réalisation de recherches sensibles à la casse dans des fichiers TXT, améliorant ainsi vos flux de travail Node.js via Java.
      
      1. Configurez un dossier pour stocker l'index de recherche.
      2. Sélectionnez le dossier contenant les fichiers TXT.
      3. Exécutez la recherche et obtenez les résultats.
      4. Traitez et utilisez les résultats.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Résultat de la recherche"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Spécifiez le chemin du dossier de l'index
        const index = new searchLib.Index("c:/MyIndex");

        // Définissez le dossier contenant les documents à rechercher
        index.add("c:/MyDocuments");

        // Activez la recherche sensible à la casse dans les paramètres
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Exécutez la recherche
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fonctionnalités Clés pour la Recherche et l'Indexation de Documents"
  description: "Avec GroupDocs.Search for Node.js via Java, vous pouvez rechercher et indexer facilement du texte dans plus de 70 formats de fichiers. Accédez et organisez les informations sans effort grâce à des outils de recherche avancés."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Fonctionnalités Principales de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de Texte Complète"
      content: "Trouvez du texte dans divers types de documents comme les PDFs, les fichiers Word, les tableurs et les présentations. Utilisez des options telles que les correspondances exactes, les recherches floues et les jokers pour des résultats précis."

    # feature loop
    - title: "Indexation de Données Efficace"
      content: "Créez et gérez des index pour accélérer les recherches. L'indexation vous aide à organiser et à localiser rapidement des données dans de grandes collections de documents."

    # feature loop
    - title: "Prise en Charge de Plusieurs Langues"
      content: "Recherchez des documents en plus de 80 langues avec prise en charge de divers agencements de clavier et variations de mots, assurant des résultats de recherche précis."

    # feature loop
    - title: "Paramètres de Recherche Personnalisables"
      content: "Ajustez les paramètres de recherche, y compris la sensibilité à la casse, les filtres de date et l'exclusion de termes ou données spécifiques lors de l'indexation."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemple : Mise en Œuvre de la Recherche Sensible à la Casse"
      content: |
        Cet exemple démontre comment effectuer des recherches sensibles à la casse pour des documents TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Définissez le dossier pour l'index de recherche
          const index = new searchLib.Index("c:/MyIndex");
              
          // Fournissez le chemin vers le dossier de documents
          index.add("c:/MyDocuments");

          // Configurez une requête de recherche
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Activez les paramètres de recherche sensible à la casse
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Recherchez le texte dans les documents
          const result = index.search(wordQuery, options);
          
          // Traitez et gérez les résultats
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Copier"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.txt"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Search gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Fonctionnalités Clés"
    exclude: "case-sensitive"
    description: "Explorez des fonctionnalités avancées pour une recherche de documents rapide et précise."
    items: 
          
        # operation loop 1
        - name: "Recherche par condition"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Trouvez des informations dans les documents en utilisant des conditions booléennes"

        # operation loop 2
        - name: "Recherche sensible à la casse"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Améliorez la précision de la recherche en tenant compte de la casse"

        # operation loop 3
        - name: "Indexation de documents"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Indexez les documents une fois et réutilisez l'index pour plusieurs recherches"

        # operation loop 4
        - name: "Filtres de recherche"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Utilisez des filtres pour affiner les données traitées"

        # operation loop 5
        - name: "Phrase exacte"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Recherchez une phrase ou une expression spécifique"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formats de Documents Compatibles"
    exclude: "TXT"
    description: "GroupDocs.Search prend en charge plus de 70 formats de documents. Personnalisez vos options de recherche et gagnez du temps avec l'indexation."
    items: 
        # format loop 1
        - name: "Recherche sensible à la casse dans DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Recherche sensible à la casse dans PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Recherche sensible à la casse dans PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Recherche sensible à la casse dans TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Recherche sensible à la casse dans XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---