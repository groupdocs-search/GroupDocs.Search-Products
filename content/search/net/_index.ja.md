---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: ja
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: ".NET ドキュメント検索およびインデックス作成ライブラリ（PDF、Officeファイルなど）"
head_description: "PDF、Word、Excel、プレゼンテーション、メール、およびウェブフォーマットのドキュメントにおけるテキスト検索とインデックス作成のための強力な.NETソリューション。"

############################# Header ############################
title: ".NET APIによる高度なドキュメント検索およびインデックス作成"
description: ".NETアプリケーションのために、一般的なドキュメント形式にわたる最先端のテキスト検索機能を強化します。"
words:
  for: "のための"

actions:
  main: "無料でNugetをダウンロード"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "ライセンス管理"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "今日から旅を始めましょう！"
  description: "GroupDocs.Searchの機能を無料で探索するか、ライセンスを取得してその可能性を最大限に活かしてください。"

release:
  title: "バージョン {0} リリース"
  notes: "新着情報を確認する"
  downloads: "ダウンロード"

code:
  title: "ディレクトリファイル内のテキストを検索"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // ドキュメント用のインデックスを作成
    Index index = new Index("c:/MyIndex");

    // 効率的な検索のためにインデックスに文書を追加
    index.Add("c:/MyDocuments");
    
    // 特定の単語やフレーズを検索。例:
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 概要"
  description: ".NET C#ライブラリによる堅牢なテキスト検索とインデックス作成。"
  features:
    # feature loop
    - title: ".NETのインデックス作成および検索機能"
      content: "GroupDocs.Search for .NETを使用して、ドキュメントデータを効率的にインデックス作成、保存、処理し、高度に正確で迅速な検索操作を実現します。"

    # feature loop
    - title: "インデックスを結合して検索速度を向上させる"
      content: "GroupDocs.Search for .NETを使用して、複数のインデックスを統合してパフォーマンスを最適化できます。デルタインデックスの影響を減らすために、包括的なインデックスに結合し、スムーズな検索を実現します。"

    # feature loop
    - title: "異なるキーボードレイアウト間での検索"
      content: "GroupDocs.Search for .NETのインテリジェントな認識を使用して、88言語および164のキーボードレイアウトにわたる検索クエリを簡単に処理します。"

    # feature loop
    - title: "形態素検索"
      content: "GroupDocs.Search for .NETは単数/複数名詞や異なる動詞の形などの単語の変形を検索でき、さまざまな言語に合わせてカスタマイズできます。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Search for .NETは主要なオペレーティングシステムおよびパッケージマネージャーとシームレスに機能します。"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "サポートされるファイル形式"
  description: |
    GroupDocs.Search for .NETを使用して幅広いファイル形式を処理します。[すべてのサポートされている形式を表示](https://docs.groupdocs.com/search/net/supported-document-formats/)。
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
  title: "GroupDocs.Search for .NETの主な機能"
  description: "PDF、DOCX、XLSX、PPTXなどの一般的な形式の高度な検索機能で、ドキュメント管理を効率化します。"

  items:
    # feature loop
    - icon: "document_info"
      title: "柔軟な検索パラメータ"
      content: "日付範囲や大文字小文字の区別を使用して検索を絞り込みます。"

    # feature loop
    - icon: "detect"
      title: "スマートスペルチェック"
      content: "スペル修正、ワイルドカード、無視する特別な文字を使用してフレーズを検索します。"

    # feature loop
    - icon: "collect"
      title: "検索結果のフィルタリング"
      content: "文書の種類または基準によって検索結果をカスタマイズおよびフィルタリングします。"

    # feature loop
    - icon: "get"
      title: "インデックスのインポートとエクスポート"
      content: "データをインポートし、インデックス作成設定を変更し、インデックス化された結果をエクスポートします。"

    # feature loop
    - icon: "remove"
      title: "不必要なデータを除外"
      content: "特定のファイルまたは単語をスキップしてインデックス化を最適化します。"

    # feature loop
    - icon: "style"
      title: "URL抽出"
      content: "HTML形式のテキストをファイルに変換し、検索結果用のリンクを生成します。"

    # feature loop
    - icon: "detect"
      title: "高速検索"
      content: "大きなインデックスをより小さな部分に分割して、より迅速に処理します。"

    # feature loop
    - icon: "manipulate"
      title: "データ処理の効率化"
      content: "データストリームや構造から直接文書をインデックス化します。"

    # feature loop
    - icon: "compare"
      title: "誤記検出"
      content: "改善された精度のために代替単語を提案し、出現を追跡します。"

    # feature loop
    - icon: "unreadable_characters"
      title: "アーカイブのサポート"
      content: "ネストされたZIPアーカイブをインデックス化し、その中のファイルの詳細を取得します。"

    # feature loop
    - icon: "hidden_print"
      title: "効率的なインデックス作成"
      content: "コンパクトなインデックス作成でディスクスペースを節約し、パスワード保護された文書を処理します。"

    # feature loop
    - icon: "style"
      title: "カスタム同義語"
      content: "特定の検索結果に合わせて同義語を追加および管理します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "GroupDocs.Search for .NETの強力な機能をハンズオンの例とともに発見してください。"
  items:
    # code sample loop
    - title: "ファジー検索で生産性を向上させる"
      content: |
        GroupDocs.Search for .NETを使用して、高度な検索アルゴリズムを通じて柔軟で正確なコンテンツコントロールを実現します。[詳しい情報を探る](https://docs.groupdocs.com/search/net/search-results/)。
        {{< landing/code title="検索結果を処理する方法">}}
        ```csharp {style=abap}
        // インデックスを作成
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // 検索オプションを設定
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // 'water'という単語または'Lorem ipsum'というフレーズを含むドキュメントを検索
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // 検索結果を処理
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "正規表現による高度な検索"
      content: |
        GroupDocs.Search for .NETは正規表現をサポートしており、正確な検索が行えます。[高度なテクニックを学ぶ](https://docs.groupdocs.com/search/net/regular-expression-search/)。
        {{< landing/code title="正規表現を使用して検索を行う方法">}}
        ```csharp {style=abap}   
        // インデックスを作成
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // テキスト形式でフレーズを検索

        // 最初のキャレット文字が先頭で、このクエリが正規表現検索であることを示します。
        string query = "^^(.)\\1{1,}";
        // 単語の先頭に同じ文字が2つ以上存在するか検索
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
