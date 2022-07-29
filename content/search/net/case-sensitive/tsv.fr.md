---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/net/case-sensitive/tsv/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Appliquer la recherche de texte sensible à la casse dans les documents TSV via .NET"
head_description: "L'API GroupDocs.Search .NET permet aux programmeurs de logiciels d'appliquer une recherche de texte sensible à la casse et de trouver la séquence exacte de mots dans les documents TSV via l'API .NET."

############################# Header ############################
title: "Comment appliquer la recherche sensible à la casse dans les documents TSV dans les applications .NET ?"
description: "L'API GroupDocs.Search .NET permet aux développeurs de logiciels d'appliquer une recherche de texte sensible à la casse dans divers types de documents tels que PDF, HTML, DOCX, PPTX, XLSX et plus encore dans les applications .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Qu'est-ce que la recherche sensible à la casse et comment y parvenir via .NET ?"
    content: |
     Il existe de nombreuses techniques de recherche utiles qui peuvent aider les utilisateurs à rechercher dans divers types de documents une combinaison particulière de mots ou d'autres données. La recherche sensible à la casse est une technique très utile qui permet aux utilisateurs de rechercher des documents et des pages Web, que les lettres majuscules et minuscules soient traitées comme différentes ou égales. Par exemple, "Ordinateur", "ordinateur" et "ORDINATEUR" seront traités comme des mots dissemblables car la lettre "C" est majuscule dans le premier cas, minuscule dans le second et toutes les lettres majuscules dans le 3ème. GroupDocs.Search pour .NET est une API de recherche de documents hautes performances pratique qui permet aux créateurs de logiciels de créer des applications logicielles et des outils pour effectuer facilement la recherche de texte ainsi que l'indexation de documents. L'API prend en charge certains des formats de fichiers les plus couramment utilisés tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, Outlook MSG, PST et bien d'autres. Une autre fonctionnalité utile est qu'il peut identifier les requêtes de recherche écrites dans une langue qui ne correspond pas à la disposition de votre clavier.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Effectuez une recherche sensible à la casse dans TSV Documents via .NET"
      content_left: |
       L'API GroupDocs.Search .NET permet aux programmeurs de logiciels d'ajouter une fonctionnalité de recherche sensible à la casse dans leur propre application C# .NET. L'exemple de code .NET suivant illustre comment effectuer une recherche sensible à la casse avec une requête sous forme de texte dans des fichiers TSV avec seulement quelques lignes de code.

      title_right: "Appliquer la recherche sensible à la casse dans TSV Documents"
      content_right: |
         * Identifiez le chemin d'accès au dossier d'index ainsi qu'au dossier de documents.
         * Générer un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Indexation des documents du dossier spécifié en appelant l'instance de la classe [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
         * Initialise une nouvelle instance de la classe [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
         * Activation de la recherche sensible à la casse en appelant la méthode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
         * Définir la chaîne de recherche et commencer la recherche
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: "Effectuer une recherche sensible à la casse sous forme d'objet via .NET"
      content_left: |
        GroupDocs.Search .NET donne aux développeurs de logiciels le pouvoir de découvrir des mots en gardant à l'esprit les lettres majuscules et minuscules dans l'application .NET. L'exemple de code .NET suivant illustre comment appliquer une recherche sensible à la casse avec une requête sous forme d'objet dans des documents TSV.

      title_right: "Effectuez une recherche sensible à la casse dans TSV Documents"
      content_right: |
        * Identifiez le chemin d'accès au dossier d'index ainsi qu'au dossier de documents.
        * Générer un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexation des documents du dossier spécifié en appelant l'instance de la classe [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
        * Initialise une nouvelle instance de la classe [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
        * Activation de la recherche sensible à la casse en appelant la méthode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
        * Création d'une requête de recherche sous forme d'objet en appelant la méthode [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
        * Lancer la recherche et afficher les résultats de la recherche
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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