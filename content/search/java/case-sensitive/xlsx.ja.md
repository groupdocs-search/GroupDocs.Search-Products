
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:31
draft: false
lang: ja
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "XLSXでのケースセンシティブ検索をJavaで行う"
head_description: "GroupDocs.Search for Java APIは、Java開発者が複数のドキュメントタイプにわたってケースセンシティブ検索を実行できるようにします。"

############################# Header ############################
title: "ケースセンシティブドキュメント検索" 
description: "GroupDocs.Search for Javaを使用すると、Javaプロジェクトにおいて精密なケースセンシティブ検索機能を実装できます。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で入手"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchについて学ぶ"
    link: "/search/java/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)は、さまざまなドキュメントにわたるテキスト検索およびインデックス作成のための多用途ツールです。PDF、Wordファイル、PowerPointプレゼンテーション、Excelシート、画像、ZIPなど70を超えるフォーマットをサポートしており、大規模なデータセットを効率的に扱うことができます。

############################# Steps ############################
steps:
    enable: true
    title: "XLSXファイルにおけるケースセンシティブ検索のガイド"
    content: |
      [GroupDocs.Search](/search/java/)を使用すると、XLSXドキュメントでケースセンシティブ検索が可能になり、Javaプロジェクトが向上します。
      
      1. 検索インデックスを保存するフォルダーを設定します。
      2. XLSXファイルを含むフォルダーを選択します。
      3. ケースセンシティブ検索を実行し、結果を収集します。
      4. 検索結果を処理し、利用します。
   
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
        // インデックスストレージの位置を定義します
        Index index = new Index("c:/MyIndex");

        // 検索するドキュメントを含むフォルダーを指定します
        index.add("c:/MyDocuments");

        // 検索設定でケースセンシティブモードを有効にします
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // 検索を実行します
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "強化された検索およびインデクシングツール"
  description: "GroupDocs.Search for Javaを使用すると、70を超えるフォーマットでのドキュメントの検索およびインデクシングが簡素化され、情報の検索と整理が容易になります。"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Searchのハイライト"
  features:
    # feature loop
    - title: "柔軟なテキスト検索"
      content: "PDF、Wordファイル、スプレッドシート、プレゼンテーションなどのドキュメントを検索できます。完全一致、ファジー検索、およびワイルドカードサポートを使用して検索結果を絞り込むことができます。"

    # feature loop
    - title: "効率的なインデックス管理"
      content: "大規模なデータセットを整理およびインデックス化し、大きなドキュメントコレクションを扱う際の検索速度とパフォーマンスを向上させます。"

    # feature loop
    - title: "グローバルな言語サポート"
      content: "80を超える言語での検索が可能で、さまざまなキーボードレイアウトと言語的バリエーションに対応し、精度を向上させます。"

    # feature loop
    - title: "カスタマイズ可能な検索フィルター"
      content: "ケースセンシティブ、日付範囲フィルタリング、インデクシング時に不要な単語やデータを除外するオプションなどで検索条件を調整できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "例：ケースセンシティブ検索クエリ"
      content: |
        この例では、XLSX文書に対してケースセンシティブ検索を実装する方法を示しています。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 検索インデックスのディレクトリを定義します
          Index index = new Index("c:/MyIndex");
              
          // 文書フォルダーの位置を指定します
          index.add("c:/MyDocuments");

          // 検索クエリを設定します
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // 検索オプションでケースセンシティブを有効にします
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // ドキュメント検索を実行します
          SearchResult result = index.search(wordQuery, options);
          
          // 取得した結果を処理します
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "主な機能の概要"
    exclude: "case-sensitive"
    description: "GroupDocs.Search for Javaが提供する強力で効果的な検索機能を発見してください。"
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
    title: "検索に対応するファイル形式"
    exclude: "XLSX"
    description: "GroupDocs.Searchは70を超える一般的なドキュメントフォーマットで動作し、カスタマイズ可能な検索設定と効率的なインデクシングを提供します。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---