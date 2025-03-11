
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: pt
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Pesquisar em documentos PPTX usando .NET"
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
    title: "Como buscar em dados PPTX"
    content: |
      [GroupDocs.Search](/search/net/) possibilita buscas eficientes de texto em documentos PPTX, tornando-o ideal para aplicações .NET.
      
      1. Configure uma pasta para armazenar o índice de busca.
      2. Selecione a pasta que contém seus arquivos.
      3. Configure as opções de busca para processar apenas documentos PPTX.
      4. Execute a busca e recupere os resultados.
   
    code:
      platform: "net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
            SearchDocumentFilter.CreateFileExtension(".pptx");

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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pptx"
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
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Encontre dados em seus documentos empresariais"
    exclude: "PPTX"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo, permitindo o processamento e a busca eficiente em documentos de escritório populares."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---