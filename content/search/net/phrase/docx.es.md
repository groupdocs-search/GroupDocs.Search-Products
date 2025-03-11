
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: es
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buscar frases en DOCX utilizando .NET"
head_description: "GroupDocs.Search for .NET mejora las aplicaciones de C# con potentes capacidades de búsqueda de frases para el contenido de los documentos."

############################# Header ############################
title: "Buscar frases en documentos" 
description: "Encuentra frases específicas rápidamente con GroupDocs.Search for .NET. Integra una funcionalidad de búsqueda eficiente en tus aplicaciones de .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Funciones de GroupDocs.Search"
    link: "/search/net/"
    link_title: "Aprende más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) es una poderosa biblioteca para indexar y buscar texto en documentos. Soporta más de 70 formatos de archivo, incluidos PDF, documentos de Word, hojas de Excel, imágenes y archivos ZIP, lo que permite obtener resultados de búsqueda rápidos y precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo buscar frases en documentos DOCX"
    content: |
      [GroupDocs.Search](/search/net/) simplifica la búsqueda en documentos DOCX. Utiliza diversas opciones para refinizar los resultados de búsqueda en aplicaciones .NET.
      
      1. Configura la carpeta del índice de búsqueda.
      2. Especifica la carpeta que contiene archivos DOCX.
      3. Configura la configuración de búsqueda.
      4. Recupera y procesa los resultados de búsqueda.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Ruta para almacenar el índice de búsqueda
        Index index = new Index("c:/MyIndex");

        // Carpeta que contiene documentos
        index.Add("c:/MyDocuments");

        // Configurar opciones de búsqueda
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Ejecutar la búsqueda
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Descubre el motor de búsqueda de documentos de .NET"
  description: "GroupDocs.Search for .NET permite búsquedas de frases en más de 70 formatos de archivo. Localiza y gestiona datos con capacidades avanzadas de búsqueda."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de frases"
      content: "Busca frases exactas en documentos de negocios, incluyendo PDF, archivos de Word, presentaciones y hojas de cálculo. Utiliza caracteres comodín y otras opciones si la frase exacta es desconocida."

    # feature loop
    - title: "Indexación eficiente de datos"
      content: "Crea y reutiliza índices de búsqueda para acelerar las búsquedas de documentos. La indexación estructura los datos de manera eficiente, haciendo que las búsquedas de frases sean más rápidas."

    # feature loop
    - title: "Soporte multilingüe"
      content: "Busca documentos en más de 80 idiomas. Soporta diferentes distribuciones de teclado y formas morfológicas de palabras para mayor precisión en las búsquedas."

    # feature loop
    - title: "Opciones de búsqueda flexibles"
      content: "Personaliza las búsquedas con características como sensibilidad a mayúsculas, búsqueda difusa y homófonas, filtrado de documentos y más."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Uso de técnicas de búsqueda avanzadas"
      content: |
        Aprende a crear consultas para buscar en DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Especificar la carpeta para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Establecer la ruta a los documentos para la búsqueda
          index.Add("c:/MyDocuments");

          // Crear una consulta para una frase específica
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Recuperar los resultados de búsqueda
          SearchResult result = index.Search(query);
          
          // Procesar y utilizar los resultados
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.docx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Prueba las características de GroupDocs.Search de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Características avanzadas"
    exclude: "phrase"
    description: "Utiliza funciones de búsqueda potentes y eficientes."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Búsqueda de frases en documentos de negocios"
    exclude: "DOCX"
    description: "GroupDocs.Search soporta búsquedas en más de 70 formatos de documentos. Utiliza opciones avanzadas e indexación para agilizar tu proceso de búsqueda."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---