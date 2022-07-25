---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/net/boolean/ppsm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Add Opérateurs de recherche booléens (AND, OR, NOT) dans les requêtes de recherche via .NET"
head_description: "L'API GroupDocs.Search .NET permet aux développeurs de logiciels d'ajouter une recherche booléenne ou de développer de nouvelles requêtes à l'aide d'opérateurs booléens AND, OR, NOT dans leurs applications .NET."

############################# Header ############################
title: "Développer des requêtes de recherche complexes à l'aide d'opérateurs booléens AND, OR, NOT dans les applications .NET"
description: "L'API GroupDocs.Search .NET permet aux programmeurs informatiques de développer des requêtes de recherche complexes à l'aide d'opérateurs booléens (AND, OR, NOT) dans leurs applications .NET. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que la recherche booléenne et comment utiliser les opérateurs booléens ?"
    content: |
       La recherche booléenne est une procédure de recherche très utile qui permet aux utilisateurs de combiner différents mots clés avec un opérateur pour délimiter, élargir et définir les résultats de la recherche. L'opérateur booléen tel que AND, OR, NOT et NEAR, etc. aide les utilisateurs à obtenir une gamme de résultats plus large ou à réduire le nombre de résultats de recherche non liés en définissant des limites. GroupDocs.Search for .NET est une puissante API de recherche de documents hautes performances qui permet aux développeurs de logiciels de développer des applications capables d'effectuer la recherche de texte et l'indexation sur certains des formats de fichiers de documents les plus courants tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel. , présentations PowerPoint, Outlook MSG, PST et bien d'autres. L'opérateur booléen ET peut être utilisé pour afficher les résultats pour tous les mots que vous avez saisis, l'opérateur OU donne des résultats pour n'importe lequel des mots que vous avez saisis, l'opérateur NON peut être utilisé pour afficher les résultats de la recherche pour aucune occurrence, etc. Une fonctionnalité intéressante est qu'il peut reconnaître les requêtes de recherche écrites dans une langue qui ne correspond pas à la disposition de votre clavier.  

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Utiliser l'opérateur booléen ET dans les requêtes de recherche via .NET"
      content_left: |
       L'API GroupDocs.Search .NET fournit une prise en charge complète pour l'ajout de fonctionnalités de recherche booléenne dans leur application .NET. L'exemple de code C# ci-dessous montre comment créer un opérateur booléen "AND" dans des requêtes sous forme de texte et d'objet dans leurs propres applications .NET. 

      title_right: " Rechercher PPSM documents  via l'opérateur booléen ET"
      content_right: |
         * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
         * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Indexation des documents du dossier spécifié en appelant la méthode [Rechercher](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Création de la sous-requête 1 et Création de la sous-requête 2 en appelant la classe [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
         * Combinaison de sous-requêtes en une seule requête en appelant la méthode [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Lancer la recherche et afficher les résultats de la recherche
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "Comment utiliser l'opérateur booléen OR via .NET"
      content_left: |
       GroupDocs.Search pour .NET est une API puissante qui permet aux programmeurs de logiciels de rechercher parmi de nombreux formats de documents populaires. Les exemples de code C# .NET ci-dessous montrent comment utiliser l'opérateur booléen "OU" dans les requêtes de forme texte et objet dans les applications C#.

      title_right: "Utilisez l'opérateur booléen OR pour rechercher des fichiers PPSM"
      content_right: |
        * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
        * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexation des documents du dossier spécifié en appelant la méthode [Rechercher](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Création de la sous-requête 1 et Création de la sous-requête 2 en appelant la classe [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Combinaison de sous-requêtes en une seule requête en appelant la méthode [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "Créer des requêtes de recherche complexes à l'aide d'opérateurs booléens"
      content_left: |
        GroupDocs.Search .NET permet aux programmeurs informatiques de combiner différents opérateurs booléens pour créer des requêtes de recherche complexes dans leurs propres applications .NET. Les exemples de code .NET suivants montrent comment complexifier les capacités de recherche de documents sans installer de logiciel ou d'outil externe.

      title_right: "Rechercher PPSM documents via des requêtes de recherche complexes"
      content_right: |
        * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
        * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexation des documents du dossier spécifié en appelant la méthode [Rechercher](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Lancer la recherche et afficher la requête textuelle des résultats de la recherche
        * Recherche avec requête d'objet
        * Création de WordQuery et relativityWordQuery en appelant la classe [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Combinaison de sous-requêtes en une seule requête en appelant la méthode [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Création d'einsteinWordQuery et d'albertWordQuery en appelant la classe [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Combinaison de sous-requêtes en une seule requête en appelant la méthode [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Combinaison de sous-requêtes en une seule requête en appelant la méthode [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

    - title_left: "Configuration requise"
      content_left: |
       GroupDocs.Search pour .NET est pris en charge sur toutes les principales plates-formes et systèmes d'exploitation. Pour un guide complet de la configuration système requise, veuillez visiter [configuration système requise](https://docs.groupdocs.com/search/net/system-requirements/) avant d'exécuter le code ci-dessous, assurez-vous que les conditions préalables suivantes sont installées sur votre système:
         * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
         * Environnement de développement : Visual Studio, Xamarin, MonoDevelop etc.
         * Frameworks : .NET Framework, .NET Standard, .NET Core, Mono
         * Obtenez la dernière version de GroupDocs.Search pour les API .NET à partir de [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
      title_right: "Pourquoi utiliser GroupDocs.Assembly"
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