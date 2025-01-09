---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: es
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: "Biblioteca de Búsqueda de Documentos .NET y Indexación para PDFs, Archivos de Office y Más"
head_description: "Poderosa solución .NET para búsqueda de texto e indexación en documentos como PDFs, Word, Excel, presentaciones, correos electrónicos y formatos web."

############################# Header ############################
title: "Búsqueda Avanzada de Documentos e Indexación con .NET API"
description: "Mejora las aplicaciones .NET con capacidades de búsqueda de texto de vanguardia en formatos de documentos populares."
words:
  for: "para"

actions:
  main: "Descargar Nuget Gratis"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Licenciamiento"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "¡Comienza Tu Aventura Hoy!"
  description: "Explora las capacidades de GroupDocs.Search de forma gratuita o asegura una licencia para desbloquear todo su potencial."

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Buscar Texto en Archivos de Directorio"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Crea un índice para tus documentos
    Index index = new Index("c:/MyIndex");

    // Agrega documentos al índice para búsquedas eficientes
    index.Add("c:/MyDocuments");
    
    // Busca palabras o frases específicas, como
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Descripción General"
  description: "Explora la biblioteca C# de .NET para robustas capacidades de búsqueda de texto e indexación."
  features:
    # feature loop
    - title: "Funciones de Indexación y Búsqueda de .NET"
      content: "Indexa, almacena y procesa datos documentales de manera eficiente con GroupDocs.Search for .NET para operaciones de búsqueda altamente precisas y rápidas."

    # feature loop
    - title: "Combina Índices para Mejorar la Velocidad de Búsqueda"
      content: "GroupDocs.Search for .NET te permite combinar múltiples índices para optimizar el rendimiento. Reduce el impacto de los índices delta combinándolos en un índice integral para búsquedas más fluidas."

    # feature loop
    - title: "Buscar a través de Diferentes Disposiciones de Teclado"
      content: "Maneja fácilmente consultas de búsqueda a través de 88 idiomas y 164 disposiciones de teclado con el reconocimiento inteligente de GroupDocs.Search for .NET."

    # feature loop
    - title: "Búsquedas de Palabras Morfológicas"
      content: "GroupDocs.Search for .NET soporta búsquedas de variaciones de palabras como sustantivos en singular/plural y diferentes formas verbales, personalizables para varios idiomas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Search for .NET funciona sin problemas en los principales sistemas operativos y administradores de paquetes."
  items:
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
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo soportados"
  description: |
    Procesa una extensa gama de formatos de archivo con GroupDocs.Search for .NET. [Ver todos los formatos soportados](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos de Oficina Populares
        * **Portable:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Texto:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formatos de Medios
        * **Formatos de imagen populares:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Imágenes de varias páginas:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Vídeo:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Otros
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Otros:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Características Clave de GroupDocs.Search for .NET"
  description: "Optimiza la gestión de documentos con capacidades avanzadas de búsqueda en formatos populares como PDF, DOCX, XLSX, PPTX y más."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parámetros de Búsqueda Flexibles"
      content: "Utiliza filtros como rangos de fechas y sensibilidad a mayúsculas y minúsculas para refinar tu búsqueda."

    # feature loop
    - icon: "detect"
      title: "Corrección Ortográfica Inteligente"
      content: "Busca frases con corrección ortográfica, comodines y caracteres especiales ignorados."

    # feature loop
    - icon: "collect"
      title: "Resultados de Búsqueda Filtrados"
      content: "Personaliza y filtra los resultados de búsqueda por tipo de documento o criterios."

    # feature loop
    - icon: "get"
      title: "Importación y Exportación de Índices"
      content: "Importa datos, modifica configuraciones de indexación y exporta resultados indexados."

    # feature loop
    - icon: "remove"
      title: "Excluir Datos Irrelevantes"
      content: "Optimiza la indexación omitiendo archivos o palabras específicas."

    # feature loop
    - icon: "style"
      title: "Extracción de URL"
      content: "Convierte texto en formato HTML a archivos y genera enlaces para resultados de búsqueda."

    # feature loop
    - icon: "detect"
      title: "Búsqueda de Alta Velocidad"
      content: "Divide índices grandes en partes más pequeñas para un procesamiento más rápido."

    # feature loop
    - icon: "manipulate"
      title: "Manejo de Datos Simplificado"
      content: "Indexa documentos directamente desde flujos de datos y estructuras."

    # feature loop
    - icon: "compare"
      title: "Detección de Errores Tipográficos"
      content: "Sugiere palabras alternativas y realiza seguimiento de ocurrencias para mejorar la precisión."

    # feature loop
    - icon: "unreadable_characters"
      title: "Soporte para Archivos Comprimidos"
      content: "Indexa archivos ZIP anidados y recupera detalles de archivos dentro de ellos."

    # feature loop
    - icon: "hidden_print"
      title: "Indexación Eficiente"
      content: "Ahorra espacio en disco con indexación compacta y procesa documentos protegidos por contraseña."

    # feature loop
    - icon: "style"
      title: "Sinónimos Personalizados"
      content: "Agrega y gestiona sinónimos para resultados de búsqueda adaptados."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Descubre las potentes capacidades de GroupDocs.Search for .NET con ejemplos prácticos."
  items:
    # code sample loop
    - title: "Aumenta la Productividad con Búsqueda Difusa"
      content: |
        Aprovecha GroupDocs.Search for .NET para un control de contenido flexible y preciso a través de algoritmos de búsqueda avanzados. [Explora más](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Cómo procesar el resultado de búsqueda">}}
        ```csharp {style=abap}
        // Crea un índice
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Configura las opciones de búsqueda
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Busca documentos que contengan la palabra 'agua' o la frase 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Procesa el resultado de la búsqueda
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Búsqueda Avanzada con Expresiones Regulares"
      content: |
        GroupDocs.Search for .NET soporta expresiones regulares para búsquedas precisas. [Aprende técnicas avanzadas](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Cómo buscar utilizando expresiones regulares">}}
        ```csharp {style=abap}   
        // Crea un índice
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Busca la frase en forma de texto

        // El primer carácter de caret al principio indica que esta es una consulta de búsqueda de expresión regular
        string query = "^^(.)\\1{1,}";
        // Busca dos o más caracteres idénticos al principio de una palabra
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
