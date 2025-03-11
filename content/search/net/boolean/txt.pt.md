
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: pt
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Pesquise TXT no .NET usando operadores booleanos"
head_description: "A API GroupDocs.Search for .NET permite que desenvolvedores C# busquem o conteúdo de documentos usando operadores booleanos como AND, OR e NOT."

############################# Header ############################
title: "Busca de texto com lógica booleana" 
description: "GroupDocs.Search for .NET facilita a criação de consultas de busca avançadas usando operadores booleanos (AND, OR, NOT) em suas aplicações .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar Gratuitamente"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) é uma biblioteca completa para buscar e indexar texto em documentos. Suporta mais de 70 formatos de arquivo, como PDF, Word, PowerPoint, Excel, imagens e arquivos ZIP, permitindo o processamento eficiente de grandes volumes de informação.

############################# Steps ############################
steps:
    enable: true
    title: "Como buscar o conteúdo de documentos TXT usando lógica booleana"
    content: |
      [GroupDocs.Search](/search/net/) torna a busca pelo conteúdo de documentos TXT direta. Ele fornece condições de busca de lógica booleana para refinar os resultados nas aplicações .NET.
      
      1. Especifique a pasta para armazenar o índice de busca.
      2. Escolha a pasta contendo os arquivos TXT.
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

        // Especifique a pasta contendo os documentos a serem pesquisados
        index.Add("c:/MyDocuments");

        // Execute uma busca usando uma consulta complexa
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explore recursos avançados para busca e indexação de documentos"
  description: "A biblioteca GroupDocs.Search for .NET simplifica a busca e indexação de texto em mais de 70 formatos de arquivo. Localize e gerencie informações com ferramentas de busca avançadas."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Principais recursos do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de texto poderosa"
      content: "Pesquise texto em diversos tipos de arquivos, incluindo PDFs, documentos Word, apresentações PowerPoint e planilhas. Utilize recursos como correspondências exatas, buscas difusas e caracteres curinga para refinar os resultados."

    # feature loop
    - title: "Indexação de grandes conjuntos de dados"
      content: "Crie e mantenha índices para pesquisas mais rápidas. A indexação estrutura e organiza os dados, facilitando a busca em grandes coleções de documentos."

    # feature loop
    - title: "Suporte a múltiplas línguas"
      content: "Pesquise documentos em mais de 80 idiomas, com suporte a diferentes layouts de teclado e formas morfológicas de palavras para aumentar a precisão da busca."

    # feature loop
    - title: "Opções de busca personalizáveis"
      content: "Ajuste as configurações de busca com recursos como sensibilidade a maiúsculas, filtros de intervalo de datas e a capacidade de excluir palavras ou dados específicos durante a indexação."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando consultas de busca booleanas avançadas"
      content: |
        Este exemplo demonstra como aplicar consultas booleanas para pesquisar documentos TXT.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Defina a pasta para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Especifique o caminho para os documentos a serem pesquisados
          index.Add("c:/MyDocuments");

          // Crie uma consulta de busca usando lógica booleana
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Recupere os resultados da busca
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "Descubra recursos principais"
    exclude: "boolean"
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
    title: "Pesquise em formatos de documentos populares"
    exclude: "TXT"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo. Personalize as regras de pesquisa e utilize a indexação para economizar tempo e esforço."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---