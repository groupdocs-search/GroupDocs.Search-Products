---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/java/filters/pdf/"
otherformats: DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2  

############################# Head ############################
head_title: "¿Integrar el filtrado de documentos PDF en los resultados de búsqueda a través de la API de Java?"
head_description: "GroupDocs.Search Java API ayuda a los desarrolladores de software a agregar PDF capacidades de búsqueda de documentos y aplicar filtrado de documentos para personalizar los resultados de búsqueda a través de Java API."

############################# Header ############################
title: "Cómo integrar el filtrado de documentos para personalizar los resultados de búsqueda dentro de las aplicaciones Java"
description: "GroupDocs.Search Java API permite a los programadores integrar funciones avanzadas de búsqueda de documentos PDF, así como personalizar los resultados de la búsqueda configurando el filtrado de documentos en sus aplicaciones Java."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Cómo integrar el filtrado de documentos para personalizar los resultados de búsqueda dentro de las aplicaciones Java"
    content: |
       El filtrado de documentos es una actividad muy útil que permite que las aplicaciones de software busquen y recuperen documentos según la secuencia de palabras relevante ingresada por un usuario en el texto de los documentos indexados. Un filtro contiene un conjunto de reglas que definen el criterio utilizado para seleccionar registros. El filtrado de documentos permite a los usuarios limitar su búsqueda a una determinada sección o un tipo de documento en particular, así como navegar a través de los resultados y encontrar lo que están buscando. GroupDocs.Search para Java es una API de búsqueda e indexación de documentos de alto rendimiento rica en características que permite a los desarrolladores de software crear aplicaciones que pueden lograr la indexación de texto y la búsqueda de algunos de los formatos de archivo de documentos más populares. Es totalmente compatible con varios tipos de documentos, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint, MSG de Outlook, PST, etc. Hay varios tipos de archivadores disponibles para que el usuario personalice los resultados de búsqueda, como filtros de ruta de archivo, filtro de extensión de archivo, filtro de atributo y muchos más.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Aplicar filtro de documentos en la búsqueda de documentos PDF a través de Java"
      content_left: |
       GroupDocs.Search Java API ayuda a los desarrolladores de software a crear aplicaciones poderosas con capacidades de búsqueda utilizando la API de Java. El siguiente ejemplo de código Java muestra cómo aplicar el filtro de documentos para buscar varios tipos de documentos con solo un par de líneas de código.

      title_right: "Configuración del filtro de documentos en la búsqueda de documentos PDF"
      content_right: |
       * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
       * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
       * Indexación de documentos de la carpeta especificada llamando al método [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
       * Crear un objeto de opciones de búsqueda llamando a la clase [earchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions)
       * Configure el filtro de documentos llamando al método [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Comience a buscar y muestre documentos de texto si encuentra alguno
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "Combine Search Document Filters to Create Composite Filter via Java"
      content_left: |
        GroupDocs.Search for Java allows software programmers to add advanced searching capability and apply custom filters for document searching inside their Java application. Users can create composite filter by combining various types of search filters. The following Java code demonstrates how to combine search document filters to create composite filter using Boolean operators AND, OR, NOT etc. with just a couple of lines of code.

      title_right: "Crear filtro compuesto para buscar archivos PDF"
      content_right: |
       * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
       * Crear un filtro compuesto AND que devuelva todos los documentos FB2 y EPUB que tengan la palabra 'Einstein' en sus rutas completas
       * Cree filter1 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Cree filter2 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Combine filtros llamando al método [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...))
       * Cree un filtro compuesto OR que devuelva todos los DOC, DOCX, PDF y todos los documentos que tengan la palabra Einstein en sus rutas completas
       * Cree filter3 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Cree filter4 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Combine filtros llamando al método [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...))
       * Creación de un filtro que devuelve todos los documentos encontrados excepto los documentos TXT
       * Cree filter4 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Appy Not filter llamando al método [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter))

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
    - title_left: "Requisitos del sistema"
      content_left: |
        GroupDocs.Search for Java es compatible con todas las principales plataformas y sistemas operativos. Para obtener una guía completa de requisitos del sistema, visite [requisitos del sistema](https://docs.groupdocs.com/search/java/system-requirements/) antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema:
          * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
          * Compatibilidad con versiones de Java: J2SE 7.0 (1.7), J2SE 8.0 (1.8) o superior
          * Obtenga la última versión de GroupDocs.Search para las API de Java de GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "Por qué usar GroupDocs.Search"
      content_right: |
        * Creación de índices de búsqueda tanto en memoria como en disco.
        * Capacidad de indexación de un archivo, secuencia o estructura.
        * Soporte de indexación de documentos protegidos por contraseña.
        * Soporte para la fusión de varios índices.
        * Documento de filtro durante la indexación de búsqueda.
        * Compatibilidad con el corrector ortográfico durante la búsqueda.
        * Los caracteres combinados son totalmente compatibles
        * La combinación de diferentes tipos de búsqueda en una consulta de búsqueda.
        * Compatibilidad con búsquedas de palabras simples y expresiones regulares
        * Totalmente compatible con el reemplazo de alias en las consultas de búsqueda.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---