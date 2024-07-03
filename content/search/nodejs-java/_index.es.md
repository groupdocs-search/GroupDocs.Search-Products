---
############################# Static ############################
layout: "landing"
date: 2024-07-03T19:47:25
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
head_title: "Node.js Biblioteca de indexación y búsqueda de texto para documentos, PDF, Office y Web"
head_description: "Solución avanzada de búsqueda de texto para aplicaciones Node.js para buscar, indexar y recopilar datos de documentos: PDF, Word, Excel, presentaciones, correo electrónico y formatos de archivos web."

############################# Header ############################
title: "Buscar e indexar documentos utilizando la API Node.js"
description: "Mejore las aplicaciones Node.js implementando la búsqueda de texto en todos los formatos de documentos populares."
words:
  for: "para"

actions:
  main: "Descarga gratuita de NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licencia"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "¿Listo para comenzar?"
  description: "Pruebe las funciones de GroupDocs.Search gratis o solicite una licencia"

release:
  title: "Versión {0} lanzada"
  notes: "Ver qué hay de nuevo"
  downloads: "Descargas"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Buscar en la carpeta con JavaScript"
  more: "Más ejemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // Creando índice
    var index = new Index("c:\\MyIndex");

    // Agregar documentos al índice
    index.addToIndex("c:\\MyDocuments");
    
    // Buscando varias palabras como
    // 'affect', 'effect', 'principles', 'principally'
    var results = index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search de un vistazo"
  description: "Biblioteca Node.js JavaScript para búsqueda de texto"
  features:
    # feature loop
    - title: "Node.js Operaciones de indexación y búsqueda"
      content: "La indexación en GroupDocs.Search for Node.js via Java recopila, almacena y analiza datos para operaciones de búsqueda precisas y eficientes. Estos índices se utilizan frecuentemente para realizar búsquedas."

    # feature loop
    - title: "Fusione varios índices para mejorar la eficiencia de la búsqueda"
      content: "La API GroupDocs.Search for Node.js via Java permite fusionar varios índices en uno. Las modificaciones frecuentes crean varios índices delta, lo que puede ralentizar el rendimiento de la búsqueda. Nuestra solución fusiona estos índices delta en un índice común, que contiene toda la información de los índices delta fusionados, lo que mejora significativamente la eficiencia de la búsqueda y mantiene los índices delta sin cambios. Se pueden configurar varias funcionalidades para ajustar este proceso."

    # feature loop
    - title: "Reconocer consultas de búsqueda desde diferentes diseños de teclado"
      content: "GroupDocs.Search for Node.js via Java reconoce consultas de búsqueda que no coinciden con la distribución del teclado. Actualmente, se admiten 88 idiomas y 164 diseños de teclado diferentes."

    # feature loop
    - title: "Buscar utilizando formas de palabras morfológicas"
      content: "Con GroupDocs.Search for Node.js via Java, puedes buscar varias formas de palabras, como sustantivos en singular y plural, o todas las formas de un verbo. Los idiomas inglés y no inglés se pueden personalizar para formas de palabras específicas."

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
  title: "Formatos de archivo admitidos"
  description: |
    GroupDocs.Search for Node.js via Java permite procesar una amplia gama de formatos de archivos. [Explore la lista completa](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos de oficina populares
        * **Portátil:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Texto:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formatos de medios
        * **Formatos de imagen populares:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Imágenes de varias páginas:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Video:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Otro
        * **Correo electrónico:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Otros:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Funciones de GroupDocs.Search for Node.js via Java"
  description: "Controle el contenido de los documentos comerciales utilizando nuestro motor de búsqueda avanzado, compatible con formatos de archivos populares, incluidos PDF, DOCX, XLSX, PPTX y más."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parámetros flexibles"
      content: "Utilice el rango de fechas y la distinción entre mayúsculas y minúsculas como parámetros de búsqueda"

    # feature loop
    - icon: "detect"
      title: "Búsqueda de revisión ortográfica"
      content: "Utilice frases de búsqueda con corrector ortográfico y comodines y omita caracteres especiales en consultas"

    # feature loop
    - icon: "collect"
      title: "Filtrado de resultados"
      content: "Configurar el filtrado de documentos en los resultados de búsqueda"

    # feature loop
    - icon: "get"
      title: "Importación y exportación"
      content: "Realizar importación o uso de lista para modificar caracteres durante la indexación y exportación a un archivo"

    # feature loop
    - icon: "remove"
      title: "Saltar datos innecesarios"
      content: "Omita selectivamente la indexación de archivos específicos y omita palabras específicas para indexar más rápido"

    # feature loop
    - icon: "style"
      title: "Procesamiento de URL"
      content: "Extraiga texto con formato HTML a un archivo y genere una URL para navegar por los resultados de búsqueda en HTML"

    # feature loop
    - icon: "detect"
      title: "Búsqueda rápida"
      content: "Divida la búsqueda en partes más pequeñas para buscar rápidamente en índices grandes"

    # feature loop
    - icon: "manipulate"
      title: "Procesamiento de flujo"
      content: "Indexar documentos de flujos y estructuras de datos"

    # feature loop
    - icon: "compare"
      title: "Manejar errores ortográficos"
      content: "Habilite el número exacto de apariciones de cada palabra encontrada para ofrecer sugerencias de palabras alternativas en caso de errores ortográficos"

    # feature loop
    - icon: "unreadable_characters"
      title: "Soporte de archivo"
      content: "Indexar archivos comprimidos dentro de otros archivos ZIP y recuperar la lista de archivos indexados en un archivo"

    # feature loop
    - icon: "hidden_print"
      title: "Ahorro de espacio en disco"
      content: "Ahorre espacio con indexación compacta y documentos protegidos con contraseña de índice"

    # feature loop
    - icon: "style"
      title: "Sinónimos personalizados"
      content: "Agregar sinónimos en inglés al diccionario de sinónimos predeterminado"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ejemplos de código"
  description: "Explora las funcionalidades de GroupDocs.Search for Node.js via Java con ejemplos"
  items:
    # code sample loop
    - title: "Utilice la búsqueda difusa para mejorar la productividad"
      content: |
        Disfrute de la funcionalidad flexible de GroupDocs.Search for Node.js via Java para mejorar el control del contenido de los documentos mediante sofisticados algoritmos de búsqueda. [Más información](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Cómo procesar el resultado de la búsqueda">}}
        ```javascript {style=abap}
        // Crear un índice
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");

        // Configurar opciones de búsqueda
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Busque documentos que contengan la palabra 'agua' o la frase 'Lorem ipsum'
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // Procesar resultado de búsqueda
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Las expresiones regulares están disponibles para escenarios de búsqueda avanzada."
      content: |
        GroupDocs.Search for Node.js via Java nos permite utilizar expresiones regulares para limitar el resultado de la búsqueda. [Sumérgete en técnicas de búsqueda avanzada](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Cómo buscar usando expresiones regulares">}}
        ```javascript {style=abap}   
        // Crear un índice
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");
 
        // Busque la frase en forma de texto.

        // El primer carácter de intercalación al principio indica que se trata de una consulta de búsqueda de expresión regular.
        var query = "^^(.)\\1{1,}";
        // Buscar dos o más caracteres idénticos al principio de una palabra
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
