
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:52
draft: false
lang: pt
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buscar frases em PDF usando Java"
head_description: "GroupDocs.Search for Java aprimora aplicativos Java com capacidades avançadas de busca por frases no conteúdo de documentos."

############################# Header ############################
title: "Encontre frases em documentos" 
description: "Localize rapidamente frases específicas com GroupDocs.Search for Java. Adicione funcionalidades poderosas de busca às suas aplicações Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Recursos do GroupDocs.Search"
    link: "/search/java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) é uma biblioteca robusta para indexação e pesquisa de texto em documentos. Suporta mais de 70 formatos de arquivo, incluindo PDFs, documentos Word, planilhas Excel, imagens e arquivos ZIP, garantindo resultados de busca rápidos e precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Como encontrar frases em documentos PDF"
    content: |
      [GroupDocs.Search](/search/java/) simplifica a busca por frases em documentos PDF. Utilize várias opções para refinar os resultados de busca nas aplicações Java.
      
      1. Crie um diretório para o índice de busca.
      2. Especifique a pasta com arquivos PDF.
      3. Ajuste os parâmetros de busca.
      4. Recupere e analise os resultados da busca.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado da busca"
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
        // Defina o caminho do índice de busca
        Index index = new Index("c:/MyIndex");

        // Especifique a pasta que contém os documentos
        index.add("c:/MyDocuments");

        // Configure as preferências de busca
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Execute a consulta de busca
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explore o mecanismo de busca de documentos Java"
  description: "GroupDocs.Search for Java permite buscas de frases em mais de 70 formatos de arquivo. Encontre e organize dados usando recursos avançados de busca."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Principais capacidades do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca por frase"
      content: "Localize frases exatas em documentos empresariais, como PDFs, arquivos Word, apresentações e planilhas. Utilize curingas e outras opções quando a frase exata não for conhecida."

    # feature loop
    - title: "Indexação de dados otimizada"
      content: "Acelere buscas em documentos criando e reutilizando índices de busca. A indexação organiza dados de forma eficiente para buscas mais rápidas e precisas."

    # feature loop
    - title: "Compatibilidade multilíngue"
      content: "Pesquise documentos em mais de 80 idiomas. Suporta diferentes layouts de teclado e análise morfológica para melhorar a precisão da busca."

    # feature loop
    - title: "Opções avançadas de busca"
      content: "Customize buscas com sensibilidade a maiúsculas, busca difusa, correspondência de homófonos, filtragem de documentos e outros recursos poderosos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizando métodos avançados de busca"
      content: |
        Aprenda a construir consultas para busca em PDF.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Defina o diretório para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Defina o caminho para os documentos alvo
          index.add("c:/MyDocuments");

          // Crie uma consulta de busca para uma frase específica
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Recupere os resultados da busca
          SearchResult result = index.search(query);
          
          // Processe e utilize os resultados obtidos
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
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Capacidades avançadas de busca"
    exclude: "phrase"
    description: "Utilize funcionalidades de busca de ponta para maior precisão e desempenho."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar frases em documentos empresariais"
    exclude: "PDF"
    description: "GroupDocs.Search permite buscas por frases em mais de 70 formatos de documento. Aproveite opções avançadas e indexação para buscas eficientes."
    items: 
        # format loop 1
        - name: "Busca de frases em DOCX"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Busca de frases em PDF"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Busca de frases em PPTX"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Busca de frases em TXT"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Busca de frases em XLSX"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---