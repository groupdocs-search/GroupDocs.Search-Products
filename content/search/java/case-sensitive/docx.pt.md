
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:31
draft: false
lang: pt
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Realize Pesquisas Sensíveis a Maiúsculas em DOCX com Java"
head_description: "A API GroupDocs.Search for Java ajuda desenvolvedores Java a realizar pesquisas sensíveis a maiúsculas em vários tipos de documentos."

############################# Header ############################
title: "Pesquisa de Documentos Sensível a Maiúsculas" 
description: "GroupDocs.Search for Java permite implementar funcionalidades de pesquisa precisas e sensíveis a maiúsculas em seus projetos Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenha Gratuitamente"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Saiba Mais Sobre GroupDocs.Search"
    link: "/search/java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) é uma ferramenta versátil para busca de texto e indexação em vários documentos. Suporta mais de 70 formatos como PDFs, arquivos do Word, apresentações do PowerPoint, planilhas do Excel, imagens e arquivos ZIP, permitindo que você gerencie de forma eficiente grandes conjuntos de dados.

############################# Steps ############################
steps:
    enable: true
    title: "Guia para Busca Sensível a Maiúsculas em Arquivos DOCX"
    content: |
      Usando [GroupDocs.Search](/search/java/), você pode realizar busca sensível a maiúsculas em documentos DOCX, aprimorando seus projetos Java.
      
      1. Defina a pasta para armazenar o índice de busca.
      2. Selecione a pasta contendo arquivos DOCX.
      3. Execute a busca sensível a maiúsculas e colete os resultados.
      4. Processe e utilize os resultados da busca.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Defina o local para o armazenamento do índice
        Index index = new Index("c:/MyIndex");

        // Aponte para a pasta contendo os documentos a serem pesquisados
        index.add("c:/MyDocuments");

        // Ative o modo sensível a maiúsculas nas configurações de busca
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Execute a busca
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ferramentas Avançadas de Busca e Indexação"
  description: "Com GroupDocs.Search for Java, você pode otimizar a busca e indexação de documentos em mais de 70 formatos, facilitando a localização e organização das informações."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Destaques do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de Texto Flexível"
      content: "Pesquise por documentos como PDFs, arquivos do Word, planilhas e apresentações. Utilize ferramentas como correspondência exata, pesquisa difusa e suporte a curingas para refinar seus resultados."

    # feature loop
    - title: "Gerenciamento Eficiente de Índices"
      content: "Organize e indexe grandes conjuntos de dados para melhorar a velocidade e o desempenho da busca ao lidar com grandes coleções de documentos."

    # feature loop
    - title: "Suporte a Idiomas Globais"
      content: "Realize buscas em mais de 80 idiomas, acomodando diferentes layouts de teclado e variações linguísticas para melhorar a precisão."

    # feature loop
    - title: "Filtros de Busca Personalizáveis"
      content: "Ajuste os critérios de busca com opções como sensibilidade a maiúsculas, filtragem por intervalo de datas e exclusão de palavras ou dados indesejados durante a indexação."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemplo: Consultas de Busca Sensível a Maiúsculas"
      content: |
        Este exemplo demonstra como implementar buscas sensíveis a maiúsculas para documentos DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Defina o diretório para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Especifique a localização da pasta de documentos
          index.add("c:/MyDocuments");

          // Configure uma consulta de busca
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Ative a sensibilidade a maiúsculas nas opções de busca
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Realize a busca nos documentos
          SearchResult result = index.search(wordQuery, options);
          
          // Processe os resultados obtidos
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Copiar"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente as funcionalidades do GroupDocs.Search gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Download do Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Visão Geral das Principais Funcionalidades"
    exclude: "case-sensitive"
    description: "Descubra as robustas e eficazes capacidades de busca oferecidas pelo GroupDocs.Search for Java."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formatos de Arquivo Suportados para Busca"
    exclude: "DOCX"
    description: "GroupDocs.Search funciona com mais de 70 formatos de documentos populares, oferecendo configurações de busca personalizáveis e indexação eficiente."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---