---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/java/phrase/dot/"
otherformats: PDF DOC DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: "API Java pour rechercher et trouver la phrase exacte dans DOT Documents"
head_description: "L'API Java GroupDocs.Search aide les programmeurs à intégrer la recherche de phrases et à découvrir une séquence de mots donnée ou une phrase exacte dans le texte des documents DOT via Java."

############################# Header ############################
title: "Comment rechercher et afficher une phrase ou une expression exacte dans les documents DOT via l'API Java ?"
description: "L'API Java GroupDocs.Search a fourni une prise en charge complète des fonctionnalités de recherche avancées permettant aux développeurs de logiciels de rechercher une phrase ou une phrase exacte dans les documents DOT via la recherche de phrases ou la recherche de phrases exactes."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que la recherche de phrases et comment l'utiliser dans les applications Java ?"
    content: |
       La recherche par expression est un moyen très efficace de rechercher dans des documents ou des pages Web une phrase ou une expression exacte, plutôt qu'un mot-clé. Cela signifie que lorsque l'utilisateur recherche une expression exacte, il souhaite trouver tous les termes de recherche dans cet ordre particulier dans lequel ils sont apparus. Cette page Web partagera des informations sur la manière dont les utilisateurs peuvent développer des applications et des outils commerciaux pour une recherche efficace de documents et de pages Web à l'aide de l'API Java. GroupDocs.Search for Java est une API Java très bien organisée et efficace qui permet aux développeurs de logiciels d'effectuer des opérations de recherche de texte de niveau basique à avancé dans leurs propres applications sans installer de logiciel tiers. L'API a inclus de nombreuses fonctionnalités utiles liées à la recherche de documents telles que la recherche simple ou booléenne, la recherche floue, la recherche sensible à la casse, les synonymes, les homophones, les caractères génériques, la recherche de type d'objet, la définition de la plage de données et d'autres types de requêtes pour rechercher rapidement et élégamment des informations. De plus, il prend également en charge la reconnaissance des requêtes de recherche écrites dans une langue qui ne correspond pas à la disposition de votre clavier.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Effectuez une recherche d'expressions dans DOT Documents via Java"
      content_left: |
       L'API Java GroupDocs.Search inclut une prise en charge complète de la recherche avancée qui permet aux professionnels du logiciel de créer des applications logicielles puissantes avec des capacités de recherche et une facilité d'utilisation. Le code Java ci-dessous montre comment effectuer une recherche de phrase sous forme de texte et d'objet avec seulement quelques lignes de code.

      title_right: "Recherche de phrases exactes dans les fichiers DOT"
      content_right: |
         * Définissez le chemin d'accès au dossier d'index et au dossier de documents.
         * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
         * Indexation des documents du dossier spécifié en appelant la méthode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
         * Recherche avec requête textuelle en appelant la méthode [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery))
         * Recherchez l'expression 'phrase text' sous forme d'objet
         * Création de word1, word2 et création de la sous-requête 3 en appelant la méthode [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
         * Combinaison de sous-requêtes pour créer une nouvelle requête de recherche en appelant [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) méthode
         * Lancer la recherche et afficher les résultats de la recherche
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "Appliquer la recherche de phrases génériques dans les fichiers DOT via Java"
      content_left: |
        GroupDocs.Search pour Java donne aux programmeurs de logiciels le pouvoir d'ajouter une fonctionnalité de recherche de mots génériques lors de la recherche de fichiers DOT dans l'application Java. Les exemples de code Java suivants montrent comment appliquer la recherche d'expressions génériques dans divers types de documents à l'aide de l'API Java.

      title_right: "Recherche de phrases avec des caractères génériques en Java"
      content_right: |
        * Définissez le chemin d'accès au dossier d'index et au dossier de documents.
        * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
        * Indexation des documents du dossier spécifié en appelant la méthode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
         * Recherche avec requête textuelle en appelant la méthode [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery))
         * Recherchez l'expression 'phrase text' sous forme d'objet
         * Création de word1 et word3 en appelant la méthode [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
         * Création de wildcard2 en appelant la méthode [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int))
         * Combinaison de sous-requêtes pour créer une nouvelle requête de recherche de phrases en appelant [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) méthode
         * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "API Java pour combiner la recherche de phrases et d'autres types de recherches"
      content_left: |
        L'API Java GroupDocs.Search permet aux programmeurs de logiciels de combiner facilement la recherche de phrases avec d'autres types de recherches. Le code Java suivant montre comment effectuer une recherche de phrases via des caractères génériques représentant des mots et des caractères dans des mots.

      title_right: "Comment combiner la recherche de phrases et d'autres recherches"
      content_right: |
        * Définissez le chemin d'accès au dossier d'index et au dossier de documents.
        * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
        * Indexation des documents du dossier spécifié en appelant la méthode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
         * Recherche avec requête textuelle en appelant la méthode [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery))
         * Recherchez l'expression 'phrase text' sous forme d'objet
        * Définir le modèle de mot et ajouter une chaîne et y ajouter un caractère générique
        * Création de wordPattern1 et Création de word3 en appelant la méthode [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern))
        * Création de wildcard2 en appelant la méthode [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int))
        * Combinaison de sous-requêtes pour créer une nouvelle requête de recherche de phrases en appelant [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) méthode
        * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

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