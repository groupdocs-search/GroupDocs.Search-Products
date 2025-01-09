---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: pt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Biblioteca de Pesquisa e Indexação de Texto Node.js para Documentos, PDF, Office e Web"
head_description: "Solução de pesquisa de texto avançada para aplicativos Node.js para buscar, indexar e coletar dados de documentos: PDF, Word, Excel, apresentações, e-mails e formatos de arquivos da web."

############################# Header ############################
title: "Pesquise e Índice Documentos usando API Node.js"
description: "Aprimore Aplicativos Node.js implementando Pesquisa de Texto em Todos os Formatos de Documentos Populares."
words:
  for: "para"

actions:
  main: "Download Gratuito do NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Comece sua jornada hoje!"
  description: "Explore as capacidades do GroupDocs.Search gratuitamente ou obtenha uma licença para desbloquear seu potencial completo."

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Realize Busca de Texto em uma Pasta com JavaScript"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Crie um índice para seus documentos
    const index = new searchLib.Index('c:/MyIndex');

    // Adicione documentos ao índice para buscas eficientes
    index.add('c:/MyDocuments');
    
    // Pesquise palavras ou frases específicas, como
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Visão Geral"
  description: "Biblioteca Node.js JavaScript para busca de texto"
  features:
    # feature loop
    - title: "Operações de Indexação e Busca Node.js"
      content: "A indexação no GroupDocs.Search for Node.js via Java coleta, armazena e analisa dados para operações de busca precisas e eficientes. Esses índices são frequentemente usados para realizar buscas."

    # feature loop
    - title: "Mescle Múltiplos Índices para Aumentar a Eficiência da Busca"
      content: "A API do GroupDocs.Search for Node.js via Java permite a mesclagem de múltiplos índices em um. As modificações frequentes criam vários índices delta, o que pode diminuir o desempenho da busca. Nossa solução mescla esses índices delta em um índice comum, contendo todas as informações dos índices delta mesclados, melhorando significativamente a eficiência da busca, mantendo os índices delta inalterados. Várias funcionalidades podem ser configuradas para aperfeiçoar esse processo."

    # feature loop
    - title: "Reconhecer Consultas de Busca de Diferentes Layouts de Teclado"
      content: "GroupDocs.Search for Node.js via Java reconhece consultas de busca que não correspondem ao layout do teclado. Atualmente, o suporte é a 88 idiomas e 164 layouts de teclado diferentes."

    # feature loop
    - title: "Pesquise Usando Formas Morfológicas de Palavras"
      content: "Com GroupDocs.Search for Node.js via Java, você pode buscar por várias formas de palavras, como substantivos singulares e plurais ou todas as formas de um verbo. Idiomas em inglês e não-ingleses podem ser personalizados para formas específicas de palavras."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de Plataforma"
  description: "GroupDocs.Search for Node.js via Java suporta todos os sistemas operacionais populares e gerenciadores de pacotes."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Search for Node.js via Java permite processar uma ampla gama de formatos de arquivo. [Explore a lista completa](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos de Escritório Populares
        * **Portátil:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Texto:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formatos de Mídia
        * **Formatos de imagem populares:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Imagens multi-página:** GIF, WEBP, TIFF
        * **Áudio:** MP3, WAV
        * **Vídeo:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Outros
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Outros:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Recursos do GroupDocs.Search for Node.js via Java"
  description: "Controle o conteúdo de documentos empresariais usando nosso motor de busca avançado, que suporta formatos de arquivo populares, incluindo PDF, DOCX, XLSX, PPTX e mais."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parâmetros Flexíveis"
      content: "Use Intervalo de Datas e Sensibilidade a Maiúsculas como Parâmetros de Busca"

    # feature loop
    - icon: "detect"
      title: "Busca com Correção Ortográfica"
      content: "Use Frases de Busca com Correção Ortográfica e Caracteres Curinga e Pule Caracteres Especiais nas Consultas"

    # feature loop
    - icon: "collect"
      title: "Filtragem de Resultados"
      content: "Configure a Filtragem de Documentos nos Resultados da Busca"

    # feature loop
    - icon: "get"
      title: "Importação e Exportação"
      content: "Realize Importação ou Use Lista para Modificar Caracteres durante a Indexação e Exporte para um Arquivo"

    # feature loop
    - icon: "remove"
      title: "Pule Dados Desnecessários"
      content: "Selecione Ignorar Indexação para Arquivos Específicos e Pule Palavras Específicas para Indexar Mais Rápido"

    # feature loop
    - icon: "style"
      title: "Processamento de URL"
      content: "Extraia Texto Formatado em HTML para um Arquivo e Gere URL para Navegar nos Resultados da Busca em HTML"

    # feature loop
    - icon: "detect"
      title: "Busca Rápida"
      content: "Divida a Busca em Pedaços Menores para Pesquisar Rapidamente Grandes Índices"

    # feature loop
    - icon: "manipulate"
      title: "Processamento de Fluxo"
      content: "Indexe Documentos de Fluxos e Estruturas de Dados"

    # feature loop
    - icon: "compare"
      title: "Trate Erros de Digitação"
      content: "Habilite o Número Exato de Ocorrências para cada Palavra Encontrada para Oferecer Sugestões de Palavras Alternativas em caso de Erros de Digitação"

    # feature loop
    - icon: "unreadable_characters"
      title: "Suporte a Arquivos Compactados"
      content: "Indexe Arquivos ZIP dentro de outros Arquivos ZIP e Recupere Listas de Arquivos Indexados em um Arquivo Compactado."

    # feature loop
    - icon: "hidden_print"
      title: "Economia de Espaço em Disco"
      content: "Economize Espaço com Indexação Compacta e Indexe Documentos Protegidos por Senha."

    # feature loop
    - icon: "style"
      title: "Sinônimos Personalizados"
      content: "Adicione Sinônimos em Inglês ao Dicionário Padrão de Sinônimos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemplos de código"
  description: "Explore as funcionalidades do GroupDocs.Search for Node.js via Java com exemplos."
  items:
    # code sample loop
    - title: "Use busca 'difusa' para aumentar a produtividade"
      content: |
        Aproveite a funcionalidade flexível do GroupDocs.Search for Node.js via Java para aprimorar o controle do conteúdo de documentos por meio de algoritmos de busca sofisticados. [Saiba mais](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Como processar o resultado da busca">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Crie um índice
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Configure as opções de busca
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Busque documentos contendo a palavra 'água' ou a frase 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Processe o resultado da busca
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Expressões regulares estão disponíveis para cenários de busca avançados"
      content: |
        GroupDocs.Search for Node.js via Java permite o uso de expressões regulares para restringir os resultados da busca. [Mergulhe em técnicas de busca avançadas](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Como buscar usando expressões regulares">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Crie um índice
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Busque a frase em formato de texto

        // O primeiro caractere ^ no início indica que esta é uma consulta de expressão regular
        const query = '^^(.)\\1{1,}';
        // Busque dois ou mais caracteres idênticos no começo de uma palavra
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
