---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: es
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Biblioteca de Búsqueda de Texto Node.js e Indexación para Documentos, PDF, Office y Web"
head_description: "Solución avanzada de búsqueda de texto para aplicaciones Node.js para buscar, indexar y recopilar datos de documentos: PDF, Word, Excel, presentaciones, correos electrónicos y formatos web."

############################# Header ############################
title: "Buscar e Indexar Documentos usando Node.js API"
description: "Mejora Aplicaciones Node.js implementando Búsqueda de Texto en Todos los Formatos de Documentos Populares."
words:
  for: "para"

actions:
  main: "Descarga Gratuita de NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licenciamiento"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "¡Comienza Tu Aventura Hoy!"
  description: "Explora las capacidades de GroupDocs.Search de forma gratuita o asegura una licencia para desbloquear todo su potencial."

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Realiza Búsqueda de Texto en una Carpeta con JavaScript"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Crea un índice para tus documentos
    const index = new searchLib.Index('c:/MyIndex');

    // Agrega documentos al índice para búsquedas eficientes
    index.add('c:/MyDocuments');
    
    // Busca palabras o frases específicas, como
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Descripción General"
  description: "Biblioteca JavaScript de Node.js para búsqueda de texto"
  features:
    # feature loop
    - title: "Operaciones de Indexación y Búsqueda Node.js"
      content: "La indexación en GroupDocs.Search for Node.js via Java recopila, almacena y analiza datos para operaciones de búsqueda precisas y eficientes. Estos índices se utilizan frecuentemente para realizar búsquedas."

    # feature loop
    - title: "Combina Múltiples Índices para Mejorar la Eficiencia de Búsqueda"
      content: "La API GroupDocs.Search for Node.js via Java permite fusionar múltiples índices en uno. Las modificaciones frecuentes crean varios índices delta, lo que puede ralentizar el rendimiento de búsqueda. Nuestra solución fusiona estos índices delta en un índice común, que contiene toda la información de los índices delta fusionados, mejorando significativamente la eficiencia de búsqueda mientras mantiene los índices delta sin cambios. Se pueden configurar diversas funcionalidades para afinar este proceso."

    # feature loop
    - title: "Reconocer Consultas de Búsqueda de Diferentes Disposiciones de Teclado"
      content: "GroupDocs.Search for Node.js via Java reconoce consultas de búsqueda que no coinciden con la disposición del teclado. Actualmente, se soportan 88 idiomas y 164 disposiciones de teclado diferentes."

    # feature loop
    - title: "Buscar Usando Formas de Palabras Morfológicas"
      content: "Con GroupDocs.Search for Node.js via Java, puedes buscar diversas formas de palabras, como sustantivos en singular y plural, o todas las formas de un verbo. Inglés y otros idiomas pueden personalizarse para formas de palabras específicas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independencia de plataforma"
  description: "GroupDocs.Search for Node.js via Java es compatible con todos los sistemas operativos y administradores de paquetes populares."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de archivo soportados"
  description: |
    GroupDocs.Search for Node.js via Java permite procesar una amplia gama de formatos de archivo. [Explora la lista completa](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
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
  title: "Características de GroupDocs.Search for Node.js via Java"
  description: "Controla el contenido de documentos empresariales usando nuestro motor de búsqueda avanzado, compatible con formatos populares que incluyen PDF, DOCX, XLSX, PPTX y más."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parámetros Flexibles"
      content: "Usa Rango de Fechas y Sensibilidad de Mayúsculas como Parámetros de Búsqueda"

    # feature loop
    - icon: "detect"
      title: "Búsqueda con Corrección Ortográfica"
      content: "Usa Frases de Búsqueda con Corrección Ortográfica y comodines y omite caracteres especiales en las consultas"

    # feature loop
    - icon: "collect"
      title: "Filtrado de Resultados"
      content: "Establece Filtrado de Documentos en los Resultados de Búsqueda"

    # feature loop
    - icon: "get"
      title: "Importar y Exportar"
      content: "Realiza Importaciones o Usa Listas para Modificar Caracteres durante la Indexación y Exportar a un Archivo"

    # feature loop
    - icon: "remove"
      title: "Omitir Datos Innecesarios"
      content: "Omitir Selectivamente la Indexación de Archivos Específicos & Omitir Palabras Específicas para Indexar Más Rápido"

    # feature loop
    - icon: "style"
      title: "Procesamiento de URL"
      content: "Extraer Texto en Formato HTML a un Archivo y Generar una URL para Navegar Resultados de Búsqueda en HTML"

    # feature loop
    - icon: "detect"
      title: "Búsqueda Rápida"
      content: "Dividir la Búsqueda en Fragmentos Más Pequeños para Buscar Rápidamente en Índices Grandes"

    # feature loop
    - icon: "manipulate"
      title: "Procesamiento por Flujos"
      content: "Indexar Documentos desde Flujos y Estructuras de Datos"

    # feature loop
    - icon: "compare"
      title: "Manejo de Errores Tipográficos"
      content: "Habilita el Número Exacto de Ocurrencias para cada Palabra Encontrada para Ofrecer Sugerencias de Palabras Alternativas en caso de Errores Tipográficos"

    # feature loop
    - icon: "unreadable_characters"
      title: "Soporte para Archivos Comprimidos"
      content: "Indexar Archivos ZIP dentro de otros Archivos ZIP y Recuperar Lista de Archivos Indexados en un Archivo"

    # feature loop
    - icon: "hidden_print"
      title: "Ahorro de Espacio en Disco"
      content: "Ahorrar Espacio con Indexación Compacta & Indexar Documentos Protegidos por Contraseña"

    # feature loop
    - icon: "style"
      title: "Sinónimos Personalizados"
      content: "Agregar Sinónimos en Inglés al Diccionario de Sinónimos Predeterminado"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Explora las funcionalidades de GroupDocs.Search for Node.js via Java con ejemplos"
  items:
    # code sample loop
    - title: "Usa la búsqueda 'difusa' para aumentar la productividad"
      content: |
        Disfruta de la funcionalidad flexible de GroupDocs.Search for Node.js via Java para mejorar el control del contenido de documentos mediante algoritmos de búsqueda sofisticados. [Aprende más](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Cómo procesar el resultado de búsqueda">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Crea un índice
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Configura las opciones de búsqueda
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Busca documentos que contengan la palabra 'agua' o la frase 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Procesa el resultado de la búsqueda
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Las expresiones regulares están disponibles para escenarios de búsqueda avanzados"
      content: |
        GroupDocs.Search for Node.js via Java nos permite usar expresiones regulares para acotar resultados de búsqueda. [Profundiza en técnicas de búsqueda avanzadas](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Cómo buscar utilizando expresiones regulares">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Crea un índice
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Busca la frase en forma de texto

        // El primer carácter de caret al principio indica que esta es una consulta de búsqueda de expresión regular
        const query = '^^(.)\\1{1,}';
        // Busca dos o más caracteres idénticos al principio de una palabra
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
