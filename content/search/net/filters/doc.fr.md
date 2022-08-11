---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "fr/search/net/filters/doc/"
otherformats: PDF DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: "Personnalisez les résultats de recherche en configurant le filtrage de documents dans les applications .NET"
head_description: "L'API GroupDocs.Search .NET permet aux développeurs de logiciels de rechercher des documents DOC Documents et de personnaliser les résultats de la recherche en appliquant le filtrage de documents dans les applications .NET."

############################# Header ############################
title: "Définir le filtrage de documents pour personnaliser les résultats de recherche dans les applications .NET"
description: "L'API GroupDocs.Search .NET aide les professionnels du logiciel à ajouter des capacités de recherche de documents et à personnaliser les résultats de recherche en appliquant le filtrage de documents dans leurs applications .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Comment appliquer le filtrage de documents dans les résultats de recherche via .NET ?"
    content: |
       Le filtrage est une technique très utile qui permet aux utilisateurs d'inspecter et de traiter les fonctionnalités. Le filtrage de documents offre aux utilisateurs un moyen simple de parcourir leurs résultats et de trouver ce qu'ils recherchent. Il donne également aux utilisateurs le pouvoir de limiter leur recherche à une certaine section ou à un type de document particulier. GroupDocs.Search pour .NET est une API de recherche de documents hautes performances riche en fonctionnalités qui permet aux développeurs de logiciels de créer des applications capables de rechercher et d'indexer du texte. Il prend en charge certains des formats de documents les plus populaires tels que PDF, HTML, e-mail Outlook, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, Outlook MSG, PST et bien d'autres. L'API prend entièrement en charge la définition du filtrage de documents pour les résultats de recherche. Vous pouvez utiliser plusieurs types de fichiers pour personnaliser vos résultats de recherche, tels que les filtres de chemin de fichier, le filtre d'extension de fichier, le filtre d'attribut et bien d'autres. Il est également possible de combiner des filtres de documents de recherche en utilisant l'opérateur booléen AND, OR & NOT etc.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Définir le filtre de document dans la recherche de doc_documents UPPER via .NET"
      content_left: |
       L'API GroupDocs.Search .NET aide les développeurs de logiciels à ajouter des fonctionnalités de recherche dans leur application .NET. L'exemple de code .NET suivant montre comment appliquer un filtre de document dans la recherche de divers types de documents avec seulement quelques lignes de code.

      title_right: "Appliquer le filtre de document dans la recherche de DOC documents"
      content_right: |
       * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
       * Création d'un index dans le dossier spécifié en appelant l'instance de la classe [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
       * Indexation des documents du dossier spécifié en appelant la méthode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
       * Création d'un objet d'options de recherche [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * Définissez le filtre de document en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Lancer la recherche et afficher les résultats de la recherche
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: "Comment combiner des filtres de recherche de documents via .NET"
      content_left: |
        GroupDocs.Search pour .NET permet aux programmeurs de logiciels de combiner des filtres de documents de recherche lors de la recherche pour contrôler lequel des documents trouvés doit être renvoyé à la suite de la recherche dans l'application C# .NET. Les exemples de code .NET suivants montrent comment combiner des filtres de documents de recherche à l'aide d'opérateurs booléens AND, OR, NOT, etc. dans des applications C#.

      title_right: "Combinez les filtres de recherche de documents dans la recherche de fichiers DOC"
      content_right: |
       * Vous devez d'abord spécifier le chemin d'accès au dossier d'index et au dossier de documents.
       * Création d'un filtre composite AND qui renvoie tous les documents FB2 et EPUB contenant le mot "Einstein" dans leur chemin complet
       * Créez filter1 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Créez filter2 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Combinez les filtres en appelant la méthode [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand)
       * Création d'un filtre composite OU qui renvoie tous les DOC, DOCX, PDF et tous les documents contenant le mot Einstein dans leur chemin complet
       * Créez un filtre3 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Créez un filtre4 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Combinez les filtres en appelant la méthode [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor)
       * Création d'un filtre qui renvoie tous les documents trouvés à l'exception des documents TXT
       * Créez un filtre4 en appelant [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Appy Not filter en appelant la méthode [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot)

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
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