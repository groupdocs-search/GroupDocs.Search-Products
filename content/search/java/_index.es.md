---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API de indexación y búsqueda de texto Java para documentos, PDF, Office y Web"
head_description: "API de búsqueda de texto avanzada para aplicaciones Java para buscar, indexar y recuperar datos de documentos: PDF, Word, Excel, presentaciones, correo electrónico y formatos de archivo web."

############################# Header ############################
title: "Buscar e indexar documentos a través de la API de Java"
description: "Cree aplicaciones Java para realizar la manipulación de búsqueda de texto en todos los formatos de documentos populares."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "/border/groupdocs-search-java.svg"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Visión de conjunto"

            # button loop
            - link: "#features"
              text: "Características"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/search"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Search for Java le permite producir aplicaciones comerciales que permiten a sus usuarios finales realizar operaciones de búsqueda como nunca antes. Nuestra API de Java permite a los usuarios operar funciones de búsqueda de texto de nivel básico a avanzado. Crear y fusionar múltiples índices. Utilice consultas simples, booleanas, de expresión regular (regex), aproximadas y de otro tipo para realizar búsquedas rápidas e inteligentes en los índices. Puede obtener la información requerida de archivos, documentos, correos electrónicos y archivos comprimidos, ya que GroupDocs.Search para Java es compatible con todos los formatos de archivo populares.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Search para Java:

        left:
          enable: true
          icon: "fas fa-search"
          title: "Indexación"
          content: |
            * Crear y administrar
            * Combinar varios índices
            * Multi-Threading Async Indexación
            * Compact Indexación
            * Archived Files Indexación
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "Búsqueda avanzada y consultas de búsqueda"
          content: |
            * Búsqueda borrosa
            * Búsqueda de sinónimos
            * Búsqueda de correo electrónico
            * Manejo de Términos Homofónicos
            * Búsqueda de archivos protegidos
            * Sencillo
            * Comodín
            * Expresión regular (regex)
            * facetado y booleano
            * Distingue mayúsculas y minúsculas
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Search for Java es compatible con todos los [formatos de archivo de documentos](https://docs.groupdocs.com/search/java/supported-document-formats/), incluidos: oficina de Microsoft, imágenes, diagramas y muchos otros.

        left:
          enable: true
          table:
            # table loop
            - title: "Formatos de oficina de Microsoft"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Project**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Otros formatos"
              content: |
                * **Formato de documento portátil**: PDF
                * **Documento abierto**: ODT, OTT, ODS, OTS, ODP
                * **Correo electrónico**: PST, OST, MSG, EML, EMLX
                * **Formatos de archivos web**: XML, HTM, HTML, XHTML, MHT, MHTML
                * **Audio**: MP3, WAV
                * **Vídeo**: AVI, MOV, QT, FLV, ASF
                * **Texto**: TXT
                * **Formato de texto enriquecido**: RTF
                * **Archivo Documentación Markdown**: MD
                * **Imágenes**: BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **Otros**: TORRENT, ZIP, DCM, DJVU, EPUB, FB2

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Search for Java apoya siguiendo Sistemas operativos, Marcos y administradores de paquetes:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * Java 7 (1.7) y superior

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entornos de desarrollo"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Herramienta de automatización de compilación"
              content: |
                * Maven

############################# Características ############################
features:
    enable: true
    title: "GroupDocs.Search for Java Características"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Cree un índice en el disco o en la memoria con Async Multithreading"

      # feature loop
      - icon: "fas fa-eye"
        content: "Ver el progreso de creación y actualización del índice"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Omitir selectivamente la indexación de archivos específicos y omitir palabras específicas para indexar más rápido"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Realizar Importación o Usar Lista para Modificar Caracteres durante la Indexación y Exportación a un Archivo"

      # feature loop
      - icon: "fas fa-code"
        content: "Recargar índice en caso de error de indexación y alertar al usuario por configuraciones contradictorias"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Notificación de estado de índice con respecto a los últimos archivos procesados"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Indexe archivos comprimidos dentro de otros archivos ZIP y obtenga una lista de archivos indexados en un archivo"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Ahorre espacio mediante la indexación compacta y la indexación de documentos protegidos con contraseña"

      # feature loop
      - icon: "fas fa-print"
        content: "Configure y realice búsquedas de sinónimos y trate inteligentemente los términos homofónicos"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Utilice el intervalo de fechas y la distinción entre mayúsculas y minúsculas como parámetros de búsqueda"

      # feature loop
      - icon: "fas fa-lock"
        content: "Cree un índice para buscar y examinar mensajes de correo electrónico a través de Aspose.Email API"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Use frases de búsqueda con corrector ortográfico y comodín y omita caracteres especiales en las consultas"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Cree un árbol de un solo objeto combinando múltiples consultas"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Divida la búsqueda en fragmentos más pequeños para buscar rápidamente índices enormes"

      # feature loop
      - icon: "fas fa-heading"
        content: "Indexar documentos de flujos y estructuras de datos"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Configurar el filtrado de documentos en los resultados de búsqueda"

      # feature loop
      - icon: "fas fa-cube"
        content: "Agregar sinónimos en inglés al diccionario de sinónimos predeterminado"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Habilite el número exacto de ocurrencias para cada palabra encontrada para ofrecer sugerencias de palabras alternativas en caso de errores ortográficos"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Agregar atributos de texto a documentos indexados sin volver a indexar"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Realizar Operaciones de Indexación y Búsqueda Basadas en Caracteres"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Índice de metadatos de formatos de documentos no textuales"

    more_feature:
      # more_feature_loop
      - title: "Indexación and Search Operation"
        content: |
          GroupDocs.Search for Java utiliza Indexación para recopilar datos, almacenarlos y analizarlos para operaciones de búsqueda precisas y eficientes. GroupDocs.Search for Java utiliza dichos índices con frecuencia para realizar búsquedas.

          * **Crear índice**: Crear carpeta de índice y agregar/indexar documentos a esa carpeta.
          * **Cargar índice**: Cargue un índice existente.
          * **Agregar documentos al índice**: agregue documentos al índice existente, de forma asíncrona.
          * **Actualizar índice**: actualice el índice existente cada vez que se modifique, agregue o elimine un documento. Esto mantiene los resultados de búsqueda actualizados.
          
          ```java
          // Creando índice
          Índice índice = índice nuevo ("c:\\MiÍndice");
          // Agregar documentos al índice
          index.addToIndex("c:\\MisDocumentos");
          // Buscando las palabras 'affect' o 'effect' en un documento con 'principal', 'principle', 'principles' o 'principalmente'
          SearchResults results = index.search("?ffect & princip?(2~4)");
          ```
      # more_feature_loop
      - title: "Combinar múltiples índices para mejorar la eficiencia de búsqueda"
        content: "GroupDocs.Search for Java API proporciona la función para fusionar múltiples índices en un índice común. Para un índice que se modifica con frecuencia, se crean varios índices delta. Sin embargo, este enfoque hace que el rendimiento de la búsqueda sea lento. GroupDocs.Search for Java supera este cuello de botella al crear un índice común mediante la fusión de varios índices delta. Este índice combinado común contiene toda la información de los índices delta combinados. Este enfoque mantiene los índices delta sin cambios mientras mejora notablemente la eficiencia de la búsqueda. Puede configurar varias funcionalidades para modificar aún más este proceso."

      # more_feature_loop
      - title: "Reconocer consultas de búsqueda de diferentes diseños de teclado"
        content: "GroupDocs.Search for Java reconoce las consultas de búsqueda que no coinciden con la distribución de su teclado. Por el momento, GroupDocs.Search para Java puede reconocer con éxito 88 idiomas y 164 distribuciones de teclado diferentes."

      # more_feature_loop
      - title: "Buscar utilizando la forma de palabra morfológica"
        content: "Usando GroupDocs.Search para Java, tiene la libertad de buscar varias formas de palabras. Puede buscar formas singulares y plurales de sustantivos específicos. O puede optar por buscar todas las formas de un verbo. También se pueden buscar raíz, tercera persona singular y pasado simple junto con varias otras formas. Para idiomas que no sean inglés, puede configurar formas de palabras personalizadas."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search ofrece API de visualización de documentos para otros entornos de desarrollo populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for .NET"
          image: "/border/groupdocs-search-net.svg"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---