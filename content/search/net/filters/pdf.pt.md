
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: pt
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Pesquisar em documentos PDF usando .NET"
head_description: "GroupDocs.Search for .NET aprimora aplicações C# com pesquisa textual eficiente em vários formatos de documentos empresariais."

############################# Header ############################
title: "Pesquise texto em documentos empresariais" 
description: "GroupDocs.Search for .NET permite pesquisas de texto poderosas e flexíveis em seus documentos. Integre facilmente a funcionalidade de busca em aplicações .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) é uma biblioteca poderosa para busca textual eficiente e indexação de documentos. Ela suporta mais de 70 formatos de arquivo, incluindo documentos padrão da indústria como PDF, Word, Excel e PowerPoint. Melhore o desempenho de pesquisa com resultados rápidos e precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Como buscar em dados PDF"
    content: |
      [GroupDocs.Search](/search/net/) possibilita buscas eficientes de texto em documentos PDF, tornando-o ideal para aplicações .NET.
      
      1. Configure uma pasta para armazenar o índice de busca.
      2. Selecione a pasta que contém seus arquivos.
      3. Configure as opções de busca para processar apenas documentos PDF.
      4. Execute a busca e recupere os resultados.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado da busca"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Caminho para armazenar o índice de busca reutilizável
        Index index = new Index("c:/MyIndex");

        // Pasta contendo documentos
        index.Add("c:/MyDocuments");

        // Pesquisar apenas em formatos de arquivo específicos
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".pdf");

        // Recuperar resultados da busca
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Recursos avançados de busca"
  description: "GroupDocs.Search for .NET possibilita buscas sofisticadas de texto em mais de 70 formatos de arquivo. A indexação melhora a eficiência da busca e ajuda na gestão do conteúdo dos documentos."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Principais recursos do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca avançada de texto"
      content: "Extraia texto relevante de documentos empresariais populares, incluindo PDFs, arquivos Word, apresentações e planilhas. Suporta várias técnicas de busca, como busca difusa, detecção de homofones e curingas."

    # feature loop
    - title: "Indexação otimizada para buscas mais rápidas"
      content: "Crie e reutilize índices de busca para aumentar a velocidade da pesquisa. A indexação otimiza o desempenho ao pesquisar em grandes coleções de documentos."

    # feature loop
    - title: "Suporte para múltiplos idiomas"
      content: "Realize buscas em documentos escritos em mais de 80 idiomas. Detecta diferentes layouts de teclado e variações de palavras para melhorar a precisão."

    # feature loop
    - title: "Configurações de busca flexíveis"
      content: "Refine os resultados da busca com opções personalizáveis, incluindo filtros, expressões regulares e configurações de sensibilidade a maiúsculas e minúsculas."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrar documentos a serem processados"
      content: |
        Aprenda como restringir buscas de documentos usando filtros
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Configure um índice que exclua certos formatos de arquivo
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Especifique o diretório dos documentos
          index.Add("c:/MyDocuments");

          // Recupere os resultados da busca
          SearchResult result = index.Search("Lorem");
          
          // Processar e utilizar a saída da busca
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Copiar"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pdf"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente as funcionalidades do GroupDocs.Search gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Download do Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Recursos principais"
    exclude: "filters"
    description: "Realize buscas precisas e eficientes de dados."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Encontre dados em seus documentos empresariais"
    exclude: "PDF"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo, permitindo o processamento e a busca eficiente em documentos de escritório populares."
    items: 
        # format loop 1
        - name: "Filtros de busca para DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Filtros de busca para PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Filtros de busca para PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Filtros de busca para TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Filtros de busca para XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---