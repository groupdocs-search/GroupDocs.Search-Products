
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: es
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buscar en documentos XLSX usando .NET"
head_description: "GroupDocs.Search for .NET mejora las aplicaciones C# con búsqueda de texto eficiente en varios formatos de documentos empresariales."

############################# Header ############################
title: "Buscar texto en documentos empresariales" 
description: "GroupDocs.Search for .NET permite búsquedas de texto potentes y flexibles en tus documentos. Integra fácilmente la funcionalidad de búsqueda en aplicaciones .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) es una poderosa biblioteca para la búsqueda de texto eficiente e indexación de documentos. Soporta más de 70 formatos de archivo, incluidos documentos estándar de la industria como PDF, Word, Excel y PowerPoint. Mejora el rendimiento de búsqueda con resultados rápidos y precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo buscar en datos XLSX"
    content: |
      [GroupDocs.Search](/search/net/) permite búsquedas de texto eficientes en documentos XLSX, lo que lo hace ideal para aplicaciones .NET.
      
      1. Configura una carpeta para almacenar el índice de búsqueda.
      2. Selecciona la carpeta que contiene tus archivos.
      3. Configura las opciones de búsqueda para procesar solo documentos XLSX.
      4. Ejecuta la búsqueda y recupera resultados.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado de búsqueda"
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
        // Ruta para almacenar el índice de búsqueda reutilizable
        Index index = new Index("c:/MyIndex");

        // Carpeta que contiene documentos
        index.Add("c:/MyDocuments");

        // Buscar solo dentro de formatos de archivo específicos
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".xlsx");

        // Recuperar resultados de búsqueda
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Funciones avanzadas de búsqueda"
  description: "GroupDocs.Search for .NET permite búsquedas de texto sofisticadas en más de 70 formatos de archivo. La indexación mejora la eficiencia de búsqueda y ayuda a gestionar el contenido de los documentos de manera efectiva."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Principales características de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto avanzada"
      content: "Extrae texto relevante de documentos empresariales populares, incluidos PDFs, archivos de Word, presentaciones y hojas de cálculo. Soporta múltiples técnicas de búsqueda como búsqueda difusa, detección de homófonos y comodines."

    # feature loop
    - title: "Indexación optimizada para búsquedas rápidas"
      content: "Construye y reutiliza índices de búsqueda para mejorar la velocidad de búsqueda. La indexación optimiza el rendimiento al buscar en grandes colecciones de documentos."

    # feature loop
    - title: "Soporte para múltiples idiomas"
      content: "Realiza búsquedas en documentos escritos en más de 80 idiomas. Detecta diferentes configuraciones de teclado y variaciones de palabras para mejorar la precisión."

    # feature loop
    - title: "Configuraciones de búsqueda flexibles"
      content: "Refina los resultados de búsqueda con opciones personalizables, incluyendo filtros, expresiones regulares y configuraciones de sensibilidad a mayúsculas."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrar documentos para ser procesados"
      content: |
        Aprende a restringir las búsquedas de documentos utilizando filtros.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Configura un índice que excluya ciertos formatos de archivo
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Especifica el directorio de los documentos
          index.Add("c:/MyDocuments");

          // Recupera resultados de búsqueda
          SearchResult result = index.Search("Lorem");
          
          // Procesa y usa los resultados de búsqueda
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
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/search/formats/searchfilters.xlsx"
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
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Search gratis o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Características clave"
    exclude: "filters"
    description: "Realiza búsquedas de datos precisas y eficientes."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Encuentra datos en tus documentos empresariales"
    exclude: "XLSX"
    description: "GroupDocs.Search soporta más de 70 formatos de archivo, permitiendo el procesamiento y la búsqueda eficiente de documentos de oficina populares."
    items: 
        # format loop 1
        - name: "Filtros de búsqueda para DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Filtros de búsqueda para PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Filtros de búsqueda para PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Filtros de búsqueda para TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Filtros de búsqueda para XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---