
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: ja
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "PDF ドキュメント内を検索 - GroupDocs.Search for Java"
head_description: "GroupDocs.Search for Java は、さまざまなビジネス文書形式をサポートし、Java アプリケーションに強力なテキスト検索を追加します。"

############################# Header ############################
title: "ビジネス文書内のテキストを見つける" 
description: "GroupDocs.Search for Java を使用すると、柔軟で正確なクエリを用いて文書内をテキスト検索できます。Java アプリケーションに検索機能を統合してください。"
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
    title: "GroupDocs.Search とは？"
    link: "/search/java/"
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) は、迅速なテキスト検索とドキュメントインデックス作成のための強力なライブラリです。PDF、Word、Excel、PowerPointなど、業界標準の70以上のファイル形式をサポートしています。高速度で正確な検索能力を利用して、アプリケーションを強化しましょう。

############################# Steps ############################
steps:
    enable: true
    title: "PDF ドキュメント内を検索する方法"
    content: |
      [GroupDocs.Search](/search/java/) を用いることで、PDF ドキュメント内で迅速かつ効率的にテキスト検索が可能です。Java アプリケーションに最適です。
      
      1. 検索インデックスを保存するフォルダーを指定します。
      2. ドキュメントを含むフォルダーを選択します。
      3. PDF ドキュメントに結果を制限するために検索オプションを設定します。
      4. 検索を実行し、結果を取得します。
   
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
        // 再利用可能な検索インデックスを保存するためのディレクトリ
        Index index = new Index("c:/MyIndex");

        // ドキュメントを格納するフォルダー
        index.add("c:/MyDocuments");

        // ドキュメント形式による検索のフィルター
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // 検索結果を取得
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "拡張された検索機能"
  description: "GroupDocs.Search for Java は70以上のファイル形式にわたる高度なテキスト検索を提供します。インデックス作成により、検索が迅速になり、ドキュメント管理の効率が向上します。"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search の主な機能"
  features:
    # feature loop
    - title: "強力なテキスト検索"
      content: "PDF、Wordファイル、プレゼンテーション、スプレッドシートなど、一般的な文書形式内のテキストを探します。ファジー検索、同音異義語、ワイルドカードなど、複数の検索方法をサポートしています。"

    # feature loop
    - title: "パフォーマンス向上のための最適化されたインデックス作成"
      content: "検索速度と効率を向上させるため、検索インデックスを作成し再利用します。特に大規模なドキュメントコレクションにおいて効果的です。"

    # feature loop
    - title: "多言語検索サポート"
      content: "80以上の言語で書かれた文書内を検索できます。異なるキーボードレイアウトや単語の変種を検出し、正確性を向上させます。"

    # feature loop
    - title: "カスタマイズ可能な検索オプション"
      content: "フィルター、正規表現、その他の高度な検索設定を使用して、検索結果を絞り込むことができます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "検索前にドキュメントをフィルタリングする"
      content: |
        フィルターを使用して検索を洗練する方法を学びます。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 特定のファイル形式を除外するインデックスを設定します。
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // ドキュメントストレージパスを指定します。
          index.add("c:/MyDocuments");

          // 検索結果を取得します。
          SearchResult result = index.search("Lorem", options);
          
          // 検索結果を処理し、利用します。
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
            link: "/examples/search/formats/searchfilters.pdf"
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
    title: "主な機能"
    exclude: "filters"
    description: "正確で効率的なテキスト検索を実行します。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ビジネス文書内を検索"
    exclude: "PDF"
    description: "GroupDocs.Search は70以上のファイル形式をサポートしており、広く使用されているオフィス文書を簡単に検索できます。"
    items: 
        # format loop 1
        - name: "DOCXの検索フィルター"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFの検索フィルター"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXの検索フィルター"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTの検索フィルター"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXの検索フィルター"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---