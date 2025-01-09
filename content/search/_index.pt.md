---
############################# Static ############################
layout: "family"
date:  2025-01-09T15:38:59
draft: false

product: "Search"
product_tag: "search"

lang: pt

############################# Head ############################
head_title: "Pesquisa e Indexação de Texto em Documentos | APIs e Aplicativo Web Gratuito"
head_description: "Realize busca eficiente de texto e indexação de dados em PDF, MS Office, OpenDocument e outros formatos de arquivo populares usando nossas APIs ou o aplicativo Document Search online gratuito."

############################# Header ############################
title: "Solução Abrangente de Pesquisa e Indexação de Documentos"
description:  |
  Realize pesquisa de texto e indexação em PDF, Microsoft Office, OpenOffice e muitos outros formatos de arquivo de documentos.

  Localize rapidamente informações em grandes coleções de documentos com capacidades avançadas de busca de texto completo.

  Personalize recursos de pesquisa como sinônimos, pesquisa difusa e radicalização para aprimorar a precisão e os resultados.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Escolha sua plataforma"
  title: "Independência de Plataforma"
  description: "GroupDocs.Search é compatível com os seguintes sistemas operacionais e frameworks:"
  details_link_title: "Saiba mais"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Qualquer outro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Recursos Chave do GroupDocs.Search"
  description: "GroupDocs.Search fornece ferramentas poderosas para indexação e busca de texto em formatos de documentos populares. Simplifique e melhore a gestão de documentos com funcionalidades avançadas de busca."

  items:
    # items loop
    - icon: "view"
      title: "Busca de texto avançada"
      content: "Realize buscas rápidas e precisas de texto em documentos indexados."

    # items loop
    - icon: "manipulate"
      title: "Opções de busca personalizáveis"
      content: "Utilize recursos como pesquisa difusa, sinônimos e radicalização para resultados mais precisos."

    # items loop
    - icon: "merge"
      title: "Suporte a múltiplos formatos"
      content: "Indexe e busque conteúdo em Microsoft Office, PDF, OpenOffice e outros formatos comuns."

    # items loop
    - icon: "additional"
      title: "Indexação eficiente"
      content: "Construa e mantenha índices rapidamente para grandes coleções de documentos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Buscando texto em formatos de documentos populares"
  description: "GroupDocs.Search exemplos de código"
  items:
    # code sample loop
    - title: "Busca de Texto"
      content: |
       GroupDocs.Search é uma ferramenta poderosa para encontrar texto em documentos. Você pode pesquisar através de múltiplos documentos em vários formatos armazenados em uma pasta específica. Os resultados da pesquisa são salvos em uma pasta separada, permitindo que você acesse e reutilize-os sem realizar a busca novamente.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Crie uma instância da classe Index, especificando a pasta para armazenar os índices.
            Index index = new Index("\\Index Folder");

            //Especifique o caminho dos documentos onde a busca será realizada.
            index.Add("\\Documents Folder");

            //Crie uma instância do objeto SearchOptions.
            SearchOptions options = new SearchOptions();

            //Realize a busca pelo texto desejado.
            SearchResult result = index.Search("ipsum dolor", options);

            //Trate e processe os resultados da busca.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Crie uma instância da classe Index, especificando a pasta para armazenar os índices.
            Index index = new Index("\\Index Folder");

            //Especifique o caminho dos documentos onde a busca será realizada.
            index.add("\\Documents Folder");

            //Crie uma instância do objeto SearchOptions.
            SearchOptions options = new SearchOptions();

            //Realize a busca pelo texto desejado.
            SearchResult result = index.search("ipsum dolor", options);

            //Trate e processe os resultados da busca.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Crie uma instância da classe Index, especificando a pasta para armazenar os índices.
            const index = new searchLib.Index('\\Index Folder');

            //Especifique o caminho dos documentos onde a busca será realizada.
            index.add('\\Documents Folder');

            //Crie uma instância do objeto SearchOptions.
            const options = new searchLib.SearchOptions();

            //Realize a busca pelo texto desejado.
            const result = index.search('ipsum dolor', options);

            //Trate e processe os resultados da busca.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Suporta mais de 70 formatos de arquivo"
  description: "GroupDocs.Search suporta quase todos os formatos de arquivo amplamente usados"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Estatísticas do Nosso Produto"
  description: "Descubra métricas chave que mostram nosso desempenho, alcance e crescimento."

  items:
    # items loop
    - number: "70+"
      title: "Formatos Suportados"
      content: "Oferecemos compatibilidade com mais de 70 formatos populares de documentos."

    # items loop
    - number: "500k"
      title: "Downloads do NuGet"
      content: "GroupDocs.Search para .NET foi baixado mais de 500.000 vezes no NuGet."

    # items loop
    - number: "12k"
      title: "Downloads do Maven"
      content: "Desenvolvedores Java baixaram GroupDocs.Search mais de 12.000 vezes do Maven."

    # items loop
    - number: "150+"
      title: "Clientes Satisfeitos"
      content: "Desenvolvedores e empresas líderes em todo o mundo confiam em nossos produtos para soluções inovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nossos Clientes Satisfeitos"
  description: "As bibliotecas GroupDocs são confiáveis por marcas e organizações líderes em todo o mundo."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Comece sua jornada hoje!"
  description: "Experimente GroupDocs.Search gratuitamente na sua plataforma preferida."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Perguntas Frequentes"
  description: "Encontre respostas para perguntas comuns sobre GroupDocs.Search."

  items:
    # items loop
    - question: "O GroupDocs.Search requer ferramentas externas para buscar documentos?"
      answer: "Não, GroupDocs.Search funciona como uma solução autônoma e não precisa de ferramentas ou software adicionais como Adobe Acrobat ou Microsoft Office para realizar buscas."

    # items loop
    - question: "Posso testar GroupDocs.Search antes de comprar?"
      answer: "Sim, você pode! GroupDocs.Search oferece um teste gratuito. Você pode explorar seus recursos, embora a versão de teste possa incluir limitações, como marcas d'água ou funcionalidades restritas. Para desbloquear todos os recursos, você pode solicitar uma licença temporária gratuita de 30 dias. Saiba mais na página de [licença temporária](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Quais opções de licenciamento estão disponíveis?"
      answer: "Oferecemos vários modelos de licenciamento para GroupDocs.Search, adaptados a diferentes necessidades. Escolha uma licença com base no tamanho da sua equipe, cenário de uso ou se você precisa do SDK/API para distribuição ao cliente. Para uso flexível, considere uma licença medida, onde você paga com base no uso real. Saiba mais sobre suas opções na página de [preços](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Aplicativos Web"
  description: "Explore GroupDocs.Search com nosso aplicativo web gratuito. Realize buscas de texto e indexação em mais de 70 formatos de arquivo populares diretamente no seu navegador—completamente grátis."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Pesquise em PDF, Excel, Word, PowerPoint e outros tipos de arquivo diretamente do seu navegador."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Carregue DOCX para realizar buscas de texto avançadas sem precisar instalar software."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Teste as capacidades de indexação e recuperação de PDFs em vários formatos gratuitamente."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---