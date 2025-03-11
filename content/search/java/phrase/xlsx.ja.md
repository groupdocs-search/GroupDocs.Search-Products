
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: ja
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "XLSX内のフレーズを検索する - GroupDocs.Search for Java"
head_description: "GroupDocs.Search for Javaは、文書コンテンツの高度なフレーズ検索機能を提供し、Javaアプリケーションを強化します。"

############################# Header ############################
title: "文書内のフレーズを特定する" 
description: "GroupDocs.Search for Javaを使用して特定のフレーズを迅速に見つけましょう。あなたのJavaアプリケーションに強力な検索機能を追加します。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ダウンロード"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchの機能"
    link: "/search/java/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)は、文書内のテキストをインデックス化し検索するための堅牢なライブラリです。PDF、Word文書、Excelスプレッドシート、画像、ZIPファイルなど70以上のファイル形式をサポートし、高速かつ正確な検索結果を保証します。

############################# Steps ############################
steps:
    enable: true
    title: "XLSX文書内のフレーズを見つける方法"
    content: |
      [GroupDocs.Search](/search/java/)は、XLSX文書内のフレーズ検索を簡素化します。Javaアプリケーション内で検索結果を refinします。
      
      1. 検索インデックスディレクトリを作成します。
      2. XLSXファイルが含まれるフォルダーを指定します。
      3. 検索パラメーターを調整します。
      4. 検索結果を取得し、分析します。
   
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
        // 検索インデックスパスを定義します
        Index index = new Index("c:/MyIndex");

        // 文書を含むフォルダーを指定します
        index.add("c:/MyDocuments");

        // 検索設定を行います
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // 検索クエリを実行します
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Java文書検索エンジンを探索する"
  description: "GroupDocs.Search for Javaは、70以上のファイル形式でフレーズ検索を可能にします。高度な検索機能を使用してデータを簡単に見つけ、整理できます。"
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Searchの主要機能"
  features:
    # feature loop
    - title: "フレーズ検索"
      content: "PDF、Wordファイル、プレゼンテーション、スプレッドシートなどのビジネス文書内の正確なフレーズを特定します。正確なフレーズが不明な場合は、ワイルドカードやその他のオプションを使用できます。"

    # feature loop
    - title: "最適化されたデータインデックス作成"
      content: "検索インデックスを作成し再利用することで文書検索を高速化します。インデックス作成はデータを効率的に整理し、より迅速かつ正確な検索を実現します。"

    # feature loop
    - title: "多言語対応"
      content: "80以上の言語で文書を検索します。異なるキーボードレイアウトや形態素分析をサポートし、検索精度を向上させます。"

    # feature loop
    - title: "高度な検索オプション"
      content: "大文字小文字の区別、ファジー検索、同音異義語の一致、文書フィルタリングなど、強力な機能を使用して検索をカスタマイズします。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度な検索方法の活用"
      content: |
        XLSX内での検索のためのクエリの構築方法を学びます。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 検索インデックス用のディレクトリを定義します
          Index index = new Index("c:/MyIndex");
              
          // ターゲット文書へのパスを設定します
          index.add("c:/MyDocuments");

          // 特定のフレーズ用の検索クエリを作成します
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // 検索結果を取得します
          SearchResult result = index.search(query);
          
          // 取得した結果を処理し活用します
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "高度な検索機能"
    exclude: "phrase"
    description: "精度とパフォーマンスを向上させるための最先端の検索機能を活用します。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ビジネス文書内のフレーズを検索する"
    exclude: "XLSX"
    description: "GroupDocs.Searchは70以上の文書形式でフレーズ検索を可能にします。効率的な検索のために高度なオプションとインデックス作成を活用します。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---