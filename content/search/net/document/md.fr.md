---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/net/document/md/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP MHTML CHM EPUB  FB2 

############################# Head ############################
head_title: "Créer et ajouter des documents Recherche et indexation dans les applications .NET"
head_description: "L'API GroupDocs.Search .NET permet d'ajouter des documents instantanés en recherchant des formats prenant en charge des formats tels que PDF DOC, DOCX, RTF, XLSX, CSV, PPTX et des messages électroniques dans les applications .NET."

############################# Header ############################
title: "Comment ajouter la recherche instantanée de documents à MD via l'API C# .NET "
description: "L'API GroupDocs.Search .NET permet aux développeurs d'ajouter des capacités de recherche et d'indexation de documents robustes à leurs applications. Il prend en charge des documents tels que PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, MSG, EML et bien d'autres. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment créer et ajouter des documents de recherche et d'indexation à l'aide de l'API .NET ?"
    content: |
       Cette page aidera les utilisateurs à apprendre comment ajouter des capacités de recherche et d'indexation de documents dans leurs propres applications avec peu d'efforts et de coûts. L'indexation est le processus utilisé par les moteurs de recherche par lequel les données sont organisées et structurées afin qu'elles puissent générer des résultats de recherche pertinents. L'objectif est de trouver et d'afficher rapidement et avec précision les informations relatives aux requêtes de l'utilisateur. GroupDocs.Search pour .NET est une puissante API de recherche de documents hautes performances qui permet aux développeurs de logiciels d'effectuer des opérations de recherche et d'indexation avancées sur la base d'algorithmes flous et de synonymes dans leurs propres applications. Il ne nécessite l'installation d'aucun outil tiers ou logiciel externe sur la machine de l'utilisateur. Il a inclus la prise en charge de certains des formats de documents les plus couramment utilisés, tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, Outlook MSG, PST et bien d'autres. Il prend en charge plusieurs types de recherches telles que mot simple, booléen, recherche d'expressions régulières, recherche sensible à la casse, floue flexible, synonyme, homophone, caractère générique, recherche par morceaux, recherche de type d'objet, définition de la plage de données, etc. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Création d'index de recherche pour le document MD via l'API .NET"
      content_left: |
       L'API GroupDocs.Search .NET fournit une prise en charge complète pour la création d'un nouvel index ou l'ouverture d'un index de recherche existant dans vos propres applications. L'exemple de code C# ci-dessous montre comment créer un nouvel index et ouvrir un index existant en utilisant seulement quelques lignes de code.

      title_right: "Comment créer un nouvel index de recherche ou ouvrir un index de recherche existant"
      content_right: |
         * Vous devez d'abord spécifier le chemin d'accès au dossier d'index
         * Créer une instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Ci-dessus va créer un index en mémoire ou sur un disque et peut également ouvrir un index existant.
       
      gisthash: "9651c19a9436afee860b7f39197f8399"
      gistfile: "create_or_open_new_search_index.cs"

    - title_left: "Comment ajouter des md_documents UPPER de manière synchrone à l'index de recherche"
      content_left: |
       GroupDocs.Search .NET permet aux développeurs de logiciels d'effectuer une indexation de documents de manière synchrone dans leurs propres applications .NET. Les exemples de code C# .NET ci-dessous montrent comment effectuer facilement une indexation synchrone. 

      title_right: "Indexation synchrone de documents via C#"
      content_right: |
        * Vous devez d'abord spécifier le chemin d'accès au dossier d'index
        * Spécifiez le chemin d'accès à un dossier contenant des documents à rechercher
        * Créer une instance de la classe [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2)
        * Ci-dessus créera un index en mémoire ou sur un disque ou ouvrira un index existant.
        * Documents d'indexation synchrone à partir du dossier spécifié
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_synchronously_to_indexing.cs"
      
    - title_left: "Effectuer l'indexation de documents de manière asynchrone via .NET"
      content_left: |
        GroupDocs.Search .NET permet aux programmeurs informatiques d'effectuer une indexation asynchrone de documents dans leurs propres applications .NET. Les exemples de code .NET suivants montrent comment réaliser une indexation asynchrone des documents avec seulement quelques lignes de code.

      title_right: "Indexation de documents MD de manière asynchrone via C#"
      content_right: |
        * Vous devez d'abord spécifier le chemin d'accès au dossier d'index
        * Spécifiez le chemin d'accès à un dossier contenant des documents à rechercher
        * Créer une instance de la classe [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2)
        * S'inscrire à l'événement
        * Besoin d'écrire un code indiquant l'achèvement de l'opération
        * Définition du drapeau pour l'indexation asynchrone
        * Documents d'indexation asynchrone à partir du dossier spécifié
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_asynchronously_to_indexing.cs"

    - title_left: "Comment utiliser et mettre en évidence les résultats de recherche dans MD Docs .NET"
      content_left: |
       GroupDocs.Search .NET API permet aux programmeurs d'interpréter un résultat de recherche et d'afficher les résultats par une simple liste de documents trouvés, ou les mots et expressions trouvés. Vous pouvez également surligner facilement le texte du document. Les exemples de code .NET suivants montrent comment répertorier les documents trouvés et mettre en évidence les résultats de la recherche avec seulement quelques lignes de code.

      title_right: "Mettez en surbrillance les résultats de la recherche dans les fichiers MD via C#"
      content_right: |
        * Effectuer une recherche dans l'index
        * Après une recherche réussie, imprimez le résultat
        * Parcourez les documents et affichez les documents trouvés
        * Surligner les occurrences dans le texte
        * Génération d'un document au format HTML de sortie avec les résultats de recherche en surbrillance
     
      gisthash: "a5d1ad6eedd2acf12a33b541e763cdb4"
      gistfile: "how_to_list_search_result.cs"

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