---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

head_title: "ドキュメント、PDF、Office、Web用のJavaテキスト検索およびインデックス作成API"
head_description: "ドキュメントからデータを検索、インデックス作成、取得するためのJavaアプリケーション用の高度なテキスト検索API：PDF、Word、Excel、プレゼンテーション、電子メール、およびWebファイル形式."

title: "JavaAPIを介したドキュメントの検索とインデックス作成"
description: "すべての一般的なドキュメント形式でテキスト検索操作を実行するJavaアプリケーションを構築する."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-java.png"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            - link: "#overview"
              text: "概要"

            - link: "#features"
              text: "特徴"

            - link: "#support"
              text: "サポート"

            - link: "https://products.groupdocs.app/search"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Search for Javaを使用すると、エンドユーザーがこれまでにない検索操作を実行できるビジネスアプリケーションを作成できます。当社のJavaAPIを使用すると、ユーザーは基本レベルから高度なレベルのテキスト検索機能を操作できます。複数のインデックスを作成してマージします。 Simple、Boolean、Regular Expression（Regex）、Fuzzy、およびその他のタイプのクエリを使用して、インデックスを迅速かつスマートに検索します。 GroupDocs.Search for Javaはすべての一般的なファイル形式をサポートしているため、ファイル、ドキュメント、電子メール、アーカイブから必要な情報を取得できます。
    tabs:
      enable: true     
      
      tab_one:
        description: |
          以下は、GroupDocs.SearchforJavaの概要です。

        left:
          enable: true
          icon: "fas fa-search"
          title: "インデックス作成"
          content: |
            *作成および管理
            *複数のインデックスをマージする
            *マルチスレッド非同期インデックス
            *コンパクトなインデックス作成
            *アーカイブファイルのインデックス作成
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "高度な検索と検索クエリ"
          content: |
            *あいまい検索
            *同義語検索
            *メール検索
            *ホモフォニック用語の処理
            *保護されたファイルの検索
            * 単純
            *ワイルドカード
            *正規表現（Regex）
            *ファセットとブール
            * 大文字と小文字を区別
      
      tab_two:
        description: |
          GroupDocs.Search for Javaは、Microsoft Office、画像、図など、一般的な[ドキュメントファイル形式]（https://docs.groupdocs.com/search/java/supported-document-formats/）をすべてサポートしています。

        left:
          enable: true
          table:
            - title: "MicrosoftOfficeの形式"
              content: |
                * ** Word **：DOC、DOCX、DOCM、DOT、DOTX、DOTM
                * ** Excel **：XLS、XLSX、XLSM、XLT、XLTX、XLTM、XLSB、XLA、XLAM、CSV、TSV
                * ** PowerPoint **：PPT、PPTX、POT、POTX、PPS、PPSX、PPTM、PPSM、POTM
                * **プロジェクト**：MPP
                * **図**：VSD、VSS
                * ** Microsoft Compiled HTML **：CHM
                * ** OneNote **：ONE

        right:
          enable: true
          table:
            - title: "OpenDocumentおよびその他の形式"
              content: |
                * **ポータブルドキュメントフォーマット**：PDF
                * ** OpenDocument **：ODT、OTT、ODS、OTS、ODP
                * **メール**：PST、OST、MSG、EML、EMLX
                * ** Webファイル形式**：XML、HTM、HTML、XHTML、MHT、MHTML
                * **オーディオ**：MP3、WAV
                * **ビデオ**：AVI、MOV、QT、FLV、ASF
                * **テキスト**：TXT
                * **リッチテキスト形式**：RTF
                * ** Markdownドキュメントファイル**：MD
                * **画像**：BMP、GIF、JP2、PNG、WEBP、TIFF、EMF、WMF、JPG、PSD
                * **その他**：TORRENT、ZIP、DCM、DJVU、EPUB、FB2

      tab_three:
        description: |
          GroupDocs.Search for Javaは、次のオペレーティングシステム、フレームワーク、パッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *MicrosoftWindowsデスクトップ
                * Microsoft Windows Server
                * Linux
                * マックOS

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * Java 7（1.7）以降

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "開発環境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                *Eclipse
            - icon: "fas fa-tools"
              title: "ビルド自動化ツール"
              content: |
                * Maven

