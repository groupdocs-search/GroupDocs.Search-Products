---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/net/filters/one/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Personalice los resultados de búsqueda configurando el filtrado de documentos en las aplicaciones .NET"
head_description: "GroupDocs.Search .NET API permite a los desarrolladores de software buscar documentos de ONE Documents y personalizar los resultados de la búsqueda mediante la aplicación de filtrado de documentos en aplicaciones .NET."

############################# Header ############################
title: "Configure el filtrado de documentos para personalizar los resultados de búsqueda dentro de las aplicaciones .NET"
description: "GroupDocs.Search .NET API ayuda a las profesiones de software a agregar capacidades de búsqueda de documentos y personalizar el resultado de la búsqueda mediante la aplicación de filtrado de documentos dentro de sus aplicaciones .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo aplicar el filtrado de documentos en los resultados de búsqueda a través de .NET?"
    content: |
       El filtrado es una técnica muy útil que permite a los usuarios inspeccionar y procesar la funcionalidad. El filtrado de documentos ofrece a los usuarios una manera fácil de navegar por sus resultados y encontrar lo que buscan. También da a los usuarios el poder de limitar su búsqueda a una determinada sección o un tipo de documento en particular. GroupDocs.Search for .NET es una API de búsqueda de documentos de alto rendimiento y rica en funciones que permite a los desarrolladores de software crear aplicaciones que pueden lograr la búsqueda e indexación de texto. Admite algunos de los formatos de documentos más populares, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint, MSG de Outlook, PST y muchos más. La API es totalmente compatible con la configuración de archivos de documentos para los resultados de búsqueda. Puede usar varios tipos de archivadores para personalizar los resultados de su búsqueda, como filtros de ruta de archivo, filtro de extensión de archivo, filtro de atributos y muchos más. También es posible combinar filtros de documentos de búsqueda utilizando el operador booleano AND, OR & NOT, etc.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Establecer filtro de documentos en la búsqueda de documentos ONE a través de .NET"
      content_left: |
       GroupDocs.Search .NET API ayuda a los desarrolladores de software a agregar capacidades de búsqueda dentro de su aplicación .NET. El siguiente ejemplo de código .NET demuestra cómo aplicar el filtro de documentos en la búsqueda de varios tipos de documentos con solo un par de líneas de código.

      title_right: "Aplicar filtro de documentos en la búsqueda de documentos ONE"
      content_right: |
       * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
       * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
       * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
       * Crear un objeto de opciones de búsqueda [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * Configure el filtro de documentos llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Comience a buscar y muestre los resultados de búsqueda
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: "Cómo combinar filtros de documentos de búsqueda a través de .NET"
      content_left: |
        GroupDocs.Search for .NET permite a los programadores de software combinar filtros de documentos de búsqueda durante la búsqueda para controlar cuál de los documentos encontrados debe devolverse como resultado de la búsqueda dentro de la aplicación C# .NET. Los siguientes ejemplos de código .NET muestran cómo combinar filtros de documentos de búsqueda mediante operadores booleanos AND, OR, NOT, etc. dentro de aplicaciones C#.

      title_right: "Combinar filtros de documentos de búsqueda en la búsqueda de archivos ONE"
      content_right: |
       * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
       * Crear un filtro compuesto AND que devuelva todos los documentos FB2 y EPUB que tengan la palabra 'Einstein' en sus rutas completas
       * Cree filter1 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Cree filter2 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Combine filtros llamando al método [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand)
       * Creación de un filtro compuesto OR que devuelve todos los DOC, DOCX, PDF y todos los documentos que tienen la palabra Einstein en sus rutas completas
       * Cree filter3 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Cree filter4 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Combine filtros llamando al método [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor)
       * Creación de un filtro que devuelve todos los documentos encontrados excepto los documentos TXT
       * Cree filter4 llamando a [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Appy Not filter llamando al método [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot)

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
    - title_left: "Requisitos del sistema"
      content_left: |
       GroupDocs.Search for .NET es compatible con todas las principales plataformas y sistemas operativos. Para obtener una guía completa de requisitos del sistema, visite [requisitos del sistema](https://docs.groupdocs.com/search/net/system-requirements/) antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema:
         * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
         * Entorno de desarrollo: Visual Studio, Xamarin, MonoDevelop, etc.
         * Marcos: .NET Framework, .NET Standard, .NET Core, Mono
         * Obtenga la última versión de GroupDocs.Search para las API de .NET de [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
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