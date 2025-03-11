
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: pt
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Busca Sensível a Maiúsculas em TXT Usando .NET"
head_description: "A API GroupDocs.Search for .NET permite que desenvolvedores C# realizem buscas sensíveis a maiúsculas em vários documentos."

############################# Header ############################
title: "Busca Sensível a Maiúsculas" 
description: "GroupDocs.Search for .NET facilita a criação de consultas avançadas de buscas sensíveis a maiúsculas em suas aplicações .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar Grátis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) é uma biblioteca robusta para busca e indexação de texto em documentos. Suporta mais de 70 formatos de arquivo, incluindo PDF, Word, PowerPoint, Excel, imagens e arquivos ZIP, garantindo o manuseio eficiente de grandes volumes de dados.

############################# Steps ############################
steps:
    enable: true
    title: "Como Realizar Busca Sensível a Maiúsculas em Documentos TXT"
    content: |
      [GroupDocs.Search](/search/net/) simplifica a busca sensível a maiúsculas em documentos TXT. Utilize-o para refinar resultados em aplicações .NET.
      
      1. Defina a pasta para armazenar o índice de busca.
      2. Escolha a pasta que contém os arquivos TXT.
      3. Execute a busca e recupere os resultados.
      4. Processar os resultados.
   
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
        // Defina o caminho para a pasta do índice
        Index index = new Index("c:/MyIndex");

        // Especifique a pasta que contém os documentos a serem pesquisados
        index.Add("c:/MyDocuments");

        // Ative a busca sensível a maiúsculas nas opções
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Execute a busca
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Recursos Avançados para Busca e Indexação de Documentos"
  description: "A biblioteca GroupDocs.Search for .NET simplifica a busca de texto e a indexação em mais de 70 formatos de arquivo. Localize e gerencie informações com ferramentas de busca poderosas."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca Avançada de Texto"
      content: "Pesquise texto em vários formatos de arquivo, incluindo PDFs, documentos do Word, planilhas e apresentações. Utilize opções como correspondências exatas, busca difusa e curingas para resultados precisos."

    # feature loop
    - title: "Indexar Grandes Conjuntos de Dados"
      content: "Crie e mantenha índices para buscas mais rápidas. A indexação organizada simplifica a busca em extensas coleções de documentos."

    # feature loop
    - title: "Suporte a Múltiplos Idiomas"
      content: "Pesquise em documentos em mais de 80 idiomas, com suporte a diferentes layouts de teclado e formas de palavras para resultados mais precisos."

    # feature loop
    - title: "Opções de Busca Personalizáveis"
      content: "Personalize as configurações de busca com sensibilidade a maiúsculas, filtros de intervalo de datas e a capacidade de excluir palavras ou dados específicos durante a indexação."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando Consultas de Busca Sensíveis a Maiúsculas"
      content: |
        Este exemplo demonstra como usar consultas sensíveis a maiúsculas para buscar documentos TXT.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Defina a pasta para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Especifique o caminho para os documentos a serem pesquisados
          index.Add("c:/MyDocuments");

          // Crie uma consulta de busca
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Ative as opções de busca sensível a maiúsculas
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Pesquise por texto nos documentos
          SearchResult result = index.Search(wordQuery, options);
          
          // Processar os resultados da busca
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
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
    title: "Descubra Recursos Principais"
    exclude: "case-sensitive"
    description: "Explore funcionalidades de busca avançadas e eficientes."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar Formatos de Documentos Populares"
    exclude: "TXT"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo. Personalize regras de busca e utilize indexação para economizar tempo e esforço."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---