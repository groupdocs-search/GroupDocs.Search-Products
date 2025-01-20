---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: fr

############################# Head ############################
head_title: "Recherche et indexation de texte dans des documents | APIs et application Web gratuite"
head_description: "Effectuez des recherches de texte efficaces et l'indexation de données sur PDF, MS Office, OpenDocument et d'autres formats de fichiers populaires à l'aide de nos APIs ou de l'application gratuite Document Search en ligne."

############################# Header ############################
title: "Solution complète de recherche et d'indexation de documents"
description:  |
  Effectuez des recherches de texte et de l'indexation sur PDF, Microsoft Office, OpenOffice et de nombreux autres formats de fichiers documentaires.

  Localisez rapidement des informations dans de grandes collections de documents grâce à des capacités de recherche en texte intégral avancées.

  Personnalisez les fonctionnalités de recherche comme les synonymes, la recherche approximative et la racinisation pour améliorer la précision et les résultats.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choisissez votre plateforme"
  title: "Indépendance de la plateforme"
  description: "GroupDocs.Search est compatible avec les systèmes d'exploitation et les frameworks suivants :"
  details_link_title: "En savoir plus"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Tout autre éditeur de texte
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Fonctionnalités clés de GroupDocs.Search"
  description: "GroupDocs.Search fournit des outils puissants pour l'indexation et la recherche de texte dans des formats de document populaires. Simplifiez et améliorez la gestion des documents grâce à une fonctionnalité de recherche avancée."

  items:
    # items loop
    - icon: "view"
      title: "Recherche de texte avancée"
      content: "Effectuez des recherches de texte rapides et précises dans les documents indexés."

    # items loop
    - icon: "manipulate"
      title: "Options de recherche personnalisables"
      content: "Utilisez des fonctionnalités telles que la recherche approximative, les synonymes et la racinisation pour des résultats plus précis."

    # items loop
    - icon: "merge"
      title: "Prise en charge de plusieurs formats"
      content: "Indexez et recherchez du contenu dans Microsoft Office, PDF, OpenOffice et d'autres formats courants."

    # items loop
    - icon: "additional"
      title: "Indexation efficace"
      content: "Construisez et maintenez rapidement des index pour de grandes collections de documents."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Recherche de texte dans des formats de documents populaires"
  description: "GroupDocs.Search exemples de code"
  items:
    # code sample loop
    - title: "Recherche de texte"
      content: |
       GroupDocs.Search est un outil puissant pour trouver du texte dans des documents. Vous pouvez rechercher à travers plusieurs documents dans divers formats stockés dans un dossier spécifique. Les résultats de la recherche sont sauvegardés dans un dossier séparé, vous permettant d'y accéder et de les réutiliser sans relancer la recherche.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Créez une instance de la classe Index, en spécifiant le dossier pour stocker les index.
            Index index = new Index("\\Index Folder");

            //Spécifiez le chemin vers les documents où la recherche sera effectuée.
            index.Add("\\Documents Folder");

            //Créez une instance de l'objet SearchOptions.
            SearchOptions options = new SearchOptions();

            //Effectuez la recherche pour le texte souhaité.
            SearchResult result = index.Search("ipsum dolor", options);

            //Gérez et traitez les résultats de la recherche.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Créez une instance de la classe Index, en spécifiant le dossier pour stocker les index.
            Index index = new Index("\\Index Folder");

            //Spécifiez le chemin vers les documents où la recherche sera effectuée.
            index.add("\\Documents Folder");

            //Créez une instance de l'objet SearchOptions.
            SearchOptions options = new SearchOptions();

            //Effectuez la recherche pour le texte souhaité.
            SearchResult result = index.search("ipsum dolor", options);

            //Gérez et traitez les résultats de la recherche.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Créez une instance de la classe Index, en spécifiant le dossier pour stocker les index.
            const index = new searchLib.Index('\\Index Folder');

            //Spécifiez le chemin vers les documents où la recherche sera effectuée.
            index.add('\\Documents Folder');

            //Créez une instance de l'objet SearchOptions.
            const options = new searchLib.SearchOptions();

            //Effectuez la recherche pour le texte souhaité.
            const result = index.search('ipsum dolor', options);

            //Gérez et traitez les résultats de la recherche.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Supporte plus de 70 formats de fichiers"
  description: "GroupDocs.Search prend en charge presque tous les formats de fichiers largement utilisés."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistiques de notre produit"
  description: "Découvrez les indicateurs clés qui montrent notre performance, notre portée et notre croissance."

  items:
    # items loop
    - number: "70+"
      title: "Formats pris en charge"
      content: "Nous offrons une compatibilité avec plus de 70 formats de documents populaires."

    # items loop
    - number: "500k"
      title: "Téléchargements NuGet"
      content: "GroupDocs.Search pour .NET a été téléchargé plus de 500 000 fois sur NuGet."

    # items loop
    - number: "12k"
      title: "Téléchargements Maven"
      content: "Les développeurs Java ont téléchargé GroupDocs.Search plus de 12 000 fois depuis Maven."

    # items loop
    - number: "150+"
      title: "Clients satisfaits"
      content: "Des développeurs et des entreprises leaders dans le monde entier comptent sur nos produits pour des solutions innovantes."


############################# Customers ###############################
customers:
  enable: true
  title: "Nos clients satisfaits"
  description: "Les bibliothèques GroupDocs sont approuvées par des marques et des organisations de premier plan à l'échelle mondiale."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Commencez votre expérience dès aujourd'hui !"
  description: "Découvrez GroupDocs.Search gratuitement sur votre plateforme préférée."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Questions fréquemment posées"
  description: "Trouvez des réponses aux questions courantes sur GroupDocs.Search."

  items:
    # items loop
    - question: "Est-ce que GroupDocs.Search nécessite des outils externes pour rechercher des documents ?"
      answer: "Non, GroupDocs.Search fonctionne comme une solution autonome et ne nécessite pas d'outils ou de logiciels supplémentaires comme Adobe Acrobat ou Microsoft Office pour effectuer des recherches."

    # items loop
    - question: "Puis-je tester GroupDocs.Search avant d'acheter ?"
      answer: "Oui, vous le pouvez ! GroupDocs.Search propose un essai gratuit. Vous pouvez explorer ses fonctionnalités, bien que la version d'essai puisse inclure des limitations telles que des filigranes ou une fonctionnalité restreinte. Pour débloquer toutes les fonctionnalités, vous pouvez demander une licence temporaire gratuite de 30 jours. En savoir plus sur la page [licence temporaire](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quelles options de licences sont disponibles ?"
      answer: "Nous proposons plusieurs modèles de licences pour GroupDocs.Search, adaptés à différents besoins. Choisissez une licence en fonction de la taille de votre équipe, du scénario d'utilisation ou de votre besoin d'utiliser le SDK/API pour la distribution aux clients. Pour une utilisation flexible, envisagez une licence à la demande où vous payez en fonction de l'utilisation réelle. En savoir plus sur vos options sur la page [tarification](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Applications Web"
  description: "Explorez GroupDocs.Search avec notre application web gratuite. Effectuez des recherches de texte et de l'indexation sur plus de 70 formats de fichiers populaires directement dans votre navigateur, complètement gratuitement."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Recherchez dans des fichiers PDF, Excel, Word, PowerPoint et d'autres types de fichiers directement depuis votre navigateur web."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Téléchargez des documents DOCX pour effectuer des recherches de texte avancées sans nécessiter d'installation de logiciel."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Testez les capacités d'indexation et de récupération des PDF sur divers formats gratuitement."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---