---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/net/case-sensitive/ppt/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Aplicar búsqueda de texto con distinción entre mayúsculas y minúsculas a través de PPT documentos a través de .NET"
head_description: "GroupDocs.Search .NET API permite a los programadores de software aplicar la búsqueda de texto que distingue entre mayúsculas y minúsculas y encontrar la secuencia exacta de palabras en PPT documentos a través de .NET API."

############################# Header ############################
title: "¿Cómo aplicar la búsqueda que distingue entre mayúsculas y minúsculas a través de PPT documentos dentro de las aplicaciones .NET?"
description: "GroupDocs.Search .NET API permite a los desarrolladores de software aplicar búsquedas de texto con distinción entre mayúsculas y minúsculas a través de varios tipos de documentos como PDF, HTML, DOCX, PPTX, XLSX y más dentro de las aplicaciones .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Qué es la búsqueda sensible a mayúsculas y minúsculas y cómo lograrla a través de .NET?"
    content: |
      Existen numerosas técnicas de búsqueda útiles que pueden ayudar a los usuarios a buscar en varios tipos de documentos una combinación particular de palabras u otros datos. La búsqueda sensible a mayúsculas y minúsculas es una técnica muy útil que permite a los usuarios buscar documentos y páginas web, ya sea que las letras mayúsculas y minúsculas se traten como diferentes o iguales. Por ejemplo, "Computadora", "computadora" y "COMPUTADORA" se tratarán como palabras diferentes porque la letra "C" está en mayúsculas en la primera instancia, en minúsculas en la segunda y todas en mayúsculas en la tercera. GroupDocs.Search for .NET es una conveniente API de búsqueda de documentos de alto rendimiento que permite al creador de software crear aplicaciones y herramientas de software para realizar búsquedas de texto e indexación de documentos con facilidad. La API brinda compatibilidad con algunos de los formatos de archivo más utilizados, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, presentaciones de PowerPoint, MSG de Outlook, PST y muchos más. Otra característica útil es que puede identificar consultas de búsqueda escritas en un idioma que no coincide con la distribución de su teclado.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Realice una búsqueda con distinción entre mayúsculas y minúsculas en PPT Documentos a través de .NET"
      content_left: |
       GroupDocs.Search .NET API permite a los programadores de software agregar funciones de búsqueda que distinguen entre mayúsculas y minúsculas dentro de su propia aplicación C# .NET. El siguiente ejemplo de código .NET ilustra cómo lograr una búsqueda que distingue entre mayúsculas y minúsculas con una consulta en forma de texto en archivos PPT con solo un par de líneas de código.

      title_right: "Aplicar búsqueda con distinción entre mayúsculas y minúsculas en PPT Documentos"
      content_right: |
         * Identifique la ruta a la carpeta de índice, así como a la carpeta de documentos.
         * Genere un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Indexación de documentos de la carpeta especificada llamando a la instancia de la clase [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
         * Inicializa una nueva instancia de la clase [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
         * Habilitar la búsqueda sensible a mayúsculas llamando al método [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
         * Definir cadena de búsqueda y comenzar a buscar
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: "Realizar búsquedas con distinción entre mayúsculas y minúsculas en forma de objeto a través de .NET"
      content_left: |
        GroupDocs.Search .NET brinda a los desarrolladores de software el poder de descubrir palabras teniendo en cuenta las letras mayúsculas y minúsculas dentro de la aplicación .NET. El siguiente ejemplo de código .NET ilustra cómo aplicar una búsqueda que distingue entre mayúsculas y minúsculas con una consulta en forma de objeto en documentos PPT.

      title_right: "Haga una búsqueda que distinga entre mayúsculas y minúsculas en PPT Documentos"
      content_right: |
        * Identifique la ruta a la carpeta de índice, así como a la carpeta de documentos.
        * Genere un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexación de documentos de la carpeta especificada llamando a la instancia de la clase [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
        * Inicializa una nueva instancia de la clase [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
        * Habilitar la búsqueda sensible a mayúsculas llamando al método [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
        * Crear consulta de búsqueda en forma de objeto llamando al método [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
        * Comience a buscar y muestre los resultados de búsqueda
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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