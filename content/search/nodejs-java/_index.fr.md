---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: fr
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Bibliothèque de recherche et d'indexation de texte Node.js pour documents, PDF, fichiers bureautiques et web"
head_description: "Solution avancée de recherche de texte pour les applications Node.js pour rechercher, indexer et collecter des données à partir de documents : PDF, Word, Excel, présentations, e-mails et formats de fichiers web."

############################# Header ############################
title: "Recherche et indexation de documents utilisant l'API Node.js"
description: "Améliorez les applications Node.js en implémentant la recherche de texte dans tous les formats de documents populaires."
words:
  for: "pour"

actions:
  main: "Téléchargement gratuit de NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licences"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Commencez votre expérience dès aujourd'hui !"
  description: "Explorez les capacités de GroupDocs.Search gratuitement ou obtenez une licence pour débloquer son plein potentiel."

release:
  title: "Version {0} publiée"
  notes: "Voir les nouveautés"
  downloads: "Téléchargements"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Effectuer une recherche de texte dans un dossier avec JavaScript"
  more: "Plus d'exemples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Créez un index pour vos documents
    const index = new searchLib.Index('c:/MyIndex');

    // Ajoutez des documents à l'index pour une recherche efficace
    index.add('c:/MyDocuments');
    
    // Recherchez des mots ou des phrases spécifiques, tels que
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Aperçu de GroupDocs.Search"
  description: "Bibliothèque Node.js JavaScript pour la recherche de texte"
  features:
    # feature loop
    - title: "Opérations d'indexation et de recherche Node.js"
      content: "L'indexation dans GroupDocs.Search for Node.js via Java collecte, stocke et analyse les données pour des opérations de recherche précises et efficaces. Ces index sont couramment utilisés pour effectuer des recherches."

    # feature loop
    - title: "Fusionner plusieurs index pour améliorer l'efficacité de recherche"
      content: "GroupDocs.Search for Node.js via Java API permet la fusion de plusieurs index en un seul. Des modifications fréquentes créent plusieurs index de delta, ce qui peut ralentir les performances de recherche. Notre solution fusionne ces index de delta en un index commun, contenant toutes les informations provenant des index de delta fusionnés, améliorant ainsi considérablement l'efficacité de recherche tout en maintenant les index de delta inchangés. Différentes fonctionnalités peuvent être configurées pour peaufiner ce processus."

    # feature loop
    - title: "Reconnaître les requêtes de recherche à partir de différentes mises en page de clavier"
      content: "GroupDocs.Search for Node.js via Java reconnaît les requêtes de recherche qui ne correspondent pas à la mise en page du clavier. Actuellement, 88 langues et 164 différentes mises en page de clavier sont prises en charge."

    # feature loop
    - title: "Rechercher à l'aide de formes morphologiques de mots"
      content: "Avec GroupDocs.Search for Node.js via Java, vous pouvez rechercher différentes formes de mots, telles que les noms singuliers et pluriels, ou toutes les formes d'un verbe. L'anglais et les langues non anglaises peuvent être personnalisés pour des formes de mots spécifiques."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Search for Node.js via Java prend en charge tous les systèmes d'exploitation populaires et gestionnaires de packages."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formats de fichiers pris en charge"
  description: |
    GroupDocs.Search for Node.js via Java permet de traiter une large gamme de formats de fichiers. [Explorez la liste complète](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formats de bureau populaires
        * **Portable:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Texte:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formats multimédia
        * **Formats d'image populaires:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Images multipages:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Vidéo:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Autres
        * **E-mail:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Autres:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Fonctionnalités de GroupDocs.Search for Node.js via Java"
  description: "Contrôlez le contenu des documents commerciaux grâce à notre moteur de recherche avancé, prenant en charge les formats de fichiers populaires, y compris PDF, DOCX, XLSX, PPTX, et plus encore."

  items:
    # feature loop
    - icon: "document_info"
      title: "Paramètres flexibles"
      content: "Utilisez des plages de dates et la sensibilité à la casse comme paramètres de recherche"

    # feature loop
    - icon: "detect"
      title: "Recherche avec vérification orthographique"
      content: "Utilisez des phrases de recherche avec vérification orthographique et caractères génériques, en sautant les caractères spéciaux dans les requêtes"

    # feature loop
    - icon: "collect"
      title: "Filtrage des résultats"
      content: "Configurez le filtrage des documents dans les résultats de recherche"

    # feature loop
    - icon: "get"
      title: "Importation et exportation"
      content: "Effectuez des importations ou utilisez une liste pour modifier les caractères lors de l'indexation et exportez dans un fichier"

    # feature loop
    - icon: "remove"
      title: "Exclusion des données non nécessaires"
      content: "Ignorer sélectivement l'indexation pour des fichiers spécifiques et des mots spécifiques pour une indexation plus rapide"

    # feature loop
    - icon: "style"
      title: "Traitement des URL"
      content: "Extrayez le texte au format HTML dans un fichier et générez une URL pour naviguer dans les résultats de recherche en HTML"

    # feature loop
    - icon: "detect"
      title: "Recherche rapide"
      content: "Divisez la recherche en morceaux plus petits pour rechercher rapidement de grands index"

    # feature loop
    - icon: "manipulate"
      title: "Traitement des flux"
      content: "Indexez les documents à partir de flux et de structures de données"

    # feature loop
    - icon: "compare"
      title: "Gérer les erreurs de frappe"
      content: "Permettre un nombre exact d'occurrences pour chaque mot trouvé afin d'offrir des suggestions alternatives en cas d'erreur typographique"

    # feature loop
    - icon: "unreadable_characters"
      title: "Support des archives"
      content: "Indexez les archives compressées à l'intérieur d'autres archives ZIP et récupérez la liste des fichiers indexés dans une archive"

    # feature loop
    - icon: "hidden_print"
      title: "Économie d'espace disque"
      content: "Économisez de l'espace avec une indexation compacte et indexez des documents protégés par mot de passe"

    # feature loop
    - icon: "style"
      title: "Synonymes personnalisés"
      content: "Ajoutez des synonymes anglais au dictionnaire de synonymes par défaut"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemples de code"
  description: "Explorez les fonctionnalités de GroupDocs.Search for Node.js via Java avec des exemples"
  items:
    # code sample loop
    - title: "Utilisez la recherche 'floue' pour améliorer la productivité"
      content: |
        Profitez de la flexibilité de GroupDocs.Search for Node.js via Java pour améliorer le contrôle du contenu des documents grâce à des algorithmes de recherche sophistiqués. [En savoir plus](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Comment traiter le résultat de la recherche">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Créez un index
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Configurez les options de recherche
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Recherchez des documents contenant le mot 'eau' ou la phrase 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Traitez le résultat de la recherche
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Les expressions régulières sont disponibles pour des scénarios de recherche avancés"
      content: |
        GroupDocs.Search for Node.js via Java vous permet d'utiliser des expressions régulières afin de restreindre les résultats de recherche. [Plongez dans des techniques de recherche avancées](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Comment rechercher avec des expressions régulières">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Créez un index
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Recherchez la phrase sous forme de texte

        // Le premier caractère de caret au début indique qu'il s'agit d'une requête de recherche d'expressions régulières
        const query = '^^(.)\\1{1,}';
        // Recherchez deux caractères identiques ou plus au début d'un mot
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
