---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/net/case-sensitive/xla/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: ".NETを介してXLAドキュメントで大文字と小文字を区別するテキスト検索を適用する"
head_description: "GroupDocs.Search .NET APIを使用すると、ソフトウェアプログラマーは大文字と小文字を区別するテキスト検索を適用し、.NETAPIを介してXLAドキュメント内の単語の正確なシーケンスを見つけることができます。"

############################# Header ############################
title: ".NETアプリ内のXLAドキュメントで大文字と小文字を区別する検索を適用するにはどうすればよいですか？"
description: "GroupDocs.Search .NET APIを使用すると、ソフトウェア開発者は、.NET Apps内のPDF、HTML、DOCX、PPTX、XLSXなどのさまざまなドキュメントタイプで大文字と小文字を区別するテキスト検索を適用できます。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "大文字と小文字を区別する検索とは何ですか .NETを介して検索を実行する方法は？"
    content: |
     ユーザーがさまざまな種類のドキュメントを検索して、単語やその他のデータの特定の組み合わせを探すのに役立つ、便利な検索手法が数多くあります。大文字と小文字を区別する検索は、大文字と小文字が異なるか等しいかどうかに関係なく、ユーザーがドキュメントとWebページを検索できるようにする非常に便利な手法です。たとえば、「Computer」、「computer」、「COMPUTER」は、最初は大文字、2番目は小文字、3番目はすべて大文字であるため、異なる単語として扱われます。 GroupDocs.Search for .NETは、ソフトウェア作成者がテキスト検索やドキュメントのインデックス作成を簡単に実行するためのソフトウェアアプリケーションとツールを作成できるようにする便利な高性能ドキュメント検索APIです。 APIは、PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシート、PowerPointプレゼンテーション、Outlook MSG、PSTなどの最も一般的に使用されるファイル形式のサポートを提供します。もう1つの便利な機能は、キーボードレイアウトと一致しない言語で書かれた検索クエリを識別できることです。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NETを介してXLAドキュメントで大文字と小文字を区別する検索を実行する"
      content_left: |
       GroupDocs.Search .NET APIを使用すると、ソフトウェアプログラマーは、大文字と小文字を区別する検索機能を独自のC＃.NETアプリケーション内に追加できます。 次の.NETコード例は、わずか数行のコードでXLAファイルのテキスト形式のクエリで大文字と小文字を区別する検索を実現する方法を示しています。

      title_right: "XLAドキュメントで大文字と小文字を区別する検索を適用する"
      content_right: |
         * インデックスフォルダとドキュメントフォルダへのパスを特定します。
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを生成します
         * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) クラスのインスタンスを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
         * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) クラスの新しいインスタンスを初期化します
         * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) メソッドを呼び出して、大文字と小文字を区別するsearchbを有効にする
         * 検索文字列を定義し、検索を開始します
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: ".NETを介してオブジェクト形式で大文字と小文字を区別する検索を実行する"
      content_left: |
        GroupDocs.Search .NETを使用すると、ソフトウェア開発者は、.NETアプリケーション内の大文字と小文字を念頭に置いて単語を見つけることができます。 次の.NETコード例は、XLAドキュメントのオブジェクト形式のクエリで大文字と小文字を区別する検索を適用する方法を示しています。

      title_right: "XLAドキュメントで大文字と小文字を区別する検索を行う"
      content_right: |
        * インデックスフォルダとドキュメントフォルダへのパスを特定します。
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを生成します
        * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) クラスのインスタンスを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
        * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) クラスの新しいインスタンスを初期化します
        * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) メソッドを呼び出して、大文字と小文字を区別するsearchbを有効にする
        * [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)メソッドを呼び出して、オブジェクト形式で検索クエリを作成する
        * 検索を開始し、検索結果を表示します
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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