---
############################# Static ############################
layout: "family"
date:  2025-01-09T15:38:59
draft: false

product: "Search"
product_tag: "search"

lang: ja

############################# Head ############################
head_title: "ドキュメントテキスト検索とインデックス作成 | APIおよび無料Webアプリ"
head_description: "当社のAPIまたは無料のオンラインドキュメント検索アプリを使用して、PDF、MS Office、OpenDocument、その他の一般的なファイル形式で効率的なテキスト検索とデータインデックス作成を実行します。"

############################# Header ############################
title: "包括的なドキュメント検索とインデックス作成ソリューション"
description:  |
  PDF、Microsoft Office、OpenOffice、およびその他の多くのドキュメントファイル形式でテキスト検索とインデックス作成を実行します。

  高度なフルテキスト検索機能を使用して、大規模なドキュメントコレクション内の情報を迅速に特定します。

  精度と結果を高めるために、同義語、ファジー検索、そしてステミングなどの検索機能をカスタマイズします。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "プラットフォームを選択"
  title: "プラットフォームの独立性"
  description: "GroupDocs.Searchは次のオペレーティングシステムとフレームワークと互換性があります："
  details_link_title: "詳細を学ぶ"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 他のテキストエディタ
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Searchの主な機能"
  description: "GroupDocs.Searchは一般的なドキュメント形式でのテキストインデックス作成と検索のための強力なツールを提供します。高度な検索機能を使ってドキュメント管理をシンプルかつ強化します。"

  items:
    # items loop
    - icon: "view"
      title: "高度なテキスト検索"
      content: "インデックス化されたドキュメント内で迅速かつ正確なテキスト検索を実行します。"

    # items loop
    - icon: "manipulate"
      title: "カスタマイズ可能な検索オプション"
      content: "ファジー検索、同義語、ステミングなどの機能を利用して、より正確な結果を得ることができます。"

    # items loop
    - icon: "merge"
      title: "複数の形式のサポート"
      content: "Microsoft Office、PDF、OpenOffice、その他の一般的な形式のコンテンツをインデックス化および検索します。"

    # items loop
    - icon: "additional"
      title: "効率的なインデックス作成"
      content: "大規模なドキュメントコレクションのために迅速にインデックスを構築し、維持します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "一般的なドキュメント形式でのテキスト検索"
  description: "GroupDocs.Searchのコード例"
  items:
    # code sample loop
    - title: "テキスト検索"
      content: |
       GroupDocs.Searchはドキュメント内のテキストを見つけるための強力なツールです。特定のフォルダーに格納されたさまざまな形式の複数のドキュメントを検索できます。検索結果は別のフォルダーに保存され、再度検索を実行することなくアクセスして再利用できます。
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // インデックスを保存するフォルダーを指定して、Indexクラスのインスタンスを作成します。
            Index index = new Index("\\Index Folder");

            //検索が実行されるドキュメントへのパスを指定します。
            index.Add("\\Documents Folder");

            //SearchOptionsオブジェクトのインスタンスを作成します。
            SearchOptions options = new SearchOptions();

            //目的のテキストに対して検索を実行します。
            SearchResult result = index.Search("ipsum dolor", options);

            //検索結果を処理および操作します。
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // インデックスを保存するフォルダーを指定して、Indexクラスのインスタンスを作成します。
            Index index = new Index("\\Index Folder");

            //検索が実行されるドキュメントへのパスを指定します。
            index.add("\\Documents Folder");

            //SearchOptionsオブジェクトのインスタンスを作成します。
            SearchOptions options = new SearchOptions();

            //目的のテキストに対して検索を実行します。
            SearchResult result = index.search("ipsum dolor", options);

            //検索結果を処理および操作します。
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // インデックスを保存するフォルダーを指定して、Indexクラスのインスタンスを作成します。
            const index = new searchLib.Index('\\Index Folder');

            //検索が実行されるドキュメントへのパスを指定します。
            index.add('\\Documents Folder');

            //SearchOptionsオブジェクトのインスタンスを作成します。
            const options = new searchLib.SearchOptions();

            //目的のテキストに対して検索を実行します。
            const result = index.search('ipsum dolor', options);

            //検索結果を処理および操作します。
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "70以上のファイル形式に対応"
  description: "GroupDocs.Searchは、一般的に使用されるほぼすべてのファイル形式をサポートします。"

############################# Metrics ###############################
metrics:
  enable: true
  title: "私たちの製品の統計"
  description: "私たちのパフォーマンス、到達範囲、および成長を示す主要な指標を発見してください。"

  items:
    # items loop
    - number: "70+"
      title: "サポートされる形式"
      content: "70以上の一般的なドキュメント形式との互換性を提供します。"

    # items loop
    - number: "500k"
      title: "NuGetダウンロード"
      content: "GroupDocs.Search for .NETは、NuGetから500,000回以上ダウンロードされました。"

    # items loop
    - number: "12k"
      title: "Mavenダウンロード"
      content: "Java開発者は、MavenからGroupDocs.Searchを12,000回以上ダウンロードしています。"

    # items loop
    - number: "150+"
      title: "満足している顧客"
      content: "世界中の開発者と著名な企業が革新的なソリューションのために我々の製品を信頼しています。"


############################# Customers ###############################
customers:
  enable: true
  title: "私たちの満足している顧客"
  description: "GroupDocsライブラリは、世界中の著名なブランドや組織から信頼されています。"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "今日から旅を始めましょう！"
  description: "お好みのプラットフォームでGroupDocs.Searchを無料で体験してください。"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "よくある質問"
  description: "GroupDocs.Searchに関する一般的な質問への回答を見つけてください。"

  items:
    # items loop
    - question: "GroupDocs.Searchはドキュメント検索のために外部ツールが必要ですか？"
      answer: "いいえ、GroupDocs.Searchはスタンドアロンソリューションとして機能し、検索を実行するためにAdobe AcrobatやMicrosoft Officeなどの追加ツールやソフトウェアは必要ありません。"

    # items loop
    - question: "GroupDocs.Searchを購入前に試すことはできますか？"
      answer: "はい、できます！ GroupDocs.Searchは無料トライアルを提供しています。機能を探索できますが、試用版には透かしや制限された機能が含まれる場合があります。すべての機能を解除するには、無料の30日間の一時ライセンスをリクエストできます。 [一時ライセンス](https://purchase.groupdocs.com/temporary-license/)ページで詳細を確認してください。"

    # items loop
    - question: "どのようなライセンスオプションがありますか？"
      answer: "GroupDocs.Searchにはさまざまなニーズに応じた複数のライセンスモデルが用意されています。チームサイズ、利用シナリオ、またはクライアントへの配布にSDK/APIが必要かどうかに基づいてライセンスを選択します。柔軟な利用のためには、実際の利用に基づいて支払うメーターライセンスを考慮してください。 [料金](https://purchase.groupdocs.com/pricing/search/net/)ページでオプションの詳細を確認してください。"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Webアプリ"
  description: "私たちの無料Webアプリケーションを使用してGroupDocs.Searchを探索してください。ブラウザから直接70以上の一般的なファイル形式でテキスト検索とインデックス作成を行えます—完全に無料で。"

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "PDF、Excel、Word、PowerPoint、その他のファイルタイプをWebブラウザから直接検索します。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "DOCXをアップロードし、ソフトウェアをインストールすることなく、高度なテキスト検索を実行します。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "さまざまな形式でのPDFのインデックス作成と取得機能を無料でテストします。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---