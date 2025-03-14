
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: fr
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Recherchez dans les documents TXT en utilisant Java"
head_description: "GroupDocs.Search for Java ajoute une recherche textuelle puissante aux applications Java, prenant en charge divers formats de documents professionnels."

############################# Header ############################
title: "Trouver du texte dans des documents professionnels" 
description: "GroupDocs.Search for Java vous permet de rechercher du texte dans des documents en utilisant des requêtes flexibles et précises. Intégrez facilement la fonctionnalité de recherche dans les applications Java."
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
    title: "Qu'est-ce que GroupDocs.Search?"
    link: "/search/java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) est une bibliothèque robuste pour une recherche textuelle rapide et un indexage de documents. Elle prend en charge plus de 70 formats de fichiers, y compris les normes de l'industrie comme PDF, Word, Excel et PowerPoint. Améliorez vos applications avec des capacités de recherche précises et à grande vitesse.

############################# Steps ############################
steps:
    enable: true
    title: "Comment rechercher dans des documents TXT"
    content: |
      [GroupDocs.Search](/search/java/) permet des recherches textuelles rapides et efficaces dans des documents TXT, parfait pour les applications Java.
      
      1. Spécifiez un dossier pour stocker l'index de recherche.
      2. Sélectionnez le dossier contenant vos documents.
      3. Configurez les options de recherche pour limiter les résultats aux documents TXT.
      4. Lancez la recherche et obtenez les résultats.
   
    code:
      platform: "java"
      copy_title: "Copier"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Résultat de la recherche"
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
        // Dossier pour stocker l'index de recherche réutilisable
        Index index = new Index("c:/MyIndex");

        // Dossier contenant les documents
        index.add("c:/MyDocuments");

        // Filtrer les recherches par format de document
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".txt");

        // Récupérer les résultats de recherche
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacités de recherche avancées"
  description: "GroupDocs.Search for Java offre une recherche textuelle avancée dans plus de 70 formats de fichiers. L'indexation accélère les recherches et améliore l'efficacité de la gestion des documents."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Caractéristiques clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche textuelle puissante"
      content: "Trouvez du texte dans des formats de documents populaires tels que les PDF, les fichiers Word, les présentations et les tableurs. Prend en charge plusieurs méthodes de recherche, y compris la recherche floue, les homophones et les jokers."

    # feature loop
    - title: "Indexation optimisée pour de meilleures performances"
      content: "Créez et réutilisez des index de recherche pour améliorer la vitesse et l'efficacité de la recherche, notamment dans de grandes collections de documents."

    # feature loop
    - title: "Support de recherche multilingue"
      content: "Recherchez dans des documents écrits en plus de 80 langues. Détecte différentes dispositions de clavier et variations de mots pour une meilleure précision."

    # feature loop
    - title: "Options de recherche personnalisables"
      content: "Affinez les résultats de la recherche à l'aide de filtres, d'expressions régulières et d'autres paramètres de recherche avancés."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrer les documents avant de rechercher"
      content: |
        Découvrez comment affiner les recherches à l'aide de filtres
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Configurer un index qui exclut certains formats de fichiers
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Spécifier le chemin de stockage des documents
          index.add("c:/MyDocuments");

          // Récupérer les résultats de recherche
          SearchResult result = index.search("Lorem", options);
          
          // Traiter et utiliser les résultats de recherche
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
          - title: "Télécharger le résultat"
            icon: "download"
            link: "/examples/search/formats/searchfilters.txt"
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
    - title: "Téléchargement Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licences"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Caractéristiques clés"
    exclude: "filters"
    description: "Effectuez des recherches textuelles précises et efficaces."
    items: 
          
        # operation loop 1
        - name: "Recherche par condition"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "Trouvez des informations dans les documents en utilisant des conditions booléennes"

        # operation loop 2
        - name: "Recherche sensible à la casse"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "Améliorez la précision de la recherche en tenant compte de la casse"

        # operation loop 3
        - name: "Indexation de documents"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "Indexez les documents une fois et réutilisez l'index pour plusieurs recherches"

        # operation loop 4
        - name: "Filtres de recherche"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "Utilisez des filtres pour affiner les données traitées"

        # operation loop 5
        - name: "Phrase exacte"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "Recherchez une phrase ou une expression spécifique"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Recherchez dans des documents professionnels"
    exclude: "TXT"
    description: "GroupDocs.Search prend en charge plus de 70 formats de fichiers, facilitant la recherche dans des documents de bureau largement utilisés."
    items: 
        # format loop 1
        - name: "Filtres de recherche pour DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Filtres de recherche pour PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Filtres de recherche pour PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Filtres de recherche pour TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Filtres de recherche pour XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---