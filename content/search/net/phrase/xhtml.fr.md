---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/net/phrase /xhtml/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP  MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Comment ajouter une recherche de phrases dans les documents XHTML dans les applications .NET ?"
head_description: "L'API GroupDocs.Search .NET permet aux professionnels du logiciel d'ajouter la recherche de phrases et de trouver la phrase exacte ou la séquence de mots fournie dans les documents XHTML via l'API .NET."

############################# Header ############################
title: "Ajouter une phrase exacte ou rechercher une expression dans XHTML Documents dans les applications .NET ?"
description: "L'API GroupDocs.Search .NET permet aux programmeurs de trouver la séquence de mots fournie dans les documents XHTML via une recherche de phrases ou une recherche de phrases exactes dans les applications .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment utiliser la recherche exacte de phrases ou de phrases dans les applications .NET ?"
    content: |
       La recherche de phrases ou de phrases exactes est un type de recherche qui permet aux utilisateurs de rechercher des documents, un site Web ou une base de données contenant une phrase ou une phrase exacte contenant un ordre spécifique et une combinaison de mots définis par les consommateurs. C'est un terme très courant dans la terminologie des moteurs de recherche et permet aux utilisateurs de rechercher des documents pour une séquence de mots spécifiée dans le texte des documents indexés. GroupDocs.Search for .NET est une API de recherche de documents et de texte hautes performances très utile qui fournit des fonctionnalités complètes pour développer des applications de recherche et d'indexation de texte prenant en charge certains des types de documents les plus courants tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, Feuilles de calcul Excel, présentations PowerPoint, Outlook MSG, PST, etc. Il a inclus la prise en charge de plusieurs fonctionnalités liées à la recherche de phrases telles que la recherche de requêtes sous forme de texte et d'objet, l'utilisation de caractères génériques dans la recherche de phrases, etc.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Comment effectuer une recherche de phrases dans les documents XHTML via .NET"
      content_left: |
       L'API GroupDocs.Search .NET permet aux développeurs de logiciels d'ajouter des fonctionnalités de recherche de phrases dans leur propre application C# .NET. L'exemple de code .NET suivant montre comment effectuer une recherche d'expression dans le texte et l'objet avec seulement quelques lignes de code.

      title_right: "Recherche d'expressions exactes dans XHTML Documents"
      content_right: |
         * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
         * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Indexation des documents du dossier spécifié en appelant la méthode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Recherchez la requête de phrase 'phrase text' sous forme de texte
         * Recherchez l'expression 'phrase text' sous forme d'objet
         * Création de word1, word2 et création de la sous-requête 3 en appelant la méthode [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
         * Combinaison de sous-requêtes pour créer une nouvelle requête de recherche en appelant la méthode [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
         * Lancer la recherche et afficher les résultats de la recherche
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: "Recherche d'expressions génériques dans XHTML Documents via .NET"
      content_left: |
        GroupDocs.Search pour .NET permet aux programmeurs de logiciels d'ajouter des fonctionnalités de recherche de phrases à l'aide de caractères génériques dans l'application C# .NET. Les exemples de code .NET suivants montrent comment appliquer la recherche d'expressions génériques dans XHTML Documents dans les applications C#.

      title_right: "Appliquer la recherche de phrases génériques dans le fichier XHTML"
      content_right: |
        * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
        * Création d'index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexation des documents du dossier spécifié en appelant la méthode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Recherchez la requête de phrase 'phrase text' sous forme de texte
        * Recherchez l'expression 'phrase text' sous forme d'objet
        * Création de word1 et création de subquery 3 en appelant la méthode [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
        * Création de wildcard2 en appelant la méthode [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1)
        * Combinaison de sous-requêtes pour créer une nouvelle requête de recherche en appelant la méthode [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
        * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: "Combinez la recherche de phrases avec d'autres types de recherches via .NET"
      content_left: |
        GroupDocs.Search .NET donne aux programmeurs de logiciels le pouvoir de combiner la recherche de phrases avec d'autres types de recherches dans l'application .NET. Les exemples de code .NET suivants montrent comment appliquer des caractères génériques représentant des mots et des caractères dans des mots.

      title_right: "API .NET pour combiner la recherche de phrases avec d'autres recherches"
      content_right: |
        * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
        * Création d'index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexation des documents du dossier spécifié en appelant la méthode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Rechercher la phrase sous forme de texte
        * Rechercher la phrase sous forme d'objet
        * Définir le modèle de mot et ajouter une chaîne.
        * Création de wordPattern1 et Création de word3 en appelant la méthode [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery)
        * Création de wildcard2 en appelant la méthode [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1)
        * Combinaison de sous-requêtes pour créer une nouvelle requête de recherche en appelant la méthode [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
        * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

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