
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:52
draft: false
lang: fr
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Rechercher des phrases dans TXT en utilisant Java"
head_description: "GroupDocs.Search for Java améliore les applications Java avec des capacités avancées de recherche de phrases pour le contenu des documents."

############################# Header ############################
title: "Trouvez des phrases dans les documents" 
description: "Localisez rapidement des phrases spécifiques avec GroupDocs.Search for Java. Ajoutez une fonctionnalité de recherche puissante à vos applications Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Télécharger"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Fonctionnalités de GroupDocs.Search"
    link: "/search/java/"
    link_title: "En savoir plus"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) est une bibliothèque robuste pour l'indexation et la recherche de texte au sein des documents. Elle prend en charge plus de 70 formats de fichiers, y compris les PDF, documents Word, tableurs Excel, images et fichiers ZIP, garantissant des résultats de recherche rapides et précis.

############################# Steps ############################
steps:
    enable: true
    title: "Comment trouver des phrases dans des documents TXT"
    content: |
      [GroupDocs.Search](/search/java/) facilite la recherche de phrases dans des documents TXT. Utilisez diverses options pour affiner les résultats de recherche dans les applications Java.
      
      1. Créer un répertoire pour l'index de recherche.
      2. Spécifiez le dossier contenant les fichiers TXT.
      3. Ajustez les paramètres de recherche.
      4. Récupérez et analysez les résultats de recherche.
   
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
        // Définir le chemin de l'index de recherche
        Index index = new Index("c:/MyIndex");

        // Spécifiez le dossier contenant les documents
        index.add("c:/MyDocuments");

        // Définir les préférences de recherche
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Exécuter la requête de recherche
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explorez le moteur de recherche de documents Java"
  description: "GroupDocs.Search for Java permet des recherches de phrases dans plus de 70 formats de fichiers. Trouvez et organisez facilement des données grâce à des fonctionnalités de recherche avancées."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Capacités clés de GroupDocs.Search"
  features:
    # feature loop
    - title: "Recherche de phrases"
      content: "Localisez des phrases exactes dans des documents commerciaux, tels que PDF, fichiers Word, présentations et tableurs. Utilisez des jokers et d'autres options lorsque la phrase exacte est inconnue."

    # feature loop
    - title: "Indexation des données optimisée"
      content: "Accélérez les recherches de documents en créant et en réutilisant des index de recherche. L'indexation organise les données efficacement pour des recherches plus rapides et plus précises."

    # feature loop
    - title: "Compatibilité multilingue"
      content: "Recherchez des documents en plus de 80 langues. Prend en charge différentes dispositions de clavier et analyses morphologiques pour améliorer la précision des recherches."

    # feature loop
    - title: "Options de recherche avancées"
      content: "Personnalisez les recherches avec sensibilité à la casse, recherche floue, correspondance des homophones, filtrage de documents et autres fonctionnalités puissantes."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilisation de méthodes de recherche avancées"
      content: |
        Apprenez à construire des requêtes pour effectuer des recherches dans TXT.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Définir le répertoire pour l'index de recherche
          Index index = new Index("c:/MyIndex");
              
          // Définir le chemin vers les documents cibles
          index.add("c:/MyDocuments");

          // Créer une requête de recherche pour une phrase spécifique
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Récupérer les résultats de la recherche
          SearchResult result = index.search(query);
          
          // Traiter et utiliser les résultats récupérés
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
            link: "/examples/search/formats/searchphrase.txt"
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
    title: "Capacités de recherche avancées"
    exclude: "phrase"
    description: "Utilisez des fonctionnalités de recherche de pointe pour améliorer la précision et les performances."
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
    title: "Rechercher des phrases dans des documents commerciaux"
    exclude: "TXT"
    description: "GroupDocs.Search permet des recherches de phrases dans plus de 70 formats de documents. Profitez des options avancées et de l'indexation pour des recherches efficaces."
    items: 
        # format loop 1
        - name: "Recherche de phrase dans DOCX"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Document Open XML de Microsoft Word"
          
        # format loop 2
        - name: "Recherche de phrase dans PDF"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Format de document portable Adobe"
          
        # format loop 3
        - name: "Recherche de phrase dans PPTX"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Présentation Open XML de PowerPoint"

        # format loop 4
        - name: "Recherche de phrase dans TXT"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Document texte"
          
        # format loop 5
        - name: "Recherche de phrase dans XLSX"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Tableur Open XML de Microsoft Excel"
  

---