features:
    enable: true
    title: "GroupDocs.Search for Java Features"

    feature:
      - icon: "fas fa-copy"
        content: "非同期マルチスレッドを使用して、ディスク上またはメモリ内にインデックスを構築する"

      - icon: "fas fa-eye"
        content: "インデックスの作成と更新の進捗状況を表示"

      - icon: "fas fa-bolt"
        content: "特定のファイルのインデックスを選択的にスキップし、特定の単語をスキップしてより速くインデックスを作成する"
      
      - icon: "fas fa-file-powerpoint"
        content: "インポートまたはリストの使用を実行して、インデックス作成およびファイルへのエクスポート中に文字を変更します"

      - icon: "fas fa-code"
        content: "エラーインデックスの場合にインデックスをリロードし、矛盾した設定についてユーザーに警告する"

      - icon: "fas fa-cloud"
        content: "最新の処理済みファイルに関するインデックスステータス通知"

      - icon: "fas fa-remove-format"
        content: "他のZIPアーカイブ内のZipアーカイブにインデックスを付け、アーカイブ内のインデックスファイルのリストを取得する"

      - icon: "fas fa-comment-slash"
        content: "コンパクトなインデックス作成とパスワードで保護されたドキュメントのインデックス作成によりスペースを節約"

      - icon: "fas fa-location-arrow"
        content: "インデックスまたはソースファイルからのドキュメントテキストの抽出"

      - icon: "fas fa-border-all"
        content: "HTML形式のテキストをファイルに抽出してURLを生成し、HTMLで検索結果をナビゲートします"

      - icon: "fas fa-wrench"
        content: "インデックス作成中に各ドキュメントに任意の追加フィールドを追加する"

      - icon: "fas fa-columns"
        content: "あいまい検索の類似性レベルを構成し、最良の結果を表示する"

      - icon: "fas fa-file-word"
        content: "あいまい検索によるタイプミスのスマート管理"

      - icon: "fas fa-envelope"
        content: "ファセット検索とブール検索を同時に使用する"

      - icon: "fas fa-print"
        content: "同義語の構成と実行検索とホモフォニック用語のスマートな処理"

      - icon: "fas fa-file-archive"
        content: "検索パラメータとして日付範囲と大文字と小文字の区別を使用する"

      - icon: "fas fa-lock"
        content: "Aspose.EmailAPIを介して電子メールメッセージを検索および参照するためのインデックスを作成する"

      - icon: "fas fa-file-code"
        content: "スペルチェックとワイルドカードで検索フレーズを使用し、クエリで特殊文字をスキップします"
      
      - icon: "fas fa-fill-drip"
        content: "複数のクエリを組み合わせて単一のオブジェクトツリーを作成する"

      - icon: "fas fa-file-excel"
        content: "小さなチャンクで検索を分割して、巨大なインデックスを迅速に検索する"

      - icon: "fas fa-heading"
        content: "ストリームとデータ構造からのインデックスドキュメント"

      - icon: "fas fa-project-diagram"
        content: "検索結果でドキュメントフィルタリングを設定する"

      - icon: "fas fa-cube"
        content: "英語の類義語をデフォルトの類義語辞書に追加する"

      - icon: "fab fa-uncharted"
        content: "見つかった単語ごとに正確な出現回数を有効にして、スペルミスの場合に代替単語の提案を提供します"

      - icon: "fab fa-uncharted"
        content: "インデックスを再作成せずに、インデックス付きドキュメントにテキスト属性を追加する"

      - icon: "fab fa-uncharted"
        content: "文字に基づいて索引付けおよび検索操作を実行する"

      - icon: "fab fa-uncharted"
        content: "非テキストドキュメント形式のインデックスメタデータ"

    more_feature:
      - title: "インデックス作成と検索操作"
        content: |
          インデックス付けは、GroupDocs.Search for Javaによって使用され、データを収集し、正確で効率的な検索操作のためにデータを保存および解析します。 GroupDocs.Search for Javaは、検索を実行するためにこのようなインデックスを頻繁に使用します。

          * **インデックスの作成**：インデックスフォルダを作成し、そのフォルダにドキュメントを追加/インデックス付けします。
          * **ロードインデックス**：既存のインデックスをロードします。
          * **ドキュメントをインデックスに追加**：ドキュメントを既存のインデックスに非同期で追加します。
          * **インデックスの更新**：ドキュメントが変更、追加、または削除されるたびに、既存のインデックスを更新します。これにより、検索結果が最新の状態に保たれます。
          
          ```java
          / Creating index
          Index index = new Index("c:\\MyIndex");
          //ドキュメントをインデックスに追加します
          index.addToIndex("c:\\MyDocuments");
          //「principal」、「principle」、「principles」、または「principally」を含むドキュメントで「affect」または「effect」という単語を検索する
          SearchResults results = index.search("?ffect & princip?(2~4)");
          ```
      - title: "複数のインデックスをマージして検索効率を向上させる"
        content: "GroupDocs.Search for Java APIは、複数のインデックスを共通のインデックスにマージする機能を提供します。頻繁に変更されるインデックスの場合、いくつかのデルタインデックスが作成されます。ただし、このアプローチでは検索パフォーマンスが低下します。 GroupDocs.Search for Javaは、さまざまなデルタインデックスをマージして、1つの共通インデックスを作成することにより、このボトルネックを克服します。この共通のマージされたインデックスには、マージされたデルタインデックスのすべての情報が含まれています。このアプローチは、検索効率を大幅に向上させながら、デルタインデックスを変更せずに維持します。このプロセスをさらに微調整するために、さまざまな機能を構成できます."

      - title: "さまざまなキーボードレイアウトの検索クエリを認識する"
        content: "GroupDocs.Search for Javaは、キーボードレイアウトと一致しない検索クエリを認識します。現在、88の言語と164の異なるキーボードレイアウトがGroupDocs.SearchforJavaによって正常に認識されています。"

      - title: "形態論的単語形式を使用した検索"
        content: "GroupDocs.Search for Javaを使用すると、さまざまな単語形式を自由に検索できます。特定の名詞の単数形と複数形を検索できます。または、動詞のすべての形式を検索することを選択できます。ルート、三人称単数形、単純過去形、その他のさまざまな形も検索できます。英語以外の言語の場合、カスタマイズされた単語フォームを構成できます."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Searchは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Search for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-net.png"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

        # solution loop
        - img_alt: "GroupDocs.Search for Node.js"
          image: "/border/groupdocs-search-nodejs-java.svg"
          product: "GroupDocs.Search"
          platform: "Node.js via Java"
          link: "/search/nodejs-java/"

back_to_top:
  enable: true
---
