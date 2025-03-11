
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: es
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buscar DOCX en .NET utilizando operadores booleanos"
head_description: "La API de GroupDocs.Search for .NET permite a los desarrolladores de C# buscar contenido de documentos utilizando operadores booleanos como AND, OR y NOT."

############################# Header ############################
title: "Búsqueda de texto con lógica booleana" 
description: "GroupDocs.Search for .NET facilita la creación de consultas de búsqueda avanzadas utilizando operadores booleanos (AND, OR, NOT) dentro de tus aplicaciones .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Gratis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Aprende más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) es una biblioteca completa para buscar e indexar texto en documentos. Soporta más de 70 formatos de archivo, como PDF, Word, PowerPoint, Excel, imágenes y archivos ZIP, lo que permite un procesamiento eficiente de grandes volúmenes de información.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo buscar contenido de documentos DOCX utilizando lógica booleana"
    content: |
      [GroupDocs.Search](/search/net/) hace que buscar contenido de documentos DOCX sea sencillo. Proporciona condiciones de búsqueda de lógica booleana para refinar los resultados en aplicaciones .NET.
      
      1. Especifica la carpeta para almacenar el índice de búsqueda.
      2. Elige la carpeta que contiene archivos DOCX.
      3. Ejecuta la búsqueda y recupera los resultados.
      4. Procesa los resultados.
   
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
        // Configura la ruta a la carpeta del índice
        Index index = new Index("c:/MyIndex");

        // Especifica la carpeta que contiene los documentos a buscar
        index.Add("c:/MyDocuments");

        // Ejecuta una búsqueda utilizando una consulta compleja
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explora características avanzadas para búsqueda e indexación de documentos"
  description: "La biblioteca GroupDocs.Search for .NET simplifica la búsqueda de texto y la indexación para más de 70 formatos de archivo. Localiza y gestiona información de manera efectiva con herramientas de búsqueda avanzadas."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Características principales de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto poderosa"
      content: "Busca texto a través de varios tipos de archivos, incluidos PDFs, documentos de Word, presentaciones de PowerPoint y hojas de cálculo. Utiliza funciones como coincidencias exactas, búsquedas difusas y comodines para refinar resultados."

    # feature loop
    - title: "Indexar grandes conjuntos de datos"
      content: "Crea y mantiene índices para búsquedas más rápidas. La indexación estructura y organiza los datos, facilitando la búsqueda en colecciones extensas de documentos."

    # feature loop
    - title: "Soporte para múltiples idiomas"
      content: "Busca documentos en más de 80 idiomas, con soporte para diferentes disposiciones de teclado y formas morfológicas de palabras que mejoran la precisión de búsqueda."

    # feature loop
    - title: "Opciones de búsqueda personalizables"
      content: "Ajusta la configuración de búsqueda con funciones como sensibilidad a mayúsculas, filtros de rango de fechas y la posibilidad de excluir palabras o datos específicos durante la indexación."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando consultas de búsqueda booleanas avanzadas"
      content: |
        Este ejemplo demuestra cómo aplicar consultas booleanas para buscar documentos DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Establece la carpeta para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Especifica la ruta a los documentos a buscar
          index.Add("c:/MyDocuments");

          // Crea una consulta de búsqueda utilizando lógica booleana
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Recupera los resultados de búsqueda
          SearchResult result = index.Search(booleanQuery);
          
          // Procesa los resultados de búsqueda
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
            link: "/examples/search/formats/searchboolean.docx"
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
    title: "Descubre características clave"
    exclude: "boolean"
    description: "Explora funcionalidades de búsqueda avanzadas y eficientes."
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
    title: "Buscar en formatos de documento populares"
    exclude: "DOCX"
    description: "GroupDocs.Search soporta más de 70 formatos de archivo. Personaliza las reglas de búsqueda y aprovecha la indexación para ahorrar tiempo y esfuerzo."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---