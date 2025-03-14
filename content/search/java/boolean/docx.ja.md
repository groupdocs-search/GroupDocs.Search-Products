
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: ja
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "DOCXにおけるJavaでのブール検索"
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
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)は、ドキュメント内のテキスト検索やデータインデックス作成のために設計された多目的ライブラリです。PDF、Word、Excel、PowerPoint、画像、ZIPアーカイブなど、70以上のファイル形式をサポートし、大規模なデータコレクションの検索を効率化します。

############################# Steps ############################
steps:
    enable: true
    title: "DOCXドキュメントでのブール検索の手順"
    content: |
      [GroupDocs.Search](/search/java/)は、DOCXドキュメント内で簡易なテキスト検索を可能にします。ブール条件をサポートすることで、Javaアプリケーションにおける検索精度を向上させることができます。
      
      1. 検索インデックスを保存するフォルダを指定します。
      2. DOCXドキュメントを含むフォルダを選択します。
      3. 検索クエリを実行し、結果を取得します。
      4. 取得した結果を処理します。
   
    code:
      platform: "java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "検索結果"
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
        - title: "ドキュメント"
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
        この例では、DOCXファイルでのブール検索を実行する方法を示します。
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
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
        links:
          #  loop
          - title: "さらに例を見る"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスを要求してください"
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
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "人気のドキュメント形式を検索"
    exclude: "DOCX"
    description: "GroupDocs.Searchは70以上のファイル形式をサポートしており、検索ルールをカスタマイズし、インデックス作成を用いてパフォーマンスを最適化できます。"
    items: 
        # format loop 1
        - name: "DOCXのブール検索"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFのブール検索"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXのブール検索"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTのブール検索"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXのブール検索"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---