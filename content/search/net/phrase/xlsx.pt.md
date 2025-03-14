
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: pt
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Pesquisar frases em XLSX usando .NET"
head_description: "GroupDocs.Search for .NET aprimora aplicações C# com poderosas capacidades de busca de frases no conteúdo dos documentos."

############################# Header ############################
title: "Pesquise por frases em documentos" 
description: "Encontre frases específicas rapidamente com GroupDocs.Search for .NET. Integre funcionalidades de busca eficientes em suas aplicações .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Características do GroupDocs.Search"
    link: "/search/net/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) é uma biblioteca robusta para indexação e pesquisa de texto em documentos. Suporta mais de 70 formatos de arquivo, incluindo PDFs, documentos Word, planilhas Excel, imagens e arquivos ZIP, permitindo resultados de busca rápidos e precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Como buscar frases em documentos XLSX"
    content: |
      [GroupDocs.Search](/search/net/) simplifica a busca em documentos XLSX. Utilize várias opções para refinar os resultados da busca em aplicações .NET.
      
      1. Configurar a pasta do índice de busca.
      2. Especificar a pasta que contém arquivos XLSX.
      3. Configurar as configurações de busca.
      4. Recuperar e processar os resultados da busca.
   
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
        // Caminho para armazenar o índice de busca
        Index index = new Index("c:/MyIndex");

        // Pasta que contém documentos
        index.Add("c:/MyDocuments");

        // Configurar opções de busca
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Executar a busca
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Descubra o motor de busca de documentos .NET"
  description: "GroupDocs.Search for .NET possibilita buscas por frases em mais de 70 formatos de arquivo. Localize e gerencie dados com capacidades avançadas de busca."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Recursos principais do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca por frases"
      content: "Pesquise por frases exatas em documentos empresariais, incluindo PDFs, arquivos Word, apresentações e planilhas. Utilize curingas e outras opções caso a frase exata seja desconhecida."

    # feature loop
    - title: "Indexação eficiente de dados"
      content: "Crie e reutilize índices de busca para acelerar as buscas em documentos. A indexação estrutura os dados de maneira eficiente, tornando as buscas por frases mais rápidas."

    # feature loop
    - title: "Suporte a múltiplas línguas"
      content: "Pesquise documentos em mais de 80 idiomas. Suporta diferentes layouts de teclado e formas morfológicas de palavras para uma melhor precisão nas buscas."

    # feature loop
    - title: "Opções de busca flexíveis"
      content: "Personalize as buscas com recursos como sensibilidade a maiúsculas, busca difusa e de homófonos, filtragem de documentos e mais."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando técnicas avançadas de busca"
      content: |
        Aprenda como criar consultas para busca em XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Especificar a pasta para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Definir o caminho para documentos a serem buscados
          index.Add("c:/MyDocuments");

          // Criar uma consulta para uma frase específica
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Recuperar os resultados da busca
          SearchResult result = index.Search(query);
          
          // Processar e utilizar os resultados
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Recursos avançados"
    exclude: "phrase"
    description: "Utilize funcionalidades de busca poderosas e eficientes."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Busca por frases em documentos empresariais"
    exclude: "XLSX"
    description: "GroupDocs.Search suporta buscas em mais de 70 formatos de documento. Utilize opções avançadas e indexação para otimizar seu processo de busca."
    items: 
        # format loop 1
        - name: "Busca de frases em DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Busca de frases em PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Busca de frases em PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Busca de frases em TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Busca de frases em XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---