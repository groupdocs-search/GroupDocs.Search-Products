
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:31
draft: false
lang: fr
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Effectuez des recherches sensibles à la casse dans XLSX avec Java"
head_description: "L'API GroupDocs.Search for Java aide les développeurs Java à exécuter des recherches sensibles à la casse sur plusieurs types de documents."

############################# Header ############################
title: "Recherche de Documents Sensible à la Casse" 
description: "GroupDocs.Search for Java vous permet de mettre en œuvre une fonctionnalité de recherche précise sensible à la casse dans vos projets Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenez-le gratuitement"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "En savoir plus sur GroupDocs.Search"
    link: "/search/java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) est un outil polyvalent pour la recherche de texte et l'indexation à travers divers documents. Il prend en charge plus de 70 formats tels que les PDF, les fichiers Word, les présentations PowerPoint, les feuilles de calcul Excel, les images et les fichiers ZIP, vous permettant de gérer efficacement des ensembles de données volumineux.

############################# Steps ############################
steps:
    enable: true
    title: "Guide pour la Recherche Sensible à la Casse dans des Fichiers XLSX"
    content: |
      En utilisant [GroupDocs.Search](/search/java/), vous pouvez effectuer des recherches sensibles à la casse dans des documents XLSX, améliorant ainsi vos projets Java.
      
      1. Définissez le dossier pour stocker l'index de recherche.
      2. Sélectionnez le dossier contenant des fichiers XLSX.
      3. Exécutez la recherche sensible à la casse et collectez les résultats.
      4. Traitez et utilisez les résultats de la recherche.
   
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
        // Définissez l'emplacement pour le stockage de l'index
        Index index = new Index("c:/MyIndex");

        // Indiquez le dossier contenant les documents à rechercher
        index.add("c:/MyDocuments");

        // Activez le mode sensible à la casse dans les paramètres de recherche
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Exécutez la recherche
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Outils de Recherche et d'Indexation Avancés"
  description: "Avec GroupDocs.Search for Java, vous pouvez rationaliser la recherche et l'indexation des documents pour plus de 70 formats, facilitant ainsi la localisation et l'organisation de l'information."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Points forts de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de Texte Flexible"
      content: "Recherchez dans des documents tels que des PDF, des fichiers Word, des tableurs et des présentations. Utilisez des outils tels que la correspondance exacte, la recherche floue et le support des caractères génériques pour affiner vos résultats."

    # feature loop
    - title: "Gestion Efficace des Index"
      content: "Organisez et indexez de grands ensembles de données pour améliorer la vitesse de recherche et la performance lors de la gestion de grandes collections de documents."

    # feature loop
    - title: "Support pour les Langues Globales"
      content: "Effectuez des recherches dans plus de 80 langues, prenant en compte différents agencements de clavier et variations linguistiques pour une meilleure précision."

    # feature loop
    - title: "Filtres de Recherche Personnalisables"
      content: "Ajustez les critères de recherche avec des options telles que la sensibilité à la casse, le filtrage par plage de dates et l'exclusion de mots ou données indésirables lors de l'indexation."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemple : Requêtes de Recherche Sensibles à la Casse"
      content: |
        Cet exemple montre comment mettre en œuvre des recherches sensibles à la casse pour des documents XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Définissez le répertoire pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Spécifiez l'emplacement du dossier de documents
          index.add("c:/MyDocuments");

          // Configurez une requête de recherche
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Activez la sensibilité à la casse dans les options de recherche
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Effectuez la recherche de documents
          SearchResult result = index.search(wordQuery, options);
          
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "Aperçu des Fonctionnalités Clés"
    exclude: "case-sensitive"
    description: "Découvrez les capacités de recherche robustes et efficaces offertes par GroupDocs.Search for Java."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formats de Fichiers Prise en Charge pour la Recherche"
    exclude: "XLSX"
    description: "GroupDocs.Search fonctionne avec plus de 70 formats de documents populaires, offrant des paramètres de recherche personnalisables et une indexation efficace."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---