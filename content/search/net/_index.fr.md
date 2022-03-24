---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "API de recherche et d'indexation de texte C# .NET pour Word Excel PDF E-mail HTML"
head_description: "API de recherche de texte C # .NET pour indexer et récupérer intelligemment des données à partir de fichiers PDF, Microsoft Office Word, Excel, présentations, OneNote, e-mail, ZIP, EPUB et Web."

############################# Header ############################
title: ".NET API pour rechercher et indexer des documents"
description: "API pour indexer les données et effectuer une recherche de texte dans tous les formats de documents courants à l'aide d'applications .NET."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "/border/groupdocs-search-net.svg"
        product: "GroupDocs.Search"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      GroupDocs.Search pour .NET est une API de recherche de documents et de texte pour les applications métier développées en C#, ASP.NET et d'autres technologies .NET. Cette API .NET prend en charge les fonctionnalités de recherche de base à avancées, par exemple, la création et la fusion de plusieurs index, la recherche dans les index à l'aide de simples, booléens, flous, d'expressions régulières (regex) et d'autres types de requêtes pour récupérer vos données requises, à partir de fichiers, documents et e-mails, grâce à la recherche intelligente. Si vous souhaitez créer une application de recherche rapide, fiable, intelligente et riche en fonctionnalités pour vos utilisateurs finaux, prenant en charge tous les formats de fichiers courants, GroupDocs.Search pour .NET est tout ce dont vous avez besoin.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Search pour .NET :
      
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
          GroupDocs.Search pour .NET prend en charge les [formats de fichier de document] suivants (https://docs.groupdocs.com/search/net/supported-document-formats/) :

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
          GroupDocs.Search for .NET prend en charge la suite Systèmes d'exploitation & Directeur chargé d'emballages:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Windows
                * Serveur Windows
                * windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * .NET Framework 2.0 ou supérieur
                * Mono Framework 1.2 ou supérieur
                * Norme .NET 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Directeur chargé d'emballage"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Environnements de développement"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Search for .NET Caractéristiques"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Créer un index en mémoire ou sur disque et effectuer une indexation et une fusion multithread"

      # feature loop
      - icon: "fas fa-eye"
        content: "Empêcher l'indexation pour les fichiers déjà indexés ou avec une chaîne spécifique dans son nom"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Afficher le pourcentage de progression de la création et de la mise à jour de l'index et obtenir le rapport de recherche"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Indexation plus rapide en excluant des mots spécifiques et la notification d'état de l'index pour les fichiers récemment traités"

      # feature loop
      - icon: "fas fa-code"
        content: "Indexer les archives ZIP dans les archives ZIP et obtenir la liste des fichiers indexés contenus dans une archive"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Utilisez la liste ou l'importation pour remplacer les caractères pendant l'indexation et les exporter vers un fichier"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Indexer et rechercher des fichiers protégés par mot de passe et indexation compacte pour économiser de l'espace disque"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Extraire le texte de l'index ou du fichier source et enregistrer automatiquement l'encodage du fichier texte dans l'index"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Ajouter des champs supplémentaires arbitraires à chaque document pendant l'indexation"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configurer le filtrage de documents dans les résultats de recherche"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Gérer les erreurs de frappe grâce à la recherche floue, définir le niveau de similarité dans la recherche floue et afficher les meilleurs résultats uniquement"

      # feature loop
      - icon: "fas fa-columns"
        content: "Indexer des documents à partir de flux et de structures de données"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Rechercher une expression complète avec des mots vides et combiner la recherche à facettes avec la recherche booléenne"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Recherche basée sur les termes homophoniques, les synonymes, la plage de dates, les caractères génériques et la sensibilité à la casse"

      # feature loop
      - icon: "fas fa-print"
        content: "Indexer et rechercher des e-mails à partir d'Outlook et parcourir à l'aide de l'API Aspose.Email"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Prend en charge la vérification orthographique et les caractères génériques dans les requêtes de recherche et saute les caractères spéciaux dans les phrases de recherche"

      # feature loop
      - icon: "fas fa-lock"
        content: "Limiter les résultats pour chaque terme dans la requête de recherche ainsi que pour tous les résultats"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Extraire du texte HTML dans un fichier et générer une URL pour naviguer dans les résultats de recherche au format HTML"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Combiner plusieurs requêtes dans une seule arborescence d'objets"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Alerter l'utilisateur pour les paramètres non compatibles et le rechargement automatique de l'index en cas d'erreur d'indexation"

      # feature loop
      - icon: "fas fa-heading"
        content: "Activer le nombre exact d'occurrences pour chaque mot trouvé pour proposer des suggestions de mots alternatives en cas de faute d'orthographe"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Ajouter des attributs de texte aux documents indexés sans réindexation"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Indexer les métadonnées des formats de documents non textuels"

    more_feature :
      # more_feature_loop
      - title: "Indexage & Search"
        content: |
          L'API GroupDocs.Search pour .NET utilise fréquemment l'index pour effectuer une recherche. Les index sont utilisés pour collecter, analyser ou stocker des données pour une recherche rapide et précise.

          * **Créer un index** : créez un dossier d'index et ajoutez/indexez des documents dans ce dossier.
          * **Charger l'index** : charge un index existant.
          * **Ajouter des documents à l'index** : ajoutez des documents à l'index existant, de manière asynchrone.
          * **Mettre à jour l'index** : mettre à jour l'index existant, chaque fois qu'un document est modifié, ajouté ou supprimé. Cela permet de maintenir les résultats de recherche à jour.

          ```cs
          Index  index = new Index(@"c:\MyIndex");
          index.AddToIndex(@"c:\MyDocuments");
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      # more_feature_loop
      - title: "Fusionner plusieurs index pour améliorer l'efficacité de la recherche"
        content: "GroupDocs.Search pour .NET est capable de fusionner plusieurs index en un seul index. Si un index est fréquemment mis à jour, il a plusieurs index delta, mais cette approche réduit les performances de recherche. GroupDocs.Search pour l'API .NET fusionne tous les index delta en un seul index consolidé. L'index fusionné principal contiendra toutes les informations des indices delta fusionnés ; cependant, les indices delta resteront inchangés. Cette approche utilisée par notre API améliore considérablement l'efficacité de la recherche. La fonction de fusion d'index fournit de nombreuses fonctionnalités permettant de peaufiner davantage ce processus."

      # more_feature_loop
      - title: "Stocker le texte dans l'index pour générer un balisage HTML"
        content: "GroupDocs.Search pour .NET peut mettre en cache le texte des documents indexés dans un index. Ce texte mis en cache est ensuite utilisé pour générer rapidement un balisage HTML en mettant en évidence les résultats de recherche. Cette approche est beaucoup plus rapide que l'extraction de texte directement à partir de fichiers. La récupération du texte du cache sera disponible même si les fichiers source ne sont plus disponibles. Le texte mis en cache peut être stocké en appliquant différents niveaux de compression pour occuper moins d'espace disque et un temps d'indexation plus rapide."

      # more_feature_loop
      - title: "Obtenir des documents connexes par Fuzzy & Regex Search"
        content: "Lorsque vous effectuez une recherche Fuzzy ou Regex, vous pouvez obtenir la liste des documents qui correspond exactement à votre entrée fournie. Cependant, vous obtiendrez également une liste de documents contenant des mots ou des termes similaires à votre entrée.. Par exemple, si vous utilisez GroupDocs.Search pour .NET, vous effectuez une recherche floue pour la requête \"coût\", vous obtiendrez des documents contenant le mot \"coût\" et des documents contenant des mots similaires tels que \"manteau\". Les résultats dépendront du niveau de flou que vous avez configuré à l'aide de cette API."

      # more_feature_loop
      - title: "Reconnaître les requêtes de recherche de différentes dispositions de clavier"
        content: "GroupDocs.Search pour .Net peut reconnaître les requêtes de recherche écrites dans une langue qui ne correspond pas à la disposition de votre clavier. Actuellement, cette API .NET peut reconnaître avec succès 88 langues et 164 dispositions de clavier différentes."

      # more_feature_loop
      - title: "Recherche à l'aide de la forme morphologique des mots"
        content: "GroupDocs.Search pour l'API .NET vous permet de rechercher différentes formes de mots. Par exemple, pour un nom, vous pouvez rechercher ses formes singulier et pluriel. Pour un verbe, vous pouvez rechercher toutes les formes de ce verbe. Vous pouvez également rechercher la racine, la troisième personne du singulier, le passé simple et diverses autres formes. Pour les langues autres que l'anglais, vous pouvez implémenter des formes de mots personnalisées."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for Java"
          image: "/border/groupdocs-search-java.svg"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
