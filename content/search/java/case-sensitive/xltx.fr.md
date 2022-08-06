---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/java/case-sensitive/xltx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "API Java pour effectuer une recherche de texte sensible à la casse dans XLTX Documents"
head_description: "L'API Java GroupDocs.Search permet aux programmeurs d'effectuer une recherche de texte sensible à la casse et de découvrir la structure exacte des mots dans les documents XLTX via Java."

############################# Header ############################
title: "Effectuez une recherche sensible à la casse dans XLTX Documents dans les applications Java"
description: "L'API Java GroupDocs.Search permet aux développeurs de logiciels d'appliquer une recherche de texte sensible à la casse à travers différents types de documents tels que PDF, HTML, DOCX, PPTX, XLSX et plus dans les applications Java."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment effectuer une recherche sensible à la casse dans les applications Java ?"
    content: |
      La sensibilité à la casse est une technique de recherche très utile qui décrit la capacité d'un programme à différencier les lettres majuscules (majuscules) et minuscules (minuscules) dans les recherches sur le Web, les bases de données ou les documents. Il est très important de se rappeler que, par défaut, le moteur de recherche est insensible à la casse, ce qui signifie que la recherche du mot Ordinateur donnera à la fois des fragments ayant un nom clé ou un texte contenant les mots Ordinateur et ordinateur. Supposons que nous devions restreindre les résultats de la recherche à ceux avec la lettre majuscule "Ordinateur", ce qui signifie que nous avons besoin d'une recherche sensible à la casse. GroupDocs.Search for Java est une API efficace de recherche et d'indexation de documents qui permet aux développeurs de logiciels de développer des applications capables d'effectuer la recherche et l'indexation de texte pour certains des types de documents les plus populaires tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, Présentations PowerPoint, Outlook MSG, PST et bien d'autres. De plus, il peut identifier les requêtes de recherche écrites dans une langue qui ne correspond pas à la disposition de votre clavier.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Recherche sensible à la casse dans XLTX Documents via Java"
      content_left: |
       L'API Java GroupDocs.Search a intégré une prise en charge complète des fonctionnalités de recherche de base et avancées permettant aux développeurs de logiciels d'effectuer des recherches sensibles à la casse dans leurs applications Java avec seulement quelques lignes de code.
       L'exemple de code Java suivant montre comment effectuer une recherche sensible à la casse avec une requête dans le texte des fichiers XLTX avec seulement quelques lignes de code.

      title_right: "Effectuer une recherche sensible à la casse dans les fichiers XLTX"
      content_right: |
         * Identifiez le chemin d'accès au dossier d'index ainsi qu'au dossier de documents.
         * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
         * Indexation des documents du dossier spécifié en appelant l'instance de la classe [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
         * Lancer une nouvelle instance de la classe [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
         * Activation de l'option de recherche sensible à la casse en appelant la méthode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
         * Définir la requête de recherche et commencer la recherche
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Faire une recherche sensible à la casse sous forme d'objet via Java"
      content_left: |
       GroupDocs.Search Java donne aux développeurs de logiciels le pouvoir d'inclure des fonctionnalités de recherche pour divers formats de documents dans leurs propres applications. L'exemple de code Java suivant montre comment effectuer des recherches sensibles à la casse avec une requête sous forme d'objet via des documents XLTX.

      title_right: "Appliquer la recherche sensible à la casse dans XLTX Documents"
      content_right: |
       * Identifiez le chemin d'accès au dossier d'index ainsi qu'au dossier de documents.
       * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
       * Indexation des documents du dossier spécifié en appelant l'instance de la classe [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
       * Lancer une nouvelle instance de la classe [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * Activation de l'option de recherche sensible à la casse en appelant la méthode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
       * Création d'une requête de recherche dans l'objet en appelant la méthode [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
       * Définir la requête de recherche et commencer la recherche
  
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

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