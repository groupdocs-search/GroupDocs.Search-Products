---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de recherche et d'indexation de texte Java pour les documents, PDF, Office et Web"
head_description: "API de recherche de texte avancée pour les applications Java pour rechercher, indexer et récupérer des données à partir de documents : PDF, Word, Excel, présentations, e-mail et formats de fichiers Web."

############################# Header ############################
title: "Rechercher et indexer des documents via l'API Java"
description: "Créez des applications Java pour effectuer la manipulation de recherche de texte dans tous les formats de documents courants."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "/border/groupdocs-search-java.svg"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Aperçu"

            # button loop
            - link: "#features"
              text: "Caractéristiques"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/search"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      GroupDocs.Search pour Java vous permet de produire des applications métier qui permettent à vos utilisateurs finaux d'effectuer des opérations de recherche comme jamais auparavant. Notre API Java permet aux utilisateurs d'utiliser des fonctions de recherche de texte de niveau basique à avancé. Créez et fusionnez plusieurs index. Utilisez des requêtes simples, booléennes, d'expression régulière (Regex), floues et d'autres types de requêtes pour rechercher rapidement et intelligemment dans les index. Vous pouvez récupérer les informations requises, à partir de fichiers, de documents, d'e-mails et d'archives, car GroupDocs.Search pour Java prend en charge tous les formats de fichiers courants.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Search pour Java :

        left:
          enable: true
          icon: "fas fa-search"
          title: "Indexage"
          content: |
            * Créer et gérer
            * Fusionner plusieurs index
            * Multi-Threading Async Indexage
            * Compact Indexage
            * Archived Files Indexage
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "Recherche avancée et requêtes de recherche"
          content: |
            * Recherche floue
            * Recherche de synonymes
            * Recherche par e-mail
            * Traitement des termes homophoniques
            * Recherche de fichiers protégés
            * Simple
            * Carte générique
            * Expression régulière (Regex)
            * À facettes et booléen
            * Sensible aux majuscules et minuscules
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Search pour Java prend en charge tous les [formats de fichiers de documents](https://docs.groupdocs.com/search/java/supported-document-formats/) courants, y compris : Microsoft Office, les images, les diagrammes et bien d'autres.

        left:
          enable: true
          table:
            # table loop
            - title: "Formats Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Project**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Autres formats"
              content: |
                * **Format de document portable** : PDF
                * **Document ouvert** : ODT, OTT, ODS, OTS, ODP
                * **E-mail** : PST, OST, MSG, EML, EMLX
                * **Formats de fichiers Web** : XML, HTM, HTML, XHTML, MHT, MHTML
                * **Audio** : MP3, WAV
                * **Vidéo** : AVI, MOV, QT, FLV, ASF
                * **Texte** : TXT
                * **Format de texte enrichi** : RTF
                * **Fichier de documentation Markdown** : MD
                * **Images** : BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **Autres** : TORRENT, ZIP, DCM, DJVU, EPUB, FB2

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Search for Java prend en charge la suite Systèmes d'exploitation, cadres et gestionnaires de packages:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Microsoft Windows
                * Serveur Microsoft Windows
                * Linux
                * Mac OS

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * Java 7 (1.7) et supérieur

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Environnements de développement"
              content: |
                * NetBeans
                * IDÉE IntelliJ
                * Éclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Outil d'automatisation de construction"
              content: |
                * Maven

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Search for Java Caractéristiques"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Créer un index sur disque ou en mémoire avec le multithreading asynchrone"

      # feature loop
      - icon: "fas fa-eye"
        content: "Afficher la progression de la création et de la mise à jour de l'index"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Sauter sélectivement l'indexation pour des fichiers spécifiques et sauter des mots spécifiques pour indexer plus rapidement"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Effectuer une importation ou utiliser la liste pour modifier les caractères pendant l'indexation et l'exportation vers un fichier"

      # feature loop
      - icon: "fas fa-code"
        content: "Recharger l'index en cas d'erreur d'indexation et d'alerte de l'utilisateur en cas de réglage contradictoires"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Notification d'état de l'index concernant les derniers fichiers traités"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Indexer les archives compressées dans d'autres archives ZIP et obtenir la liste des fichiers indexés dans une archive"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Économisez de l'espace grâce à l'indexation compacte et à l'indexation des documents sécurisés par mot de passe"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Document Extraction de texte à partir d'un index ou d'un fichier source"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Extraction de texte au format HTML dans un fichier et création d'une URL pour naviguer dans les résultats de recherche en HTML"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Ajouter des champs supplémentaires arbitraires à chaque document pendant l'indexation"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configurer le niveau de similarité pour la recherche floue et afficher les meilleurs résultats"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Gestion intelligente des fautes de frappe grâce à la recherche floue"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Utiliser la recherche à facettes et booléenne simultanément"

      # feature loop
      - icon: "fas fa-print"
        content: "Configurer et effectuer une recherche de synonymes et traiter intelligemment les termes homophoniques"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Utiliser la plage de dates et la sensibilité à la casse comme paramètres de recherche"

      # feature loop
      - icon: "fas fa-lock"
        content: "Créer un index pour rechercher et parcourir les e-mails via l'API Aspose.Email"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Utiliser des expressions de recherche avec vérification orthographique et caractères génériques et ignorer les caractères spéciaux dans les requêtes"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Créer une arborescence d'objets unique en combinant plusieurs requêtes"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Divisez la recherche en plus petits morceaux pour rechercher rapidement des index volumineux"

      # feature loop
      - icon: "fas fa-heading"
        content: "Indexer des documents à partir de flux et de structures de données"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Configurer le filtrage de documents dans les résultats de recherche"

      # feature loop
      - icon: "fas fa-cube"
        content: "Ajouter des synonymes anglais au dictionnaire de synonymes par défaut"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Activer le nombre exact d'occurrences pour chaque mot trouvé pour proposer des suggestions de mots alternatives en cas de faute d'orthographe"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Ajouter des attributs de texte aux documents indexés sans réindexation"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Perform Indexage and Searching Operations Based on Characters"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Indexer les métadonnées des formats de documents non textuels"

    more_feature :
      # more_feature_loop
      - title: "Indexage and Search Operation"
        content: |
          L'indexage est utilisé par GroupDocs.Search pour Java pour collecter des données, ainsi que pour les stocker et les analyser pour des opérations de recherche précises et efficaces. GroupDocs.Search pour Java utilise fréquemment ces index pour effectuer des recherches.

          * **Créer un index** : créez un dossier d'index et ajoutez/indexez des documents dans ce dossier.
          * **Charger l'index** : charge un index existant.
          * **Ajouter des documents à l'index** : ajoutez des documents à l'index existant, de manière asynchrone.
          * **Mettre à jour l'index** : mettre à jour l'index existant, chaque fois qu'un document est modifié, ajouté ou supprimé. Cela permet de maintenir les résultats de recherche à jour.
          
          ```java
          // Création de l'index
          Index index = new Index("c:\\MonIndex");
          // Ajout de documents à indexer
          index.addToIndex("c:\\MesDocuments");
          // Recherche des mots 'affect' ou 'effect' dans un document avec 'principal', 'principle', 'principles' ou 'principally'
          SearchResults résultats = index.search("?effet & principe?(2~4)");
          ```
      # more_feature_loop
      - title: "Fusionner plusieurs index pour améliorer l'efficacité de la recherche"
        content: "L'API GroupDocs.Search for Java fournit la fonctionnalité permettant de fusionner plusieurs index en un index commun. Pour un index fréquemment modifié, plusieurs index delta sont créés. Cependant, cette approche ralentit les performances de recherche. GroupDocs.Search pour Java surmonte ce goulot d'étranglement en créant un index commun en fusionnant divers index delta. Cet index fusionné commun contient toutes les informations des index delta fusionnés. Cette approche maintient les index delta inchangés tout en améliorant remarquablement l'efficacité de la recherche. Vous pouvez configurer diverses fonctionnalités pour peaufiner davantage ce processus."

      # more_feature_loop
      - title: "Reconnaître les requêtes de recherche de différentes dispositions de clavier"
        content: "GroupDocs.Search pour Java reconnaît les requêtes de recherche qui ne correspondent pas à la disposition de votre clavier. À l'heure actuelle, 88 langues et 164 dispositions de clavier différentes peuvent être reconnues avec succès par GroupDocs.Search for Java."

      # more_feature_loop
      - title: "Recherche à l'aide de la forme morphologique des mots"
        content: "En utilisant GroupDocs.Search pour Java, vous avez la liberté de rechercher différentes formes de mots. Vous pouvez rechercher la forme singulière et plurielle d'un nom spécifique. Ou vous pouvez choisir de rechercher toutes les formes d'un verbe. La racine, la troisième personne du singulier et le passé simple ainsi que diverses autres formes peuvent également être recherchés. Pour les langues autres que l'anglais, vous pouvez configurer des formes de mots personnalisées."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for .NET"
          image: "/border/groupdocs-search-net.svg"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

        # solution loop
        - img_alt: "GroupDocs.Search for Node.js"
          image: "/border/groupdocs-search-nodejs-java.svg"
          product: "GroupDocs.Search"
          platform: "Node.js via Java"
          link: "/search/nodejs-java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---