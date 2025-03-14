
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: fr
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Recherche booléenne TXT via Node.js"
head_description: "Utilisez l'API GroupDocs.Search for Node.js via Java pour effectuer des recherches avancées dans le contenu des documents avec des opérateurs booléens tels que AND, OR et NOT, adaptés aux développeurs JavaScript."

############################# Header ############################
title: "Effectuer des recherches avec logique booléenne" 
description: "Avec GroupDocs.Search for Node.js via Java, vous pouvez créer des requêtes de recherche avancées en utilisant des opérateurs booléens (AND, OR, NOT) de manière fluide dans votre environnement Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger maintenant"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que GroupDocs.Search ?"
    link: "/search/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) est un outil robuste pour rechercher et indexer du texte au sein de documents. Il prend en charge plus de 70 formats comme PDF, Word, Excel, PowerPoint, images et fichiers ZIP, facilitant le traitement de grandes quantités d'informations de manière efficace.

############################# Steps ############################
steps:
    enable: true
    title: "Comment rechercher dans des documents TXT à l'aide d'opérateurs booléens"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) vous permet de rechercher du contenu dans des fichiers TXT de manière efficace. Grâce à la logique booléenne, vous pouvez affiner vos requêtes de recherche dans les applications Node.js via Java pour une meilleure précision.
      
      1. Configurez le dossier pour stocker l'index de recherche.
      2. Sélectionnez le dossier contenant les fichiers TXT pour la recherche.
      3. Exécutez la requête de recherche et récupérez les résultats.
      4. Traitez et analysez les résultats de la recherche.
   
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

        // Définir l'emplacement du dossier d'index
        const index = new searchLib.Index("c:/MyIndex");

        // Préciser le dossier contenant les documents à rechercher
        index.add("c:/MyDocuments");

        // Exécuter une requête de recherche avec une logique avancée
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Outils puissants pour la recherche et l'indexation de documents"
  description: "GroupDocs.Search for Node.js via Java rationalise la recherche de texte et l'indexation pour plus de 70 types de fichiers, vous aidant à trouver et à gérer les informations plus rapidement et avec précision."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Caractéristiques clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de texte améliorée"
      content: "Trouvez du texte rapidement dans divers formats tels que PDFs, documents Word, présentations et feuilles de calcul. Utilisez des fonctionnalités telles que les correspondances exactes, les recherches avec jokers et la recherche approximative pour des résultats précis."

    # feature loop
    - title: "Indexation de données efficace"
      content: "Créez et gérez des index pour accélérer les recherches dans de grandes collections de documents. L'indexation garantit un accès rapide et structuré à vos données."

    # feature loop
    - title: "Support multilingue"
      content: "Recherchez dans des documents écrits dans plus de 80 langues. Le support morphologique et la compatibilité avec les dispositions de clavier améliorent les résultats de recherche dans différentes langues."

    # feature loop
    - title: "Paramètres de recherche flexibles"
      content: "Personnalisez votre recherche en activant la sensibilité à la casse, en appliquant des filtres de dates ou en ignorant des mots et données spécifiques lors de l'indexation."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemple de recherche booléenne avancée"
      content: |
        Cet exemple démontre comment créer des requêtes basées sur des booléens pour rechercher du contenu dans des documents TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Définir le dossier pour l'index de recherche
          const index = new searchLib.Index("c:/MyIndex");
              
          // Fournir l'emplacement des documents à rechercher
          index.add("c:/MyDocuments");

          // Construire une requête en utilisant des opérateurs booléens
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Récupérer les résultats de la recherche
          const result = index.search(booleanQuery);
          
          // Traitez et utilisez les résultats de la recherche
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "Fonctionnalités clés de GroupDocs.Search"
    exclude: "boolean"
    description: "Déverrouillez des fonctionnalités de recherche avancées, efficaces et personnalisables."
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
    title: "Rechercher des formats de document populaires"
    exclude: "TXT"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers, offrant des règles de recherche flexibles et une indexation efficace pour gagner du temps et des efforts."
    items: 
        # format loop 1
        - name: "Recherche booléenne dans DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Recherche booléenne dans PDF"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Recherche booléenne dans PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Recherche booléenne dans TXT"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Recherche booléenne dans XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---