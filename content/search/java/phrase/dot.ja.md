---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/java/phrase/dot/"
otherformats: PDF DOC DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: "{{$ 5}}_UPPERドキュメントで正確なフレーズを検索および検索するJavaAPI"
head_description: "GroupDocs.Search Java APIは、プログラマーがフレーズ検索を埋め込んで、Javaを介して{{$ 5}}_UPPERドキュメントのテキスト内の特定の単語シーケンスまたは正確なフレーズを検出するのに役立ちます。"

############################# Header ############################
title: "JavaAPIを介してdot_ UPPERドキュメント内の正確な文またはフレーズを検索および表示する方法は？"
description: "GroupDocs.Search Java APIは、ソフトウェア開発者がフレーズ検索または正確な文検索を介して{{$ 5}}_UPPERドキュメント内の正確な文またはフレーズを検索できるようにする高度な検索機能を完全にサポートしています。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "フレーズ検索とは何ですか？Javaアプリでそれを使用する方法は？"
    content: |
       フレーズ検索は、キーワードではなく、正確な文やフレーズをドキュメントやWebページ内で検索する非常に効果的な方法です。これは、ユーザーが正確なフレーズを検索するときに、表示された特定の順序ですべての検索用語を検索したいことを意味します。このWebページでは、ユーザーがJavaAPIを使用して効率的なドキュメントとWebページを検索するためのビジネスアプリケーションとツールを開発する方法に関する情報を共有します。 GroupDocs.Search for Javaは、非常によく構成された効率的なJava APIであり、ソフトウェア開発者は、サードパーティのソフトウェアをインストールせずに、独自のアプリ内で基本レベルから高度なレベルのテキスト検索操作を操作できます。 APIには、単純検索またはブール検索、ファジー、大文字と小文字を区別する検索、同義語、同音異義語、ワイルドカード、オブジェクトタイプ検索、データ範囲の設定、その他のタイプのクエリなど、ドキュメント検索に関連する多数の貴重な機能が含まれており、情報をすばやくエレガントに検索できます。さらに、キーボードレイアウトと一致しない言語で書かれた検索クエリの認識もサポートします。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Javaを介してDOTドキュメントでフレーズ検索を行う"
      content_left: |
       GroupDocs.Search Java APIには、ソフトウェアの専門家が検索機能と使いやすさを備えた強力なソフトウェアアプリケーションを作成できるようにする、高度な検索の完全なサポートが含まれています。 以下のJavaコードは、わずか数行のコードでテキストおよびオブジェクト形式でフレーズ検索を実行する方法を示しています。

      title_right: "DOTファイルでの正確な文の検索"
      content_right: |
         * インデックスフォルダとドキュメントフォルダへのパスを定義します。
         * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
         * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
         * [検索](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) メソッドを呼び出してテキストクエリで検索する
         *オブジェクト形式でフレーズ「フレーズテキスト」を検索します
         * [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) メソッドを呼び出してword1、word2を作成し、サブクエリ3を作成する
         * [CreatePhraseSearchQuery](https：//apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery（com.groupdocs.search.SearchQuery...)) を呼び出して、サブクエリを組み合わせて新しい検索クエリを作成します。方法
         *検索を開始し、検索結果を表示します
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "Javaを介してDOTファイルを介してワイルドカードフレーズ検索を適用する"
      content_left: |
        GroupDocs.Search for Javaを使用すると、ソフトウェアプログラマーは、Javaアプリケーション内の{{$ 5}}_UPPERファイルを検索するときにワイルドカードフレーズ検索機能を追加できます。 次のJavaコード例は、JavaAPIを使用してさまざまなドキュメントタイプでワイルドカードフレーズ検索を適用する方法を示しています。

      title_right: "Javaでワイルドカードを使用したフレーズ検索"
      content_right: |
        * インデックスフォルダとドキュメントフォルダへのパスを定義します。
        * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
        * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
        * [検索](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) メソッドを呼び出してテキストクエリで検索する
        * オブジェクト形式でフレーズ「フレーズテキスト」を検索します
        * [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) メソッドを呼び出してword1とword3を作成する
        * [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) メソッドを呼び出してwildcard2を作成する
        * [CreatePhraseSearchQuery](https：//apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery（com.groupdocs.search.SearchQuery...)を呼び出して、サブクエリを組み合わせて新しいフレーズ検索クエリを作成します。 ） 方法
        * 検索を開始し、検索結果を表示します
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "フレーズ検索と他のタイプの検索を組み合わせるJavaAPI"
      content_left: |
        GroupDocs.Search Java APIを使用すると、ソフトウェアプログラマーはフレーズ検索を他のタイプの検索と簡単に組み合わせることができます。 次のJavaコードは、単語および単語内の文字を表すワイルドカードを使用してフレーズ検索を実行する方法を示しています。

      title_right: "フレーズ検索と他の検索を組み合わせる方法"
      content_right: |
        * インデックスフォルダとドキュメントフォルダへのパスを定義します。
        * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
        * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
         * [検索](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) メソッドを呼び出してテキストクエリで検索する
         *オブジェクト形式でフレーズ「フレーズテキスト」を検索します
        *単語パターンを定義し、文字列を追加してワイルドカードを追加します
        * [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern)) メソッドを呼び出してwordPattern1を作成し、word3を作成する
        * [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) メソッドを呼び出してwildcard2を作成する
        * [CreatePhraseSearchQuery](https：//apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery（com.groupdocs.search.SearchQuery...)) 方法 を呼び出して、サブクエリを組み合わせて新しいフレーズ検索クエリを作成します。
        *検索を開始し、検索結果を表示します
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

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