---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: es
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Solución de Búsqueda y Indexación de Documentos Java para PDFs, Archivos de Office y Contenido Web"
head_description: "Búsqueda de texto poderosa e indexación para aplicaciones Java. Busca y organiza datos en PDFs, Word, Excel, presentaciones, correos electrónicos y formatos web."

############################# Header ############################
title: "Búsqueda Eficiente de Documentos e Indexación con Java API"
description: "Potencia aplicaciones Java con robustas características de búsqueda de texto en todos los formatos populares de documentos."
words:
  for: "para"

actions:
  main: "Descargar Maven Gratis"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Licenciamiento"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "¡Comienza Tu Aventura Hoy!"
  description: "Explora las capacidades de GroupDocs.Search de forma gratuita o asegura una licencia para desbloquear todo su potencial."

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"

code:
  title: "Buscar Texto en Archivos Usando Java"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Crea un índice para tus documentos
    Index index = new Index("c:/MyIndex");

    // Agrega documentos al índice para búsquedas eficientes
    index.add("c:/MyDocuments");
    
    // Busca palabras o frases específicas, como
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Descripción General"
  description: "Descubre las poderosas capacidades de búsqueda de texto de la biblioteca Java de Java."
  features:
    # feature loop
    - title: "Operaciones de Indexación y Búsqueda en Java"
      content: "Con GroupDocs.Search for Java, puedes recopilar, almacenar y analizar datos de manera eficiente para crear índices detallados para búsquedas más rápidas y precisas."

    # feature loop
    - title: "Optimiza la Búsqueda Combinando Índices"
      content: "Combina fácilmente múltiples índices con GroupDocs.Search for Java para racionalizar las búsquedas. Reduce el impacto de los índices delta más pequeños al consolidarlos en un único índice de alto rendimiento."

    # feature loop
    - title: "Soporte para Disposiciones de Teclado Multilingües"
      content: "Busca a través de diferentes idiomas y disposiciones de teclado con GroupDocs.Search for Java. Soporta 88 idiomas y 164 configuraciones de teclado para una versatilidad inigualable."

    # feature loop
    - title: "Capacidades de Búsqueda Morfológica"
      content: "Encuentra diferentes formas de palabras como sustantivos en singular/plural o variaciones verbales utilizando GroupDocs.Search for Java. Personaliza las opciones de búsqueda para inglés y otros idiomas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Search for Java es compatible con principales sistemas operativos y administradores de paquetes."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo soportados"
  description: |
    Trabaja con una amplia gama de formatos de archivo usando GroupDocs.Search for Java. [Ver la lista completa](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Características de GroupDocs.Search for Java"
  description: "Gestiona el contenido de documentos de manera efectiva con capacidades avanzadas de búsqueda que soportan formatos como PDF, DOCX, XLSX, PPTX y más."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parámetros de Búsqueda Personalizables"
      content: "Refina las búsquedas usando rangos de fecha y filtros de sensibilidad a mayúsculas y minúsculas."

    # feature loop
    - icon: "detect"
      title: "Corrección Ortográfica Mejorada"
      content: "Busca de manera eficiente con corrección ortográfica, comodines y al ignorar caracteres especiales."

    # feature loop
    - icon: "collect"
      title: "Resultados de Búsqueda Filtrados"
      content: "Aplica filtros para centrar los resultados de búsqueda en tipos específicos de documentos o criterios."

    # feature loop
    - icon: "get"
      title: "Importar y Exportar Datos de Índices"
      content: "Importa fácilmente datos para indexar o exporta resultados a archivos para su uso posterior."

    # feature loop
    - icon: "remove"
      title: "Omitir Archivos Innecesarios"
      content: "Optimiza la indexación excluyendo archivos o palabras específicas."

    # feature loop
    - icon: "style"
      title: "Procesamiento de HTML y URL"
      content: "Extrae contenido HTML a archivos y genera URLs para navegación a través de los resultados de búsqueda."

    # feature loop
    - icon: "detect"
      title: "Búsqueda Rápida en Índices Grandes"
      content: "Acelera las operaciones de búsqueda dividiendo índices grandes en partes manejables."

    # feature loop
    - icon: "manipulate"
      title: "Indexación Basada en Flujos"
      content: "Indexa datos directamente desde flujos o estructuras de datos."

    # feature loop
    - icon: "compare"
      title: "Manejo de Consultas Mal Escritas"
      content: "Detecta errores tipográficos y sugiere palabras alternativas para mejorar la precisión de búsqueda."

    # feature loop
    - icon: "unreadable_characters"
      title: "Soporte Integral para Archivos Comprimidos"
      content: "Indexa archivos dentro de archivos comprimidos y recupera listas detalladas de archivos dentro de ZIP."

    # feature loop
    - icon: "hidden_print"
      title: "Indexación que Ahorra Espacio"
      content: "Indexa de forma compacta para ahorrar espacio en disco y procesa archivos protegidos por contraseña."

    # feature loop
    - icon: "style"
      title: "Soporte para Sinónimos Personalizados"
      content: "Amplía el diccionario de sinónimos para mejorar la precisión de búsqueda con opciones personalizadas."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Prueba las características de GroupDocs.Search for Java con estos ejemplos de código."
  items:
    # code sample loop
    - title: "Aumenta la Precisión de Búsqueda con Coincidencias Difusas"
      content: |
        Explora la flexibilidad de GroupDocs.Search for Java para gestionar contenido con capacidades avanzadas de búsqueda difusa. [Aprende más](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Cómo procesar el resultado de búsqueda">}}
        ```java {style=abap}
        // Crea un índice
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Configura las opciones de búsqueda
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Busca documentos que contengan la palabra 'agua' o la frase 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Procesa el resultado de la búsqueda
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Refina los Resultados con Expresiones Regulares"
      content: |
        Utiliza expresiones regulares en GroupDocs.Search for Java para crear resultados de búsqueda precisos y detallados. [Descubre técnicas avanzadas](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Cómo buscar utilizando expresiones regulares">}}
        ```java {style=abap}   
        // Crea un índice
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Busca la frase en forma de texto

        // El primer carácter de caret al principio indica que esta es una consulta de búsqueda de expresión regular
        String query = "^^(.)\\1{1,}";
        // Busca dos o más caracteres idénticos al principio de una palabra
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
