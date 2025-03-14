
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: fr
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Trouvez du texte dans PPTX avec GroupDocs.Search dans Node.js"
head_description: "Utilisez GroupDocs.Search for Node.js via Java avec JavaScript pour rechercher du texte efficacement dans divers formats de documents."

############################# Header ############################
title: "Solution de recherche documentaire intelligente" 
description: "Localisez rapidement du texte dans différents formats de documents grâce à GroupDocs.Search for Node.js via Java. Créez des requêtes de recherche avancées au sein de vos applications Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Essayez gratuitement"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction à GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) est une bibliothèque haute performance pour la recherche en texte intégral et l'indexation de documents. Elle prend en charge plus de 70 types de fichiers, y compris PDF, Word, PowerPoint, Excel, images et archives ZIP, garantissant des résultats rapides et précis.

############################# Steps ############################
steps:
    enable: true
    title: "Effectuer une recherche dans des fichiers PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) vous permet d'exécuter des recherches dans des fichiers PPTX, en affinant les résultats dans les applications Node.js via Java.
      
      1. Définissez un dossier de stockage pour l'index de recherche.
      2. Sélectionnez un dossier contenant des fichiers PPTX.
      3. Définissez des paramètres de recherche supplémentaires.
      4. Exécutez la recherche et analysez les résultats.
   
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

        // Spécifiez le répertoire pour le stockage de l'index de recherche
        const index = new searchLib.Index("c:/MyIndex");

        // Choisissez le dossier contenant les documents à rechercher
        index.add("c:/MyDocuments");

        // Activez la recherche par homophones pour des mots similaires
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Exécutez une requête de recherche complexe
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacités avancées de recherche et d'indexation"
  description: "GroupDocs.Search for Node.js via Java offre des outils puissants de recherche textuelle et d'indexation à travers plus de 70 formats de documents, facilitant la recherche et l'organisation des informations."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Principaux avantages de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche textuelle exhaustive"
      content: "Localisez du texte dans plusieurs types de documents, y compris des PDF, des documents Word, des présentations PowerPoint et des tableurs. Utilisez des correspondances exactes, des recherches floues et des caractères génériques pour des résultats affinés."

    # feature loop
    - title: "Indexation efficace pour les grandes données"
      content: "Accélérez les recherches en créant des index structurés, facilitant la récupération d'informations à partir de grandes collections de documents."

    # feature loop
    - title: "Prend en charge plus de 80 langues"
      content: "Recherchez dans des documents de différentes langues, avec reconnaissance automatique de diverses formes de mots et dispositions de clavier."

    # feature loop
    - title: "Paramètres de recherche personnalisés"
      content: "Ajustez les options de recherche telles que la sensibilité à la casse, les filtres de date et les exclusions de mots pour obtenir des résultats précis."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utiliser la recherche pour les documents PPTX"
      content: |
        Cet exemple montre comment utiliser des requêtes de recherche dans des documents PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Définissez le répertoire pour l'indexation de recherche
          const index = new searchLib.Index("c:/MyIndex");
              
          // Fournissez le chemin du fichier pour le stockage des documents
          index.add("c:/MyDocuments");

          // Entrez le mot de passe pour les fichiers protégés
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", '123456');

          // Activez la recherche floue pour la détection de mots similaires
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Extrayez les résultats de recherche
          const result = index.search("Loarem", options);
          
          // Traitez et examinez les résultats
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
            link: "/examples/search/formats/searchdocument.pptx"
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
    title: "Explorez les fonctionnalités clés"
    exclude: "document"
    description: "Découvrez des fonctionnalités de recherche à haute vitesse conçues pour améliorer l'efficacité et la précision."
    items: 
          
        # operation loop 1
        - name: "Recherche par condition"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Trouvez des informations dans les documents en utilisant des conditions booléennes"

        # operation loop 2
        - name: "Recherche sensible à la casse"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Améliorez la précision de la recherche en tenant compte de la casse"

        # operation loop 3
        - name: "Indexation de documents"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Indexez les documents une fois et réutilisez l'index pour plusieurs recherches"

        # operation loop 4
        - name: "Filtres de recherche"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Utilisez des filtres pour affiner les données traitées"

        # operation loop 5
        - name: "Phrase exacte"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Recherchez une phrase ou une expression spécifique"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Recherchez dans une variété de documents"
    exclude: "PPTX"
    description: "GroupDocs.Search fonctionne avec plus de 70 formats de fichiers, y compris les documents de bureau, garantissant des recherches rapides et précises avec un support d'indexation."
    items: 
        # format loop 1
        - name: "Recherche dans le document DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Recherche dans le document PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Recherche dans le document PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Recherche dans le document TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Recherche dans le document XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---