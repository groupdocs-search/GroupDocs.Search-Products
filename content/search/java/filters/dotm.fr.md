---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/java/filters/dotm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB8 

############################# Head ############################
head_title: "Intégrer le filtrage de documents DOTM dans les résultats de recherche via l'API Java ?"
head_description: "L'API Java GroupDocs.Search aide les développeurs de logiciels à ajouter des capacités de recherche de documents DOTM et à appliquer le filtrage de documents pour personnaliser les résultats de recherche via l'API Java."

############################# Header ############################
title: "Comment intégrer le filtrage de documents pour personnaliser les résultats de recherche dans les applications Java"
description: "L'API Java GroupDocs.Search permet aux programmeurs d'intégrer des fonctionnalités avancées de recherche de documents DOTM ainsi que de personnaliser les résultats de la recherche en définissant le filtrage des documents dans leurs applications Java."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment intégrer le filtrage de documents pour personnaliser les résultats de recherche dans les applications Java"
    content: |
       Le filtrage de documents est une activité très utile qui permet aux applications logicielles de rechercher et de récupérer des documents dans la séquence de mots pertinente saisie par un utilisateur dans le texte des documents indexés. Un filtre contient un ensemble de règles qui définissent les critères utilisés pour sélectionner les enregistrements. Le filtrage de documents permet aux utilisateurs de limiter leur recherche à une certaine section ou à un type de document particulier, ainsi que de naviguer dans les résultats et de trouver ce qu'ils recherchent. GroupDocs.Search pour Java est une API d'indexation et de recherche de documents hautes performances riche en fonctionnalités qui permet aux développeurs de logiciels de créer des applications capables d'indexer du texte et de rechercher certains des formats de fichiers de documents les plus populaires. Il prend entièrement en charge divers types de documents tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, Outlook MSG, PST, etc. Il existe différents types de fichiers disponibles pour que l'utilisateur puisse personnaliser les résultats de la recherche, tels que les filtres de chemin de fichier, le filtre d'extension de fichier, le filtre d'attribut et bien d'autres. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Appliquer le filtre de document dans la recherche de dotm_documents UPPER via Java"
      content_left: |
       L'API Java GroupDocs.Search aide les développeurs de logiciels à créer des applications puissantes avec des capacités de recherche à l'aide de l'API Java. L'exemple de code Java ci-dessous montre comment appliquer un filtre de document pour rechercher différents types de documents avec seulement quelques lignes de code.

      title_right: "Paramètre de filtre de document dans la recherche de dotm_documents UPPER"
      content_right: |
       * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
       * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
       * Indexation des documents du dossier spécifié en appelant la méthode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
       * Création d'un objet d'options de recherche en appelant la classe [earchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions)
       * Définir le filtre de document en appelant la méthode [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Commencez à rechercher et à afficher des documents texte si vous en trouvez
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "Combinez les filtres de recherche de documents pour créer un filtre composite via Java"
      content_left: |
        GroupDocs.Search pour Java permet aux programmeurs de logiciels d'ajouter une capacité de recherche avancée et d'appliquer des filtres personnalisés pour la recherche de documents dans leur application Java. Les utilisateurs peuvent créer un filtre composite en combinant différents types de filtres de recherche. Le code Java suivant montre comment combiner des filtres de documents de recherche pour créer un filtre composite à l'aide des opérateurs booléens AND, OR, NOT etc. avec seulement quelques lignes de code.

      title_right: "Créer un filtre composite pour rechercher des fichiers DOTM"
      content_right: |
       * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
       * Création d'un filtre composite AND qui renvoie tous les documents FB2 et EPUB contenant le mot "Einstein" dans leur chemin complet
       * Créez filter1 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Créez filter2 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Combinez les filtres en appelant la méthode [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...))
       * Créez un filtre composite OR qui renvoie tous les documents DOC, DOCX, PDF et tous les documents contenant le mot Einstein dans leur chemin complet
       * Créez un filtre3 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Créez un filtre4 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Combinez les filtres en appelant la méthode [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...))
       * Création d'un filtre qui renvoie tous les documents trouvés à l'exception des documents TXT
       * Créez un filtre4 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Filtre Appy Not en appelant la méthode [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter))

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
    - title_left: "Configuration requise"
      content_left: |
       GroupDocs.Search pour Java est pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Pour un guide complet de la configuration système requise, veuillez visiter [configuration système requise](https://docs.groupdocs.com/search/java/system-requirements/) avant d'exécuter le code ci-dessous, assurez-vous que les conditions préalables suivantes sont installées sur votre système:
         * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
         * Prise en charge des versions Java : J2SE 7.0 (1.7), J2SE 8.0 (1.8) ou supérieur
         * Obtenez la dernière version de GroupDocs.Search pour les API Java de GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "Pourquoi utiliser GroupDocs.Search"
      content_right: |
        * Création d'index de recherche en mémoire ainsi que sur disque.
        * Capacité d'indexation à partir d'un fichier, d'un flux ou d'une structure.
        * Prise en charge de l'indexation des documents protégés par mot de passe.
        * Prise en charge de la fusion de plusieurs index.
        * Filtrer le document lors de l'indexation de la recherche.
        * Prise en charge de la vérification orthographique lors de la recherche.
        * Les caractères mélangés sont entièrement pris en charge
        * Combinaison de différents types de recherche en une seule requête de recherche.
        * Prise en charge des recherches de mots simples et d'expressions régulières
        * Prise en charge complète du remplacement d'alias dans les requêtes de recherche.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---