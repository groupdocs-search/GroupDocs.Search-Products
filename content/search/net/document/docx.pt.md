
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: pt
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Pesquisar documentos DOCX em .NET com GroupDocs.Search"
head_description: "Use GroupDocs.Search for .NET para realizar buscas textuais eficientes em vários formatos de documentos com C#."

############################# Header ############################
title: "Busca avançada de texto em documentos" 
description: "GroupDocs.Search for .NET simplifica a busca textual em formatos de documentos populares, permitindo que você crie consultas de pesquisa poderosas em suas aplicações .NET."
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
       [GroupDocs.Search for .NET](/search/net/) é uma biblioteca poderosa projetada para pesquisa e indexação de texto completo em documentos. Ela suporta mais de 70 formatos de arquivo, incluindo PDF, Word, PowerPoint, Excel, imagens e arquivos ZIP, garantindo resultados de busca rápidos e precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Como realizar busca textual em documentos DOCX"
    content: |
      [GroupDocs.Search](/search/net/) permite operações avançadas de busca de conteúdo em documentos DOCX, possibilitando resultados de busca refinados em aplicações .NET.
      
      1. Configure a pasta para armazenar o índice de busca.
      2. Escolha a pasta que contém arquivos DOCX.
      3. Configure opções adicionais de busca.
      4. Execute a busca e revise os resultados.
   
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
        // Defina o caminho para o índice de busca
        Index index = new Index("c:/MyIndex");

        // Selecione a pasta contendo os documentos a serem pesquisados
        index.Add("c:/MyDocuments");

        // Ative a busca homófona para encontrar palavras que soam semelhantes
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Execute uma consulta de busca complexa
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Recursos avançados de busca e indexação"
  description: "GroupDocs.Search for .NET aprimora a pesquisa de texto e a indexação em mais de 70 formatos de arquivo, fornecendo ferramentas eficientes para localizar e gerenciar informações."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Principais Recursos do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca textual poderosa"
      content: "Pesquise texto em múltiplos tipos de documentos, incluindo PDFs, documentos Word, apresentações PowerPoint e planilhas. Utilize recursos como correspondências exatas, busca difusa e curingas para refinar seus resultados."

    # feature loop
    - title: "Indexação rápida para grandes conjuntos de dados"
      content: "Crie e gerencie índices de busca para recuperação rápida de informações. A indexação otimiza as buscas em coleções extensas de documentos."

    # feature loop
    - title: "Suporte a múltiplas idiomas"
      content: "Realize buscas em mais de 80 idiomas, com suporte a diferentes layouts de teclado e variações de palavras para melhorar a precisão."

    # feature loop
    - title: "Configurações de busca personalizáveis"
      content: "Ajuste os parâmetros de busca com opções como sensibilidade a maiúsculas, filtros de intervalo de datas e exclusões de palavras para obter melhores resultados."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Executando consultas de busca avançadas"
      content: |
        Este exemplo demonstra como aplicar consultas de busca para documentos DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Defina a pasta para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Especifique o caminho para os arquivos de documento
          index.Add("c:/MyDocuments");

          // Forneça uma senha para documentos protegidos
          index.Dictionaries.DocumentPasswords.Add("protected.docx", "123456");

          // Ative a busca difusa para encontrar palavras semelhantes
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Recupere os resultados da busca
          SearchResult result = index.Search("Loarem", options);
          
          // Processar a saída da busca
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
            link: "/examples/search/formats/searchdocument.docx"
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
    title: "Explore recursos principais"
    exclude: "document"
    description: "Aproveite funcionalidades de busca avançadas e de alto desempenho."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Pesquise em seus documentos empresariais"
    exclude: "DOCX"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo, incluindo documentos de escritório, permitindo buscas rápidas e eficientes com capacidades de indexação."
    items: 
        # format loop 1
        - name: "Buscar no documento DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Buscar no documento PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Buscar no documento PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Buscar no documento TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Buscar no documento XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---