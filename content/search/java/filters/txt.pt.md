
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:36
draft: false
lang: pt
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Pesquisar em documentos TXT usando Java"
head_description: "GroupDocs.Search for Java adiciona uma poderosa busca por texto em aplicações Java, suportando vários formatos de documentos empresariais."

############################# Header ############################
title: "Encontre texto em documentos empresariais" 
description: "GroupDocs.Search for Java permite buscar texto em documentos usando consultas flexíveis e precisas. Integre facilmente a funcionalidade de busca em aplicações Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) é uma biblioteca robusta para busca rápida de texto e indexação de documentos. Suporta mais de 70 formatos de arquivo, incluindo padrões da indústria como PDF, Word, Excel e PowerPoint. Aprimore suas aplicações com capacidades de busca precisas e de alta velocidade.

############################# Steps ############################
steps:
    enable: true
    title: "Como pesquisar em documentos TXT"
    content: |
      [GroupDocs.Search](/search/java/) permite buscas textuais rápidas e eficientes em documentos TXT, perfeito para aplicações Java.
      
      1. Especifique uma pasta para armazenar o índice de busca.
      2. Selecione a pasta contendo seus documentos.
      3. Configure as opções de busca para limitar os resultados a documentos TXT.
      4. Execute a busca e obtenha os resultados.
   
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
        // Diretório para armazenar o índice de busca reutilizável
        Index index = new Index("c:/MyIndex");

        // Pasta contendo os documentos
        index.add("c:/MyDocuments");

        // Filtrar buscas por formato de documento
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".txt");

        // Recuperar resultados da busca
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades de busca aprimoradas"
  description: "GroupDocs.Search for Java oferece busca avançada de texto em mais de 70 formatos de arquivo. A indexação acelera as buscas e melhora a eficiência na gestão de documentos."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Recursos principais do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de texto poderosa"
      content: "Encontre texto em formatos de documentos populares, como PDFs, arquivos do Word, apresentações e planilhas. Suporta múltiplos métodos de busca, incluindo busca difusa, homônimos e curingas."

    # feature loop
    - title: "Indexação otimizada para melhor desempenho"
      content: "Crie e reutilize índices de pesquisa para aumentar a velocidade e eficiência da busca, especialmente em grandes coleções de documentos."

    # feature loop
    - title: "Suporte a busca multilíngue"
      content: "Pesquise em documentos escritos em mais de 80 idiomas. Detecta diferentes layouts de teclado e variações de palavras para maior precisão."

    # feature loop
    - title: "Opções de busca personalizáveis"
      content: "Refine os resultados da busca com filtros, expressões regulares e outras configurações avançadas de busca."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrar documentos antes da busca"
      content: |
        Aprenda a como refinar buscas usando filtros
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Configure um índice que exclua certos formatos de arquivo
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Especifique o caminho de armazenamento dos documentos
          index.add("c:/MyDocuments");

          // Recupere os resultados da busca
          SearchResult result = index.search("Lorem", options);
          
          // Processar e usar os resultados da busca
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Recursos principais"
    exclude: "filters"
    description: "Realize buscas textuais precisas e eficientes."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Pesquisar em documentos empresariais"
    exclude: "TXT"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo, facilitando a busca em documentos de escritório amplamente utilizados."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---