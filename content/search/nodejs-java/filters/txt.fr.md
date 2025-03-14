
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: fr
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Rechercher dans des documents TXT en utilisant Node.js"
head_description: "GroupDocs.Search for Node.js via Java apporte des capacités de recherche textuelle rapides et précises aux applications JavaScript, prenant en charge plusieurs formats de documents."

############################# Header ############################
title: "Trouver du texte dans des documents professionnels" 
description: "GroupDocs.Search for Node.js via Java offre une fonctionnalité de recherche puissante et flexible pour les documents. Intégrez la recherche textuelle dans les applications Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) est une bibliothèque robuste de recherche et d'indexation qui permet une récupération rapide de texte dans des documents. Elle prend en charge plus de 70 formats de fichiers, y compris PDF, Word, Excel et PowerPoint, garantissant des recherches précises et efficaces.

############################# Steps ############################
steps:
    enable: true
    title: "Comment effectuer une recherche dans des documents TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilite la recherche de texte dans des documents TXT pour les applications Node.js via Java.
      
      1. Créez un répertoire pour stocker l'index de recherche.
      2. Choisissez le dossier contenant les documents.
      3. Définissez les options de recherche pour inclure uniquement des fichiers TXT.
      4. Exécutez la recherche et récupérez les résultats.
   
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

        // Définir un répertoire pour stocker l'index de recherche
        const index = new searchLib.Index("c:/MyIndex");

        // Spécifiez le dossier contenant les documents consultables
        index.add("c:/MyDocuments");

        // Restreindre la recherche à des formats de fichiers spécifiques
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // Récupérer et traiter les résultats de recherche
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacités de recherche avancées"
  description: "GroupDocs.Search for Node.js via Java améliore l'efficacité de la recherche documentaire en indexant plus de 70 formats de fichiers. Optimisez la récupération de contenu avec des techniques de recherche avancées."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de texte complète"
      content: "Extraire et localiser du texte dans des formats de documents populaires, tels que les PDF, les fichiers Word, les tableurs et les présentations. Prend en charge la recherche approchée, les homophones et les requêtes avec caractères génériques."

    # feature loop
    - title: "Indexation optimisée pour la performance"
      content: "Accélérez les recherches en créant des index réutilisables. Améliore la vitesse et l'efficacité lors de la manipulation de grandes collections de documents."

    # feature loop
    - title: "Support multilingue"
      content: "Recherchez à travers des documents en plus de 80 langues. Reconnaît les mises en page de clavier et les variations de mots pour une meilleure précision."

    # feature loop
    - title: "Options de recherche personnalisables"
      content: "Affinez les résultats de recherche avec des filtres, des expressions régulières, la sensibilité à la casse et d'autres paramètres flexibles."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrer les documents consultables"
      content: |
        Apprenez à affiner les recherches de documents à l'aide de filtres.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Configurer un index pour exclure des formats de fichiers indésirables
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Spécifiez le répertoire contenant les documents
          index.add("c:/MyDocuments");

          // Traitez les résultats de recherche pour un usage ultérieur
          const result = index.Search("Lorem", options);
          
          // Traitez les résultats de recherche pour un usage ultérieur
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Fonctionnalités clés"
    exclude: "filters"
    description: "Effectuez des recherches textuelles rapides et précises à travers des documents."
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
    title: "Rechercher dans divers formats de documents"
    exclude: "TXT"
    description: "GroupDocs.Search prend en charge plus de 70 types de fichiers, permettant une recherche textuelle efficace à travers divers documents professionnels et de bureau."
    items: 
        # format loop 1
        - name: "Filtres de recherche pour DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Filtres de recherche pour PDF"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Filtres de recherche pour PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Filtres de recherche pour TXT"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Filtres de recherche pour XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---