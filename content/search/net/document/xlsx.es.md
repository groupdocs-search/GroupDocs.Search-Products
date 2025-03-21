
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: es
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Buscar documentos XLSX en .NET con GroupDocs.Search"
head_description: "Utilice GroupDocs.Search for .NET para realizar búsquedas textuales eficientes en varios formatos de documento con C#."

############################# Header ############################
title: "Búsqueda avanzada de texto en documentos" 
description: "GroupDocs.Search for .NET simplifica la búsqueda de texto en formatos de documentos populares, permitiéndole crear consultas de búsqueda potentes en sus aplicaciones de .NET."
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
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) es una biblioteca potente diseñada para la búsqueda y el indexado de texto completo en documentos. Soporta más de 70 formatos de archivo, incluyendo PDF, Word, PowerPoint, Excel, imágenes y archivos ZIP, asegurando resultados de búsqueda rápidos y precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo realizar una búsqueda de texto en documentos XLSX"
    content: |
      [GroupDocs.Search](/search/net/) permite operaciones de búsqueda de contenido avanzadas en documentos XLSX, permitiendo resultados de búsqueda refinados en aplicaciones .NET.
      
      1. Configure la carpeta para almacenar el índice de búsqueda.
      2. Elija la carpeta que contiene archivos XLSX.
      3. Configure opciones de búsqueda adicionales.
      4. Ejecute la búsqueda y revise los resultados.
   
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
        // Defina la ruta para el índice de búsqueda
        Index index = new Index("c:/MyIndex");

        // Seleccione la carpeta que contiene los documentos a buscar
        index.Add("c:/MyDocuments");

        // Habilite la búsqueda de homófonos para encontrar palabras que suenan similares
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Ejecute una consulta de búsqueda compleja
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Funciones avanzadas de búsqueda e indexación"
  description: "GroupDocs.Search for .NET mejora la búsqueda de texto y la indexación en más de 70 formatos de archivo, proporcionando herramientas eficientes para localizar y gestionar información."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto potente"
      content: "Busque texto en múltiples tipos de documentos, incluidos PDFs, documentos de Word, presentaciones de PowerPoint y hojas de cálculo. Utilice características como coincidencias exactas, búsqueda difusa y comodines para refinar sus resultados."

    # feature loop
    - title: "Indexación rápida para grandes conjuntos de datos"
      content: "Cree y gestione índices de búsqueda para una recuperación rápida de información. La indexación optimiza las búsquedas en colecciones extensas de documentos."

    # feature loop
    - title: "Soporte multilingüe"
      content: "Realice búsquedas en más de 80 idiomas, con soporte para diferentes distribuciones de teclado y variaciones de palabras para mejorar la precisión."

    # feature loop
    - title: "Configuraciones de búsqueda personalizables"
      content: "Ajuste los parámetros de búsqueda con opciones como sensibilidad a mayúsculas, filtros de rango de fechas y exclusiones de palabras para obtener mejores resultados."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ejecutando consultas de búsqueda avanzadas"
      content: |
        Este ejemplo demuestra cómo aplicar consultas de búsqueda para documentos XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Defina la carpeta para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Especifique la ruta a los archivos del documento
          index.Add("c:/MyDocuments");

          // Proporcione una contraseña para documentos protegidos
          index.Dictionaries.DocumentPasswords.Add("protected.xlsx", "123456");

          // Habilite la búsqueda difusa para encontrar palabras similares
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Recupere los resultados de la búsqueda
          SearchResult result = index.Search("Loarem", options);
          
          // Procese la salida de la búsqueda
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    title: "Explore las características clave"
    exclude: "document"
    description: "Aproveche las funcionalidades de búsqueda avanzadas y de alto rendimiento."
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
    title: "Busque en sus documentos empresariales"
    exclude: "XLSX"
    description: "GroupDocs.Search admite más de 70 formatos de archivo, incluidos documentos de oficina, permitiendo búsquedas rápidas y eficientes con capacidades de indexación."
    items: 
        # format loop 1
        - name: "Buscar en documento DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Buscar en documento PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Buscar en documento PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Buscar en documento TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Buscar en documento XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---