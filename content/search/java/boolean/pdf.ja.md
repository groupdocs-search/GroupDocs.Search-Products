
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: ja
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "PDFにおけるJavaでのブール検索"
head_description: "GroupDocs.Search for Javaを使用すると、開発者はAND、OR、NOTなどのブール演算子を用いてドキュメント検索を実行できます。"

############################# Header ############################
title: "ブールテキスト検索" 
description: "GroupDocs.Search for Javaを利用して、Javaプロジェクト内で高度なブール（AND、OR、NOT）検索クエリを作成します。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchについて"
    link: "/search/java/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)は、ドキュメント内のテキスト検索やデータインデックス作成のために設計された多目的ライブラリです。PDF、Word、Excel、PowerPoint、画像、ZIPアーカイブなど、70以上のファイル形式をサポートし、大規模なデータコレクションの検索を効率化します。

############################# Steps ############################
steps:
    enable: true
    title: "PDFドキュメントでのブール検索の手順"
    content: |
      [GroupDocs.Search](/search/java/)は、PDFドキュメント内で簡易なテキスト検索を可能にします。ブール条件をサポートすることで、Javaアプリケーションにおける検索精度を向上させることができます。
      
      1. 検索インデックスを保存するフォルダを指定します。
      2. PDFドキュメントを含むフォルダを選択します。
      3. 検索クエリを実行し、結果を取得します。
      4. 取得した結果を処理します。
   
    code:
      platform: "java"
      copy_title: "コピー"
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
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらに例を見る"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // インデックスフォルダのパスを設定
        Index index = new Index("c:/MyIndex");

        // 検索対象のドキュメントが含まれるフォルダのパスを提供
        index.add("c:/MyDocuments");

        // 複雑なクエリで検索を実行
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ドキュメント検索とインデックス作成のための強力なツール"
  description: "GroupDocs.Search for Javaは、70を超えるフォーマットでのテキスト検索とデータインデックス作成を簡素化します。その高度なツールにより、コンテンツの検索と管理が容易になります。"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Searchの主な機能"
  features:
    # feature loop
    - title: "包括的なテキスト検索"
      content: "PDF、Wordドキュメント、プレゼンテーション、スプレッドシートなど、複数のフォーマットで検索が可能です。結果を絞り込むために、正確な一致、ファジー検索、ワイルドカードクエリなどのオプションを利用できます。"

    # feature loop
    - title: "効率的なデータインデックス作成"
      content: "迅速なドキュメント検索のためにインデックスを構築および維持します。この機能はデータを効率的に整理し、大規模なドキュメントコレクションを扱いやすくします。"

    # feature loop
    - title: "多言語サポート"
      content: "80以上の言語で書かれたドキュメントを検索します。形態素を利用し、さまざまなキーボードレイアウトを活用することで、精度を向上させます。"

    # feature loop
    - title: "柔軟な検索カスタマイズ"
      content: "大文字小文字の区別、日付範囲フィルター、除外などの機能を使用して、検索結果をさらに絞り込むための設定を調整できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "複雑なブール検索クエリの使用"
      content: |
        この例では、PDFファイルでのブール検索を実行する方法を示します。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 検索インデックス用のフォルダを設定
          Index index = new Index("c:/MyIndex");
              
          // 検索対象のドキュメントへのパスを提供
          index.add("c:/MyDocuments");

          // ブールロジックを用いてクエリを構築
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // 検索結果を取得
          SearchResult result = index.search(booleanQuery);
          
          // 取得した結果を処理
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "コピー"
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
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pdf"
        links:
          #  loop
          - title: "さらに例を見る"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "ドキュメンテーション"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Mavenのダウンロード"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主要機能の概要"
    exclude: "boolean"
    description: "強力で効率的な検索機能を解放します"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "人気のドキュメント形式を検索"
    exclude: "PDF"
    description: "GroupDocs.Searchは70以上のファイル形式をサポートしており、検索ルールをカスタマイズし、インデックス作成を用いてパフォーマンスを最適化できます。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---