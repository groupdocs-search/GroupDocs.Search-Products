
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: es
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Búsqueda Sensible a Mayúsculas en TXT Usando .NET"
head_description: "La API GroupDocs.Search for .NET permite a los desarrolladores de C# realizar búsquedas sensibles a mayúsculas en varios documentos."

############################# Header ############################
title: "Búsqueda Sensible a Mayúsculas" 
description: "GroupDocs.Search for .NET facilita la creación de consultas avanzadas de búsqueda sensible a mayúsculas dentro de tus aplicaciones .NET."
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
       [GroupDocs.Search for .NET](/search/net/) es una biblioteca robusta para la búsqueda y el indexado de texto en documentos. Soporta más de 70 formatos de archivo, incluidos PDF, Word, PowerPoint, Excel, imágenes y archivos ZIP, asegurando un manejo eficiente de grandes volúmenes de datos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo Realizar Búsqueda Sensible a Mayúsculas en Documentos TXT"
    content: |
      [GroupDocs.Search](/search/net/) simplifica la búsqueda sensible a mayúsculas en documentos TXT. Úsalo para refinar resultados en aplicaciones .NET.
      
      1. Define la carpeta para almacenar el índice de búsqueda.
      2. Elige la carpeta que contiene archivos TXT.
      3. Ejecuta la búsqueda y recupera resultados.
      4. Procesa los resultados.
   
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
        // Establecer la ruta a la carpeta del índice
        Index index = new Index("c:/MyIndex");

        // Especificar la carpeta que contiene los documentos a buscar
        index.Add("c:/MyDocuments");

        // Habilitar la búsqueda sensible a mayúsculas en las opciones
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Ejecutar la búsqueda
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Funciones Avanzadas para la Búsqueda e Indexado de Documentos"
  description: "La biblioteca GroupDocs.Search for .NET simplifica la búsqueda de texto y el indexado a través de más de 70 formatos de archivo. Localiza y gestiona información con potentes herramientas de búsqueda."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Características Clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda Avanzada de Texto"
      content: "Busca texto en varios formatos de archivo, incluidos PDFs, documentos de Word, hojas de cálculo y presentaciones. Utiliza opciones como coincidencias exactas, búsqueda difusa y comodines para obtener resultados precisos."

    # feature loop
    - title: "Indexar Grandes Conjuntos de Datos"
      content: "Crea y mantiene índices para búsquedas más rápidas. Un indexado organizado simplifica la búsqueda en colecciones extensas de documentos."

    # feature loop
    - title: "Soporte Multilingüe"
      content: "Busca a través de documentos en más de 80 idiomas, con soporte para diferentes disposiciones de teclado y formas de palabras para resultados más precisos."

    # feature loop
    - title: "Opciones de Búsqueda Personalizables"
      content: "Personaliza la configuración de búsqueda con sensibilidad a mayúsculas, filtros por rango de fechas y la capacidad de excluir palabras o datos específicos durante el indexado."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Uso de Consultas de Búsqueda Sensibles a Mayúsculas"
      content: |
        Este ejemplo muestra cómo utilizar consultas sensibles a mayúsculas para buscar documentos TXT.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Establecer la carpeta para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Especificar la ruta a los documentos que se van a buscar
          index.Add("c:/MyDocuments");

          // Crear una consulta de búsqueda
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Habilitar opciones de búsqueda sensibles a mayúsculas
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Buscar texto en los documentos
          SearchResult result = index.Search(wordQuery, options);
          
          // Procesar los resultados de la búsqueda
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
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
    title: "Descubre Funciones Clave"
    exclude: "case-sensitive"
    description: "Explora funcionalidades de búsqueda avanzadas y eficientes."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar Formatos de Documento Populares"
    exclude: "TXT"
    description: "GroupDocs.Search soporta más de 70 formatos de archivo. Personaliza las reglas de búsqueda y utiliza el indexado para ahorrar tiempo y esfuerzo."
    items: 
        # format loop 1
        - name: "Búsqueda sensible a mayúsculas y minúsculas en DOCX"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas en PDF"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Búsqueda sensible a mayúsculas y minúsculas en PPTX"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Búsqueda sensible a mayúsculas y minúsculas en TXT"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Búsqueda sensible a mayúsculas y minúsculas en XLSX"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---