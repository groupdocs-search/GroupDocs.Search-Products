
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: ja
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "XLSX ドキュメント内のテキストを見つける GroupDocs.Search for Java"
head_description: "GroupDocs.Search for Java は Java 開発者が様々なドキュメントフォーマット内でテキストを迅速に検索できるようにサポートします。"

############################# Header ############################
title: "スマートなドキュメントテキスト検索" 
description: "GroupDocs.Search for Java を使用すると、Java アプリケーション内の複数のドキュメントタイプからテキストをシームレスに検索および抽出できます。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアルを取得"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search は何をしますか？"
    link: "/search/java/"
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) は、PDF、Word、PowerPoint、Excel、画像、ZIPアーカイブなど、70以上のファイルフォーマットをサポートする強力なドキュメント検索およびインデックス作成ライブラリです。大量のドキュメントコレクションに対して、高速で正確、かつスケーラブルな検索機能を提供します。

############################# Steps ############################
steps:
    enable: true
    title: "XLSX ファイル内でのテキスト検索を実行する"
    content: |
      [GroupDocs.Search](/search/java/) は洗練されたロジックとインデックス作成を用いて XLSX ファイルを検索し、Java アプリケーション内の検索精度を向上させます。
      
      1. 検索インデックスを保存するディレクトリを設定します。
      2. XLSX ファイルが含まれるフォルダを選択します。
      3. 追加の検索オプションを定義します。
      4. 検索を実行し、結果を分析します。
   
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
        // 検索インデックスを格納するディレクトリを設定します
        Index index = new Index("c:/MyIndex");

        // 検索可能なドキュメントが含まれるフォルダを指定します
        index.add("c:/MyDocuments");

        // 同音異義語検索を有効にして、発音が似ている単語を一致させます
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // 高度な検索クエリを実行します
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "強化された検索およびインデックス作成機能"
  description: "GroupDocs.Search for Java は70以上のドキュメントフォーマットにわたるテキストの検索とインデックス作成を簡素化し、情報を迅速に管理および取得するための効率的なツールを提供します。"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search のコア機能"
  features:
    # feature loop
    - title: "包括的なテキスト検索"
      content: "PDF、Wordドキュメント、PowerPointプレゼンテーション、スプレッドシートなど、複数のドキュメントフォーマットを横断してテキストを見つけます。正確な一致、あいまい検索、ワイルドカードを使用して、検索結果を洗練させることができます。"

    # feature loop
    - title: "大規模データ向けの最適化されたインデックス作成"
      content: "検索を高速化するために構造化されたインデックスを作成し、広範なドキュメントリポジトリを効率的にナビゲートできるようにします。"

    # feature loop
    - title: "複数の言語をサポート"
      content: "80以上の言語での検索が可能で、異なるキーボードレイアウトや単語形態変化のサポートを内蔵しており、精度を向上させます。"

    # feature loop
    - title: "柔軟な検索設定"
      content: "大文字小文字の区別、日付ベースのフィルタリング、特定の単語を除外するオプションなどを使用して、検索結果を正確にカスタマイズできます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度な検索クエリの実装"
      content: |
        この例では、XLSX ドキュメント内を効率的に検索するための検索クエリの使用方法を示します。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 検索インデックス用のディレクトリを定義します
          Index index = new Index("c:/MyIndex");
              
          // ドキュメントのファイルパスを提供します
          index.add("c:/MyDocuments");

          // 暗号化されたドキュメントのためのパスワードを入力します
          index.getDictionaries().getDocumentPasswords().add("protected.xlsx", "123456");

          // 類似の単語を検出するためにあいまい検索を有効にします
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // 検索結果を取得します
          SearchResult result = index.Search("Loarem", options);
          
          // 検索結果を処理し、分析します
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    exclude: "document"
    description: "効率性と精度を重視した高性能なテキスト検索機能を発見してください。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "GroupDocs.Search を使用して XLSX ドキュメント全体の情報を見つける"
    exclude: "XLSX"
    description: "70以上のフォーマットをサポートする GroupDocs.Search は、オフィスファイルを含む高速検索を実現します。"
    items: 
        # format loop 1
        - name: "DOCXドキュメント内を検索"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFドキュメント内を検索"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXドキュメント内を検索"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTドキュメント内を検索"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXドキュメント内を検索"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---