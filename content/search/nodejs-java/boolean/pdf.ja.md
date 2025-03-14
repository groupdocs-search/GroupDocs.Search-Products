
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: ja
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PDF文書におけるブール検索 - Node.js"
head_description: "GroupDocs.Search for Node.js via Java APIを使用して、AND、OR、NOTなどのブール演算子を使用して文書コンテンツ内で高度な検索を実行します。これはJavaScript開発者向けに特化されています。"

############################# Header ############################
title: "ブール論理検索を実行する" 
description: "GroupDocs.Search for Node.js via Javaを使うことで、Node.js環境内で高度な検索クエリをブール演算子（AND、OR、NOT）を用いてシームレスに作成できます。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "今すぐダウンロード"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchとは？"
    link: "/search/nodejs-java/"
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)は、文書内のテキストを検索およびインデックス化するための強力なツールです。PDF、Word、Excel、PowerPoint、画像、ZIPファイルなど、70以上のファイル形式をサポートし、大量の情報を効率的に処理することが可能です。

############################# Steps ############################
steps:
    enable: true
    title: "PDF文書でのブール演算子による検索方法"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)を使用すれば、PDFファイル内のコンテンツを効果的に検索できます。ブール論理を用いることで、Node.js via Javaアプリケーション内で検索クエリを改善し、精度を向上させることができます。
      
      1. 検索インデックスを格納するフォルダを設定します。
      2. PDFファイルが含まれるフォルダを選択します。
      3. 検索クエリを実行し、結果を取得します。
      4. 検索結果を処理し、分析します。
   
    code:
      platform: "nodejs-java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "検索結果"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらに例を見る"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // インデックスフォルダの場所を設定します
        const index = new searchLib.Index("c:/MyIndex");

        // 検索対象の文書が含まれるフォルダを指定します
        index.add("c:/MyDocuments");

        // 高度な論理を用いて検索クエリを実行します
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書検索とインデックス作成の強力なツール"
  description: "GroupDocs.Search for Node.js via Javaは70以上のファイルタイプに対応したテキスト検索とインデックス作成を効率化し、情報の発見と管理を迅速かつ正確に行います。"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Searchの主な機能"
  features:
    # feature loop
    - title: "強化されたテキスト検索"
      content: "PDF、Word文書、プレゼンテーション、スプレッドシートなど、さまざまな形式間でテキストを迅速に見つけることができます。正確な結果を得るために、完全一致、ワイルドカード検索、ファジー検索などの機能を利用してください。"

    # feature loop
    - title: "効率的なデータインデックス作成"
      content: "大規模な文書コレクション内での検索を迅速化するためにインデックスを構築および管理します。インデックス作成により、データへの迅速かつ構造化されたアクセスが可能になります。"

    # feature loop
    - title: "多言語サポート"
      content: "80以上の言語で書かれた文書を検索できます。形態素解析サポートとキーボードレイアウトの互換性により、異なる言語での検索結果が向上します。"

    # feature loop
    - title: "柔軟な検索設定"
      content: "検索のカスタマイズが可能で、大文字小文字の区別を有効にしたり、日付フィルタを適用したり、インデックス作成時に特定の単語やデータをスキップできます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度なブール検索の例"
      content: |
        この例では、PDF文書内のコンテンツを検索するためのブールベースのクエリを作成する方法を示します。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 検索インデックス用のフォルダを定義します
          const index = new searchLib.Index("c:/MyIndex");
              
          // 検索対象の文書の場所を指定します
          index.add("c:/MyDocuments");

          // ブール演算子を使用してクエリを作成します
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // 検索結果を取得します
          const result = index.search(booleanQuery);
          
          // 検索結果を処理し、利用します
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "コピー"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pdf"
        links:
          #  loop
          - title: "さらに例を見る"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスを要求してください"
  items:
    #  loop
    - title: "NPMのダウンロード"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "GroupDocs.Searchの主要な機能"
    exclude: "boolean"
    description: "高度で効率的かつカスタマイズ可能な検索機能を活用することができます。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "一般的な文書形式を検索"
    exclude: "PDF"
    description: "GroupDocs.Searchは70以上のファイル形式をサポートしており、効率的なインデックス作成と柔軟な検索ルールを提供して、時間と労力を節約します。"
    items: 
        # format loop 1
        - name: "DOCXのブール検索"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFのブール検索"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXのブール検索"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTのブール検索"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXのブール検索"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---