---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: C# .NET Búsqueda de texto & Indexación API para Word Excel PDF Email HTML"
head_description: "API de búsqueda de texto C# .NET para indexar y recuperar datos de manera inteligente de archivos PDF, Office de Microsoft Word, Excel, presentaciones, OneNote, correo electrónico, ZIP, EPUB y archivos web."

############################# Header ############################
title: ".NET API para buscar e indexar documentos"
description: "API para indexar datos y realizar búsquedas de texto en todos los formatos de documentos populares utilizando aplicaciones .NET."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "/border/groupdocs-search-net.svg"
        product: "GroupDocs.Search"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Search for .NET es una API de búsqueda de documentos y texto para aplicaciones empresariales desarrollada en C#, ASP.NET y otras tecnologías .NET. Esta API de .NET admite funciones de búsqueda básicas y avanzadas, por ejemplo, creación y combinación de múltiples índices, búsqueda a través de índices usando Sencillo, Boolean, Fuzzy, Expresión regular (regex) y otros tipos de consulta para obtener los datos requeridos, desde archivos, documentos y correos electrónicos, a través de la búsqueda inteligente. Si desea crear una aplicación de búsqueda rápida, confiable, inteligente y rica en funciones para sus usuarios finales, compatible con todos los formatos de archivo populares, GroupDocs.Search for .NET es todo lo que necesita..
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Search para .NET:
      
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
          GroupDocs.Search para .NET es compatible con los siguientes [formatos de archivo de documento] (https://docs.groupdocs.com/search/net/supported-document-formats/):

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
          GroupDocs.Search for .NET es compatible con los siguientes sistemas operativos, marcos y administrador de paquetes:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * .NET Framework 2.0 o superior
                * Mono Framework 1.2 o superior
                * .NET estándar 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Gerente de empaquetación"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entornos de desarrollo"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Características ############################
features:
    enable: true
    title: "GroupDocs.Search for .NET Características"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Cree un índice en la memoria o en el disco y realice una indexación y fusión de subprocesos múltiples"

      # feature loop
      - icon: "fas fa-eye"
        content: "Impedir la indexación de archivos ya indexados o con una cadena específica en su nombre"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Ver el porcentaje de progreso de la creación y actualización del índice y obtener un informe de búsqueda"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Indexación más rápida al excluir palabras específicas y notificación de estado de índice para archivos procesados ​​recientemente"

      # feature loop
      - icon: "fas fa-code"
        content: "Indexe archivos ZIP dentro de archivos ZIP y obtenga una lista de archivos indexados contenidos en un archivo"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Use Lista o Importar para Reemplazar Caracteres durante la Indexación y Exportarlos a un Archivo"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Indexación y búsqueda de archivos protegidos por contraseña e indexación compacta para ahorrar espacio en disco"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Extraiga texto del índice o del archivo fuente y guarde automáticamente la codificación del archivo de texto en el índice"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Agregue Campos Adicionales Arbitrarios a cada Documento durante la Indexación"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Configurar el filtrado de documentos en los resultados de búsqueda"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Manejar los errores de tipeo a través de Búsqueda borrosa, establecer el nivel de similitud en Búsqueda borrosa y mostrar solo los mejores resultados"

      # feature loop
      - icon: "fas fa-columns"
        content: "Indexar documentos de flujos y estructuras de datos"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Buscar frases completas con palabras vacías y combinar búsqueda facetada con búsqueda booleana"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Búsqueda basada en términos homofónicos, sinónimos, rango de fechas, comodines y mayúsculas y minúsculas"

      # feature loop
      - icon: "fas fa-print"
        content: "Indexe y busque correos electrónicos desde Outlook y navegue usando Aspose.Email API"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Admite el corrector ortográfico y los comodines en las consultas de búsqueda y omite caracteres especiales en las frases de búsqueda"

      # feature loop
      - icon: "fas fa-lock"
        content: "Limite los resultados para cada término en la consulta de búsqueda, así como para todos los resultados"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Extraiga texto HTML a un archivo y genere URL para navegar por los resultados de búsqueda con formato HTML"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Combine varias consultas en un solo árbol de objetos"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Alertar al usuario sobre configuraciones no compatibles y recarga automática de índice en caso de error de indexación"

      # feature loop
      - icon: "fas fa-heading"
        content: "Habilite el número exacto de ocurrencias para cada palabra encontrada para ofrecer sugerencias de palabras alternativas en caso de errores ortográficos"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Agregar atributos de texto a documentos indexados sin volver a indexar"

      # feature loop
      - icon: "fas fa-cube"
        content: "Realizar Operaciones de Indexación y Búsqueda Basadas en Caracteres"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Índice de metadatos de formatos de documentos no textuales"

    more_feature:
      # more_feature_loop
      - title: "Indexación & Search"
        content: |
          GroupDocs.Search for .NET API utiliza con frecuencia el índice para realizar la búsqueda. Los índices se utilizan para recopilar, analizar o almacenar datos para una búsqueda rápida y precisa.

          * **Crear índice**: Cree una carpeta de índice y agregue/indexe documentos a esa carpeta.
          * **Cargar índice**: Cargue un índice existente.
          * **Agregar documentos al índice**: Agregue documentos al índice existente, de forma asíncrona.
          * **Índice de actualización**: Actualice el índice existente, cada vez que se modifique, agregue o elimine un documento. Esto mantiene los resultados de búsqueda actualizados.

          ```cs
          Index  index = new Index(@"c:\MyIndex");
          index.AddToIndex(@"c:\MyDocuments");
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      # more_feature_loop
      - title: "Combinar múltiples índices para mejorar la eficiencia de búsqueda"
        content: "GroupDocs.Search for .NET puede fusionar varios índices en un solo índice. Si un índice se actualiza con frecuencia, tiene varios índices delta, pero este enfoque reduce el rendimiento de la búsqueda. GroupDocs.Search for .NET API fusiona todos los índices delta en un índice consolidado. El índice combinado primario contendrá toda la información de los índices delta combinados; sin embargo, los índices delta permanecerán sin cambios. Este enfoque utilizado por nuestra API mejora considerablemente la eficiencia de búsqueda. La función de combinación de índices proporciona numerosas funcionalidades para modificar y modificar aún más este proceso."

      # more_feature_loop
      - title: "Almacenar texto en índice para generar marcado HTML"
        content: "GroupDocs.Search for .NET puede almacenar en caché el texto de los documentos indexados en un índice. Este texto almacenado en caché se usa para generar rápidamente marcado HTML resaltando los resultados de búsqueda. Este enfoque es mucho más rápido que extraer texto directamente de los archivos. La recuperación de texto de la memoria caché estará disponible incluso si los archivos de origen ya no están disponibles. El texto en caché se puede almacenar aplicando varios niveles de compresión para ocupar menos espacio en disco y un tiempo de indexación más rápido."

      # more_feature_loop
      - title: "Obtener documentos relacionados por Fuzzy & Regex Search"
        content: "Cuando realiza una búsqueda Fuzzy o Regex, puede obtener la lista de documentos que coinciden exactamente con la entrada proporcionada. Sin embargo, también obtendrá una lista de documentos que contienen palabras o términos similares a su entrada. Por ejemplo, si usa GroupDocs.Search para .NET, realiza una búsqueda aproximada para la consulta \"costo\", obtendrá documentos que contienen la palabra \"costo\" y documentos que contienen palabras similares, como \"abrigo\". Los resultados dependerán del nivel de borrosidad que haya configurado con esta API."

      # more_feature_loop
      - title: "Reconocer consultas de búsqueda de diferentes diseños de teclado"
        content: "GroupDocs.Search for .Net puede reconocer consultas de búsqueda escritas en un idioma que no coincide con la distribución de su teclado. Actualmente, esta API de .NET puede reconocer con éxito 88 idiomas y 164 diseños de teclado diferentes."

      # more_feature_loop
      - title: "Buscar utilizando la forma de palabra morfológica"
        content: "GroupDocs.Search for .NET API le permite buscar varias formas de palabras. Por ejemplo, para un sustantivo puede buscar sus formas singular y plural. Para un verbo, puede buscar todas las formas de ese verbo. También puede buscar raíz, tercera persona del singular, pasado simple y varias otras formas. Para idiomas que no sean inglés, puede implementar formas de palabras personalizadas."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search ofrece API de visualización de documentos para otros entornos de desarrollo populares"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for Java"
          image: "/border/groupdocs-search-java.svg"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
