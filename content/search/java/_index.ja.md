---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: ja
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Java ドキュメント検索およびインデックス作成ソリューション（PDF、Officeファイル、ウェブコンテンツ用）"
head_description: "Javaアプリケーション向けの強力なテキスト検索とインデックス作成。PDF、Word、Excel、プレゼンテーション、メール、およびウェブフォーマットでデータを簡単に検索および整理します。"

############################# Header ############################
title: "Java APIによる効率的なドキュメント検索とインデックス作成"
description: "Javaアプリケーションに、すべての一般的なドキュメント形式にわたる堅牢なテキスト検索機能を提供します。"
words:
  for: "のための"

actions:
  main: "無料でMavenをダウンロード"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "ライセンス管理"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "今日から旅を始めましょう！"
  description: "GroupDocs.Searchの機能を無料で探索するか、ライセンスを取得してその可能性を最大限に活かしてください。"

release:
  title: "バージョン {0} リリース"
  notes: "新着情報を確認する"
  downloads: "ダウンロード"

code:
  title: "Javaを使用してファイル内でテキストを検索"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // ドキュメント用のインデックスを作成
    Index index = new Index("c:/MyIndex");

    // 効率的な検索のためにインデックスに文書を追加
    index.add("c:/MyDocuments");
    
    // 特定の単語やフレーズを検索。例:
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 概要"
  description: "Java Javaライブラリによる強力なテキスト検索機能。"
  features:
    # feature loop
    - title: "Javaにおけるインデックス作成と検索操作"
      content: "GroupDocs.Search for Javaを使用してデータを集め、保存し、効率的に分析し、詳細なインデックスを作成し、より迅速で正確な検索を実現します。"

    # feature loop
    - title: "インデックスを統合して検索を最適化"
      content: "GroupDocs.Search for Javaを使用して、複数のインデックスを簡単に結合し検索を効率化します。小さなデルタインデックスの影響を減らすために、単一の高性能インデックスに統合します。"

    # feature loop
    - title: "多言語キーボードレイアウトのサポート"
      content: "GroupDocs.Search for Javaを使用して異なる言語とキーボードレイアウトにわたる検索を行います。88言語および164のキーボード構成に対応しています。"

    # feature loop
    - title: "形態素検索機能"
      content: " GroupDocs.Search for Javaを使用して、単数/複数名詞や動詞の変化などの異なる単語の形を見つけます。英語や他の言語向けに検索オプションをカスタマイズします。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Search for Javaは主要なオペレーティングシステムとパッケージマネージャーと互換性があります。"
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "サポートされるファイル形式"
  description: |
    GroupDocs.Search for Javaを使用してさまざまなファイル形式で作業します。[完全なリストを表示](https://docs.groupdocs.com/search/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### 一般的なオフィス形式
        * **ポータブル:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **テキスト:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### メディア形式
        * **一般的な画像形式:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **マルチページ画像:** GIF, WEBP, TIFF
        * **オーディオ:** MP3, WAV
        * **ビデオ:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### その他
        * **メール:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **ウェブ:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **その他:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Javaの機能"
  description: "PDF、DOCX、XLSX、PPTXなどの一般的な形式の高度な検索機能を使用して、ドキュメントコンテンツを効果的に管理します。"

  items:
    # feature loop
    - icon: "document_info"
      title: "カスタマイズ可能な検索パラメータ"
      content: "検索時に日付範囲や大文字小文字の区別を使用します。"

    # feature loop
    - icon: "detect"
      title: "拡張スペルチェック"
      content: "スペルチェック、ワイルドカード、および特別な文字を無視して効率的に検索します。"

    # feature loop
    - icon: "collect"
      title: "検索結果のフィルタリング"
      content: "検索結果を特定の文書タイプや基準に基づいて焦点を当てます。"

    # feature loop
    - icon: "get"
      title: "インデックスデータのインポートとエクスポート"
      content: "インデックスデータを簡単にインポートまたはエクスポートします。"

    # feature loop
    - icon: "remove"
      title: "不要なファイルをスキップ"
      content: "特定のファイルや単語を除外してインデックス作成を最適化します。"

    # feature loop
    - icon: "style"
      title: "HTMLおよびURL処理"
      content: "HTMLコンテンツをファイルに抽出し、検索結果をナビゲートするためのURLを生成します。"

    # feature loop
    - icon: "detect"
      title: "大規模インデックスの迅速検索"
      content: "大規模インデックスを扱いやすいチャンクに分割して、検索操作を迅速にします。"

    # feature loop
    - icon: "manipulate"
      title: "ストリームベースのインデックス作成"
      content: "ストリームやデータ構造から直接データをインデックス化します。"

    # feature loop
    - icon: "compare"
      title: "誤記があるクエリへの対応"
      content: "誤記を検出し、より良い検索精度のために代替の単語を提案します。"

    # feature loop
    - icon: "unreadable_characters"
      title: "包括的なアーカイブサポート"
      content: "ネストされたアーカイブをインデックス化し、ZIPファイル内のファイルの詳細リストを取得します。"

    # feature loop
    - icon: "hidden_print"
      title: "スペースを節約するインデックス作成"
      content: "コンパクトなインデックス作成でディスクスペースを節約し、パスワード保護されたファイルを処理します。"

    # feature loop
    - icon: "style"
      title: "カスタム同義語のサポート"
      content: "精度の向上を目指して同義語辞書を拡張します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "これらのコードサンプルを使用してGroupDocs.Search for Javaの機能を試してください。"
  items:
    # code sample loop
    - title: "ファジーマッチングで検索精度を向上させる"
      content: |
        GroupDocs.Search for Javaの柔軟性を活用して、コンテンツの管理を高度なファジー検索機能で強化します。[さらに詳しく](https://docs.groupdocs.com/search/java/search-results/)。
        {{< landing/code title="検索結果を処理する方法">}}
        ```java {style=abap}
        // インデックスを作成
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // 検索オプションを設定
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 'water'という単語または'Lorem ipsum'というフレーズを含むドキュメントを検索
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // 検索結果を処理
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "検索結果を正規表現で絞り込む"
      content: |
        GroupDocs.Search for Javaで正規表現を使用して、正確で詳細な検索結果を生成します。 [高度なテクニックを見つける](https://docs.groupdocs.com/search/java/regular-expression-search/)。
        {{< landing/code title="正規表現を使用して検索を行う方法">}}
        ```java {style=abap}   
        // インデックスを作成
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // テキスト形式でフレーズを検索

        // 最初のキャレット文字が先頭で、このクエリが正規表現検索であることを示します。
        String query = "^^(.)\\1{1,}";
        // 単語の先頭に同じ文字が2つ以上存在するか検索
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
