
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: fr
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Trouvez du texte dans des documents DOCX avec GroupDocs.Search pour Java"
head_description: "GroupDocs.Search for Java aide les développeurs Java à rechercher rapidement du texte dans divers formats de documents."

############################# Header ############################
title: "Recherche de texte dans les documents intelligente" 
description: "Avec GroupDocs.Search for Java, vous pouvez rechercher et extraire du texte sans effort à partir de plusieurs types de documents dans vos applications Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenez un essai gratuit"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Que fait GroupDocs.Search ?"
    link: "/search/java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) est une bibliothèque robuste pour la recherche et l'indexation de documents, prenant en charge plus de 70 formats de fichiers, y compris PDF, Word, PowerPoint, Excel, images et archives ZIP. Elle permet des capacités de recherche rapides, précises et évolutives pour de grandes collections de documents.

############################# Steps ############################
steps:
    enable: true
    title: "Effectuer des recherches textuelles dans des fichiers DOCX"
    content: |
      [GroupDocs.Search](/search/java/) permet de rechercher des fichiers DOCX en utilisant une logique sophistiquée et l'indexation, améliorant la précision des recherches dans les applications Java.
      
      1. Configurez un répertoire pour stocker l'index de recherche.
      2. Choisissez un dossier contenant des fichiers DOCX.
      3. Définissez des options de recherche supplémentaires.
      4. Exécutez la recherche et analysez les résultats.
   
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
        // Définir le répertoire pour le stockage de l'index de recherche
        Index index = new Index("c:/MyIndex");

        // Spécifiez le dossier contenant les documents consultables
        index.add("c:/MyDocuments");

        // Activer la recherche par homophones pour trouver des mots à prononciation similaire
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Exécuter une requête de recherche avancée
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fonctionnalités avancées de recherche et d'indexation"
  description: "GroupDocs.Search for Java facilite la recherche et l'indexation de texte à travers plus de 70 formats de documents, offrant des outils efficaces pour gérer et récupérer rapidement l'information."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Fonctionnalités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de texte complète"
      content: "Trouvez du texte à travers différents formats de documents tels que les PDF, les documents Word, les présentations PowerPoint et les tableurs. Utilisez des correspondances exactes, une recherche approximative et des opérateurs génériques pour des résultats de recherche affinés."

    # feature loop
    - title: "Indexation optimisée pour de grandes données"
      content: "Créez des index structurés pour accélérer les recherches, ce qui facilite la navigation à travers d'importants dépôts de documents."

    # feature loop
    - title: "Prise en charge de plusieurs langues"
      content: "Effectuez des recherches en plus de 80 langues avec une prise en charge intégrée de différents agencements de clavier et variations de morphologie, améliorant ainsi la précision."

    # feature loop
    - title: "Paramètres de recherche flexibles"
      content: "Personnalisez les recherches avec des options telles que la sensibilité à la casse, le filtrage par date et la capacité d'exclure des mots spécifiques pour des résultats précis."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Mise en œuvre de requêtes de recherche avancées"
      content: |
        Cet exemple illustre comment utiliser des requêtes de recherche pour chercher efficacement dans des documents DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Définir le répertoire pour l'indexation de la recherche
          Index index = new Index("c:/MyIndex");
              
          // Fournir le chemin du fichier pour les documents
          index.add("c:/MyDocuments");

          // Entrer le mot de passe pour les documents chiffrés
          index.getDictionaries().getDocumentPasswords().add("protected.docx", "123456");

          // Activer la recherche approximative pour détecter les mots similaires
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Récupérer les résultats de recherche
          SearchResult result = index.Search("Loarem", options);
          
          // Traiter et analyser les résultats de recherche
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
            link: "/examples/search/formats/searchdocument.docx"
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
    title: "Aperçu des fonctionnalités clés"
    exclude: "document"
    description: "Découvrez les fonctionnalités de recherche de texte hautes performances conçues pour l'efficacité et la précision."
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
    title: "Trouvez des informations dans des documents DOCX avec GroupDocs.Search"
    exclude: "DOCX"
    description: "GroupDocs.Search prend en charge plus de 70 formats, y compris les fichiers bureautiques, permettant des recherches rapides avec des fonctionnalités d'indexation avancées."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Format de Document Portable Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Présentation Open XML PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Document Texte"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Feuille de Calcul Open XML Microsoft Excel"
  

---