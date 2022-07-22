---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/net/phrase /xhtml/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP  MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: ".NETアプリの XHTMLドキュメントにフレーズ検索を追加するにはどうすればよいですか？"
head_description: "GroupDocs.Search .NET APIを使用すると、ソフトウェアの専門家はフレーズ検索を追加して、.NETAPIを介してXHTMLドキュメント内の正確なフレーズまたは提供された単語のシーケンスを見つけることができます。"

############################# Header ############################
title: ".NETアプリ内のXHTMLドキュメントに正確な文またはフレーズ検索を追加しますか？"
description: "GroupDocs.Search .NET APIを使用すると、プログラマーは、.NET Apps内のフレーズ検索または正確な文検索を介して、XHTMLドキュメントで提供されている単語のシーケンスを見つけることができます。 "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NETアプリで正確な文またはフレーズ検索を使用する方法は？"
    content: |
       正確な文またはフレーズ検索は、ユーザーが特定の順序と消費者によって定義された単語の組み合わせを含む正確な文またはフレーズを持つドキュメント、Web、またはデータベースを検索できるようにする一種の検索です。 これは検索エンジンの用語で非常に一般的な用語であり、ユーザーはインデックス付きドキュメントのテキスト内の指定された単語のシーケンスでドキュメントを検索できます。 GroupDocs.Search for .NETは、非常に便利な高性能ドキュメントおよびテキスト検索APIであり、PDF、HTML、Outlook電子メール、Microsoft Office Word、 Excelワークシート、PowerPointプレゼンテーション、Outlook MSG、PSTなど。 テキストやオブジェクト形式でのクエリの検索、フレーズ検索でのワイルドカードの使用など、フレーズ検索に関連するいくつかの機能のサポートが含まれています。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NETを介してXHTMLドキュメントでフレーズ検索を実行する方法"
      content_left: |
       GroupDocs.Search .NET APIを使用すると、ソフトウェア開発者は独自のC＃.NETアプリケーション内にフレーズ検索機能を追加できます。 次の.NETコード例は、わずか数行のコードでテキストとオブジェクトのフレーズ検索を実行する方法を示しています。

      title_right: "XHTMLドキュメントでの正確なフレーズ検索"
      content_right: |
         * まず、インデックスフォルダとドキュメントフォルダへのパスを指定する必要があります。
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
         * [検索](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
         * テキスト形式でフレーズクエリ「フレーズテキスト」を検索します
         * オブジェクト形式で「フレーズテキスト」というフレーズを検索します
         * [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) メソッドを呼び出してword1、word2を作成し、サブクエリ3を作成する
         * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)メソッドを呼び出して、サブクエリを組み合わせて新しい検索クエリを作成します
         *検索を開始し、検索結果を表示します
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: ".NETを介したXHTMLドキュメントでのワイルドカードフレーズ検索"
      content_left: |
        GroupDocs.Search for .NETを使用すると、ソフトウェアプログラマーは、C＃.NETアプリケーション内でワイルドカードを使用してフレーズ検索機能を追加できます。 次の.NETコード例は、C＃アプリケーション内のXHTMLドキュメントでワイルドカードフレーズ検索を適用する方法を示しています。

      title_right: "XHTMLファイルでワイルドカードフレーズ検索を適用する"
      content_right: |
        * まず、インデックスフォルダとドキュメントフォルダへのパスを指定する必要があります。
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
        * [検索](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
        * テキスト形式でフレーズクエリ「フレーズテキスト」を検索します
        * オブジェクト形式で「フレーズテキスト」というフレーズを検索します
        * [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) メソッドを呼び出してword1を作成し、サブクエリ3を作成する
        * [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) メソッドを呼び出してwildcard2を作成する
        * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) メソッドを呼び出して、サブクエリを組み合わせて新しい検索クエリを作成します
         *検索を開始し、検索結果を表示します
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: ".NET を介してフレーズ検索を他のタイプの検索と組み合わせる"
      content_left: |
        GroupDocs.Search .NETを使用すると、ソフトウェアプログラマーは、フレーズ検索を.NETアプリケーション内の他のタイプの検索と組み合わせることができます。 次の.NETコード例は、単語を表すワイルドカードと単語内の文字の両方を適用する方法を示しています。

      title_right: "フレーズ検索を他の検索と組み合わせるための.NETAPI"
      content_right: |
        * まず、インデックスフォルダとドキュメントフォルダへのパスを指定する必要があります。
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) クラスのインスタンスを呼び出して、指定されたフォルダーにインデックスを作成します
        * [検索](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
        *テキスト形式でフレーズを検索します
        *オブジェクト形式でフレーズを検索します
        *単語パターンを定義し、文字列を追加します。
        * [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery) メソッドを呼び出してwordPattern1とword3を作成する
        * [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) メソッドを呼び出してwildcard2を作成する
        * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) メソッドを呼び出して、サブクエリを組み合わせて新しい検索クエリを作成します
        *検索を開始し、検索結果を表示します
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

    - title_left: "システム要求"
      content_left: |
        GroupDocs.Search for .NETは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 完全なシステム要件ガイドについては、以下のコードを実行する前に[システム要件](https://docs.groupdocs.com/search/net/system-requirements/) にアクセスしてください。次の前提条件がインストールされていることを確認してください。 システム：
          *オペレーティングシステム：Microsoft Windows、Linux、MacOS
          *開発環境：Visual Studio、Xamarin、MonoDevelopなど
          *フレームワーク：.NETフレームワーク、.NET標準、.NETコア、モノラル
          * [NuGet](https://www.nuget.org/packages/GroupDocs.search/) から最新バージョンのGroupDocs.Search for.NETAPIを入手してください。
        
      title_right: "GroupDocs.Search を使用する理由"
      content_right: |
        * メモリ内およびディスク上での検索インデックスの作成。
        * ファイル、ストリーム、または構造からインデックスを作成する機能。
        * パスワードで保護されたドキュメントのインデックス作成のサポート。
        * 複数のインデックスのマージのサポート。
        * 検索のインデックス作成中にドキュメントをフィルタリングします。
        * 検索中のスペルチェックのサポート。
        * ブレンドされた文字は完全にサポートされています
        * さまざまな種類の検索を1つの検索クエリに結合します。
        * 単純な単語と正規表現の検索がサポートされています
        * 検索クエリでのエイリアス置換を完全にサポートします。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---