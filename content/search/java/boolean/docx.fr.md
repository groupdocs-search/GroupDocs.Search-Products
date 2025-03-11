
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: fr
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Recherche booléenne dans DOCX avec Java"
head_description: "Avec GroupDocs.Search for Java, les développeurs peuvent effectuer des recherches de documents en utilisant des opérateurs booléens tels que AND, OR et NOT."

############################# Header ############################
title: "Recherche de texte booléenne" 
description: "Utilisez GroupDocs.Search for Java pour créer des requêtes de recherche avancées booléennes (AND, OR, NOT) dans vos projets Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger gratuitement"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "À propos de GroupDocs.Search"
    link: "/search/java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) est une bibliothèque polyvalente conçue pour la recherche de texte et l'indexation de données dans les documents. Elle prend en charge plus de 70 types de fichiers, notamment PDF, Word, Excel, PowerPoint, images et archives ZIP, permettant des recherches efficaces à travers de grandes collections de données.

############################# Steps ############################
steps:
    enable: true
    title: "Comment effectuer des recherches booléennes dans des documents DOCX"
    content: |
      [GroupDocs.Search](/search/java/) permet des recherches de texte dans des documents DOCX. Avec le support des conditions booléennes, vous pouvez améliorer la précision des recherches dans les applications Java.
      
      1. Spécifiez le dossier pour stocker l'index de recherche.
      2. Sélectionnez le dossier contenant les documents DOCX.
      3. Exécutez la requête de recherche et récupérez les résultats.
      4. Traitez les résultats obtenus.
   
    code:
      platform: "java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "cliquez pour copier"
        copy_done: "copié"
      links:
        #  loop
        - title: "Plus d'exemples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Définissez le chemin du dossier d'index
        Index index = new Index("c:/MyIndex");

        // Fournissez le chemin du dossier contenant les documents pour la recherche
        index.add("c:/MyDocuments");

        // Exécutez une recherche avec une requête complexe
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Outils puissants pour la recherche et l'indexation de documents"
  description: "GroupDocs.Search for Java simplifie les recherches de texte et l'indexation de données pour plus de 70 formats. Ses outils avancés vous permettent de trouver et de gérer le contenu de manière efficace."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de texte complète"
      content: "Recherchez à travers plusieurs formats tels que des PDFs, des documents Word, des présentations, des feuilles de calcul, et plus encore. Utilisez des options telles que la correspondance exacte, la recherche floue et les requêtes avec des jokers pour affiner les résultats."

    # feature loop
    - title: "Indexation de données efficace"
      content: "Construisez et maintenez des index pour des recherches de documents plus rapides. Cette fonctionnalité organise les données de manière efficace, facilitant la gestion de grandes collections de documents."

    # feature loop
    - title: "Support multi-langues"
      content: "Recherchez dans des documents écrits en plus de 80 langues. Améliorez la précision en exploitant les formes morphologiques des mots et les différentes dispositions de clavier."

    # feature loop
    - title: "Personnalisation flexible de la recherche"
      content: "Ajustez les paramètres de recherche avec des fonctionnalités telles que la sensibilité à la casse, les filtres de plage de dates et les exclusions pour affiner vos résultats."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilisation de requêtes de recherche booléennes complexes"
      content: |
        Cet exemple montre comment effectuer des recherches booléennes dans des fichiers DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Définissez le dossier pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Fournissez le chemin des documents à rechercher
          index.add("c:/MyDocuments");

          // Construisez la requête en utilisant la logique booléenne
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Récupérez les résultats de la recherche
          SearchResult result = index.search(booleanQuery);
          
          // Traitez les résultats récupérés
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Copier"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "cliquez pour copier"
          copy_done: "copié"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
        links:
          #  loop
          - title: "Plus d'exemples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Prêt à commencer ?"
  description: "Essayez les fonctionnalités de GroupDocs.Search gratuitement ou demandez une licence"
  items:
    #  loop
    - title: "Téléchargement de Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Fonctionnalités clés en un coup d'œil"
    exclude: "boolean"
    description: "Débloquez des capacités de recherche puissantes et efficaces"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Rechercher des formats de documents populaires"
    exclude: "DOCX"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers, vous permettant de personnaliser les règles de recherche et d'utiliser l'indexation pour optimiser les performances."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---