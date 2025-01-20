---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: en

############################# Head ############################
head_title: "Document Text Search & Indexing | APIs & Free Web App"
head_description: "Perform efficient text search and data indexing on PDF, MS Office, OpenDocument, and other popular file formats using our APIs or the free online Document Search app."

############################# Header ############################
title: "Comprehensive Document Search & Indexing Solution"
description:  |
  Perform text search and indexing on PDF, Microsoft Office, OpenOffice and many other document file formats.

  Quickly locate information in large document collections with advanced full-text search capabilities.

  Customize search features like synonyms, fuzzy search, and stemming to enhance accuracy and results.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Choose your platform"
  title: "Platform independence"
  description: "GroupDocs.Search is compatible with the following operating systems and frameworks:"
  details_link_title: "Learn more"

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
                    Atom <br> Visual Studio Code <br> Any other text editor
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Key Features of GroupDocs.Search"
  description: "GroupDocs.Search provides powerful tools for indexing and searching text in popular document formats. Simplify and enhance document management with advanced search functionality."

  items:
    # items loop
    - icon: "view"
      title: "Advanced text search"
      content: "Perform fast and accurate text searches across indexed documents."

    # items loop
    - icon: "manipulate"
      title: "Customizable search options"
      content: "Utilize features like fuzzy search, synonyms, and stemming for more precise results."

    # items loop
    - icon: "merge"
      title: "Support for multiple formats"
      content: "Index and search content in Microsoft Office, PDF, OpenOffice, and other common formats."

    # items loop
    - icon: "additional"
      title: "Efficient indexing"
      content: "Quickly build and maintain indexes for large document collections."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Searching text in popular document formats"
  description: "GroupDocs.Search code examples"
  items:
    # code sample loop
    - title: "Text Search"
      content: |
       GroupDocs.Search is a powerful tool for finding text in documents. You can search through multiple documents in various formats stored in a specific folder. The search results are saved in a separate folder, allowing you to access and reuse them without running the search again.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Create an instance of the Index class, specifying the folder for storing indexes.
            Index index = new Index("\\Index Folder");

            //Specify the path to the documents where the search will be performed.
            index.Add("\\Documents Folder");

            //Create an instance of the SearchOptions object.
            SearchOptions options = new SearchOptions();

            //Perform the search for the desired text.
            SearchResult result = index.Search("ipsum dolor", options);

            //Handle and process the search results.
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
            // Create an instance of the Index class, specifying the folder for storing indexes.
            Index index = new Index("\\Index Folder");

            //Specify the path to the documents where the search will be performed.
            index.add("\\Documents Folder");

            //Create an instance of the SearchOptions object.
            SearchOptions options = new SearchOptions();

            //Perform the search for the desired text.
            SearchResult result = index.search("ipsum dolor", options);

            //Handle and process the search results.
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

            // Create an instance of the Index class, specifying the folder for storing indexes.
            const index = new searchLib.Index('\\Index Folder');

            //Specify the path to the documents where the search will be performed.
            index.add('\\Documents Folder');

            //Create an instance of the SearchOptions object.
            const options = new searchLib.SearchOptions();

            //Perform the search for the desired text.
            const result = index.search('ipsum dolor', options);

            //Handle and process the search results.
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
  title: "Supports 70+ file formats"
  description: "GroupDocs.Search supports almost all widely used file formats"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Our Product Stats"
  description: "Discover key metrics showcasing our performance, reach, and growth."

  items:
    # items loop
    - number: "70+"
      title: "Supported Formats"
      content: "We provide compatibility with over 70 popular document formats."

    # items loop
    - number: "500k"
      title: "NuGet Downloads"
      content: "GroupDocs.Search for .NET has been downloaded more than 500,000 times on NuGet."

    # items loop
    - number: "12k"
      title: "Maven Downloads"
      content: "Java developers have downloaded GroupDocs.Search over 12,000 times from Maven."

    # items loop
    - number: "150+"
      title: "Satisfied Customers"
      content: "Developers and leading businesses worldwide rely on our products for innovative solutions."


############################# Customers ###############################
customers:
  enable: true
  title: "Our Happy Customers"
  description: "GroupDocs libraries are trusted by leading brands and organizations worldwide."

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
  title: "Start Your Journey Today!"
  description: "Experience GroupDocs.Search for free on your preferred platform."

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
  title: "Frequently Asked Questions"
  description: "Find answers to common questions about GroupDocs.Search."

  items:
    # items loop
    - question: "Does GroupDocs.Search require external tools for searching documents?"
      answer: "No, GroupDocs.Search works as a standalone solution and does not need additional tools or software like Adobe Acrobat or Microsoft Office to perform searches."

    # items loop
    - question: "Can I test GroupDocs.Search before purchasing?"
      answer: "Yes, you can! GroupDocs.Search offers a free trial. You can explore its features, though the trial version may include limitations such as watermarks or restricted functionality. To unlock all features, you can request a free 30-day temporary license. Learn more on the [temporary license](https://purchase.groupdocs.com/temporary-license/) page."

    # items loop
    - question: "What licensing options are available?"
      answer: "We provide several licensing models for GroupDocs.Search, tailored to different needs. Choose a license based on your team size, usage scenario, or whether you need the SDK/API for client distribution. For flexible usage, consider a metered license where you pay based on actual usage. Learn more about your options on the [pricing](https://purchase.groupdocs.com/pricing/search/net/) page."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Web Apps"
  description: "Explore GroupDocs.Search with our free web application. Perform text searches and indexing on over 70 popular file formats directly in your browser—completely free."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Search within PDF, Excel, Word, PowerPoint, and other file types straight from your web browser."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Upload DOCX to perform advanced text searches without needing to install software."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Test PDFs indexing and retrieval capabilities on various formats for free."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---