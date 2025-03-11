
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: fr
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Rechercher des phrases dans PPTX en utilisant Node.js"
head_description: "GroupDocs.Search for Node.js via Java ajoute une fonctionnalité de recherche de phrases puissante aux applications JavaScript pour une recherche de documents efficace."

############################# Header ############################
title: "Trouvez des phrases dans les documents" 
description: "Localisez rapidement des phrases spécifiques avec GroupDocs.Search for Node.js via Java. Intégrez des capacités de recherche rapides et précises dans vos applications Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Fonctionnalités de GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) est une bibliothèque à haute performance pour l'indexation et la recherche de texte dans les documents. Elle supporte plus de 70 formats de fichiers, y compris les PDF, les documents Word, les feuilles de calcul Excel, les images et les archives ZIP, garantissant des résultats de recherche précis et rapides.

############################# Steps ############################
steps:
    enable: true
    title: "Comment trouver des phrases dans des documents PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilite la recherche de phrases dans des documents PPTX. Appliquez différentes options de recherche pour affiner les résultats dans les applications Node.js via Java.
      
      1. Configurez un dossier pour l'index de recherche.
      2. Définissez le dossier contenant les fichiers PPTX.
      3. Configurez les paramètres de recherche.
      4. Récupérez et traitez les résultats de recherche.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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

        // Spécifiez le chemin pour stocker l'index de recherche
        const index = new searchLib.Index("c:/MyIndex");

        // Définissez le dossier contenant les documents
        index.add("c:/MyDocuments");

        // Configurez les paramètres de recherche
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Exécutez la requête de recherche
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Découvrez le moteur de recherche de documents Node.js"
  description: "GroupDocs.Search for Node.js via Java permet des recherches de phrases dans plus de 70 formats de fichiers, facilitant la recherche et l'organisation des données avec des fonctionnalités de recherche avancées."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Capacités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de phrases"
      content: "Trouvez des phrases exactes dans des documents commerciaux tels que des PDF, des fichiers Word, des présentations et des feuilles de calcul. Utilisez des jokers et des options de recherche flexibles lorsque la phrase complète est inconnue."

    # feature loop
    - title: "Indexation de données optimisée"
      content: "Améliorez la performance des recherches en créant des index réutilisables. L'indexation structurée accélère les recherches de documents et améliore la précision."

    # feature loop
    - title: "Compatibilité multi-langues"
      content: "Recherchez des documents dans plus de 80 langues avec le support de différents agencements de claviers et de variations morphologiques, garantissant des résultats précis."

    # feature loop
    - title: "Options de recherche avancées"
      content: "Personnalisez vos recherches avec sensibilité à la casse, correspondance approximative, détection d'homophones, filtrage de documents et d'autres fonctionnalités puissantes."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilisation de techniques de recherche avancées"
      content: |
        Apprenez à construire des requêtes pour rechercher dans PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Définissez le répertoire de l'index de recherche
          const index = new searchLib.Index("c:/MyIndex");
              
          // Définissez le chemin vers les documents cibles
          index.add("c:/MyDocuments");

          // Créez une requête pour la phrase désirée
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Récupérez les résultats de recherche
          const result = index.search(query);
          
          // Traitez et utilisez les résultats
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pptx"
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
    - title: "Téléchargement de NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Capacités de recherche avancées"
    exclude: "phrase"
    description: "Tirez parti de puissantes fonctionnalités de recherche pour des résultats plus rapides et plus précis."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Rechercher des phrases dans des documents commerciaux"
    exclude: "PPTX"
    description: "GroupDocs.Search prend en charge les recherches de phrases dans plus de 70 formats de documents. Utilisez des options avancées et l'indexation pour rationaliser le processus de recherche."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---