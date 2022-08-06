---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/java/case-sensitive/one/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "ONE ドキュメントで大文字と小文字を区別するテキスト検索を実行する Java API"
head_description: "GroupDocs.Search Java API を使用すると、プログラマは大文字と小文字を区別してテキスト検索を実行し、Java を介して ONE ドキュメント内の単語の正確な構造を発見できます。"

############################# Header ############################
title: "Java アプリで ONE ドキュメントを介して大文字と小文字を区別して検索を実行する"
description: "GroupDocs.Search Java API を使用すると、ソフトウェア開発者は Java アプリで PDF、HTML、DOCX、PPTX、XLSX などのさまざまなドキュメント タイプに対して大文字と小文字を区別するテキスト検索を適用できます。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java アプリで大文字と小文字を区別する検索を実行する方法は?"
    content: |
      大文字と小文字の区別は、Web、データベース、またはドキュメントの検索で大文字 (大文字) と小文字 (小文字) を区別するプログラムの機能を表す非常に便利な検索手法です。デフォルトでは、検索エンジンは大文字と小文字を区別しないことに注意してください。つまり、Computer という単語を検索すると、キー名を持つフラグメントまたは Computer と computer という単語を持つテキストの両方が返されます。検索結果を大文字の「Computer」を含むものに絞り込む必要があるとします。これは、大文字と小文字を区別して検索する必要があることを意味します。 GroupDocs.Search for Java は、ソフトウェア開発者が PDF、HTML、Outlook 電子メール、Microsoft Office Word、Excel ワークシートなどの最も一般的なドキュメント タイプのテキスト検索およびインデックス作成を実行できるアプリケーションを開発できるようにする、効果的なドキュメント検索およびインデックス作成 API です。 PowerPoint プレゼンテーション、Outlook MSG、PST など。さらに、キーボード レイアウトと一致しない言語で書かれた検索クエリを識別できます。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java による ONE ドキュメントの大文字と小文字を区別した検索"
      content_left: |
       GroupDocs.Search Java API には、基本的な検索機能と高度な検索機能の完全なサポートが組み込まれており、ソフトウェア開発者は Java アプリケーション内で数行のコードだけで大文字と小文字を区別した検索を行うことができます。
       
       次の Java コード例は、ONE ファイル内のテキスト内のクエリを使用して、数行のコードで大文字と小文字を区別する検索を実行する方法を示しています。

      title_right: "ONE ファイルで大文字と小文字を区別して検索を実行する"
      content_right: |
         * インデックス フォルダーとドキュメント フォルダーへのパスを特定します。
         * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) クラスのインスタンスを呼び出して、指定したフォルダにインデックスを作成する
         * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) クラスのインスタンスを呼び出して、指定したフォルダーからドキュメントのインデックスを作成する
         * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) クラスの新しいインスタンスを開始する
         * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) メソッドを呼び出して、大文字と小文字を区別する検索オプションを有効にします。
         * 検索クエリを定義して検索を開始
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Java を介してオブジェクト形式で大文字と小文字を区別する検索を行う"
      content_left: |
        GroupDocs.Search Java を使用すると、ソフトウェア開発者は、独自のアプリケーション内にさまざまなドキュメント形式の検索機能を組み込むことができます。 次の Java コード例は、ONE ドキュメントを介してオブジェクト形式のクエリで大文字と小文字を区別する検索を実行する方法を示しています。 

      title_right: "ONE ドキュメントで大文字と小文字を区別する検索を適用する"
      content_right: |
        * インデックス フォルダーとドキュメント フォルダーへのパスを特定します。
        * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) クラスのインスタンスを呼び出して、指定したフォルダにインデックスを作成する
        * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) クラスのインスタンスを呼び出して、指定したフォルダーからドキュメントのインデックスを作成する
        * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) クラスの新しいインスタンスを開始する
        * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) メソッドを呼び出して、大文字と小文字を区別する検索オプションを有効にします。
        * [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) メソッドを呼び出してオブジェクトに検索クエリを作成する
        * 検索クエリを定義して検索を開始
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

    - title_left: "システム要求"
      content_left: |
        GroupDocs.Search for Javaは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 完全なシステム要件ガイドについては、以下のコードを実行する前に[システム要件](https://docs.groupdocs.com/search/java/system-requirements/) にアクセスしてください。次の前提条件がインストールされていることを確認してください。 システム：
          *オペレーティングシステム：Microsoft Windows、Linux、MacOS
          * Javaバージョンのサポート：J2SE 7.0（1.7）、J2SE 8.0（1.8）以降
          * GroupDocsの最新バージョンを入手します。GroupDocs[リポジトリ](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/) からJavaAPIを検索します。
        
      title_right: "GroupDocs.Searchを使用する理由"
      content_right: |
        * メモリ内およびディスク上での検索インデックスの作成。
        * ファイル、ストリーム、または構造からインデックスを作成する機能。
        * パスワードで保護されたドキュメントのインデックス作成のサポート。
        * 複数のインデックスのマージのサポート。
        * 検索のインデックス作成中にドキュメントをフィルタリングします。
        * 検索中のスペルチェックのサポート。
        * ブレンドされた文字は完全にサポートされています
        * さまざまな種類の検索を1つの検索クエリに結合します。
        * 単純な単語と正規表現の検索のサポート
        * 検索クエリでのエイリアス置換を完全にサポートします。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---