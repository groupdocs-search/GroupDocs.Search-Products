
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:52
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "TXT内のフレーズを検索する - GroupDocs.Search for Java"
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
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)は、文書内のテキストをインデックス化し検索するための堅牢なライブラリです。PDF、Word文書、Excelスプレッドシート、画像、ZIPファイルなど70以上のファイル形式をサポートし、高速かつ正確な検索結果を保証します。

############################# Steps ############################
steps:
    enable: true
    title: "TXT文書内のフレーズを見つける方法"
    content: |
      [GroupDocs.Search](/search/java/)は、TXT文書内のフレーズ検索を簡素化します。Javaアプリケーション内で検索結果を refinします。
      
      1. 検索インデックスディレクトリを作成します。
      2. TXTファイルが含まれるフォルダーを指定します。
      3. 検索パラメーターを調整します。
      4. 検索結果を取得し、分析します。
   
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
        TXT内での検索のためのクエリの構築方法を学びます。
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
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/search/formats/searchphrase.txt"
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
    title: "高度な検索機能"
    exclude: "phrase"
    description: "精度とパフォーマンスを向上させるための最先端の検索機能を活用します。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ビジネス文書内のフレーズを検索する"
    exclude: "TXT"
    description: "GroupDocs.Searchは70以上の文書形式でフレーズ検索を可能にします。効率的な検索のために高度なオプションとインデックス作成を活用します。"
    items: 
        # format loop 1
        - name: "DOCXのフレーズ検索"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFのフレーズ検索"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXのフレーズ検索"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTのフレーズ検索"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXのフレーズ検索"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---