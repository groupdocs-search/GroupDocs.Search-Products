
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: ru
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Выполнение чувствительных к регистру поисков в PPTX с помощью Java"
head_description: "API GroupDocs.Search for Java помогает разработчикам Java выполнять чувствительные к регистру поиски по нескольким типам документов."

############################# Header ############################
title: "Поиск документов с учетом регистра" 
description: "GroupDocs.Search for Java позволяет реализовать точные функции поиска с учетом регистра в ваших проектах на Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Получить бесплатно"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Узнайте о GroupDocs.Search"
    link: "/search/java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) — это универсальный инструмент для текстового поиска и индексации по различным документам. Он поддерживает более 70 форматов, таких как PDF, Word, PowerPoint, Excel, изображения и ZIP-файлы, что позволяет эффективно работать с большими объемами данных.

############################# Steps ############################
steps:
    enable: true
    title: "Руководство по поиску с учетом регистра в файлах PPTX"
    content: |
      Используя [GroupDocs.Search](/search/java/), вы можете выполнить чувствительные к регистру поиски в документах PPTX, улучшая ваши проекты на Java.
      
      1. Установите папку для хранения индекса поиска.
      2. Выберите папку, содержащую файлы PPTX.
      3. Запустите поиск с учетом регистра и соберите результаты.
      4. Обработайте и используйте полученные результаты поиска.
   
    code:
      platform: "java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат поиска"
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
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Определите расположение для хранения индекса
        Index index = new Index("c:/MyIndex");

        // Укажите папку, содержащую документы для поиска
        index.add("c:/MyDocuments");

        // Включите режим чувствительности к регистру в настройках поиска
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Выполните поиск
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные инструменты поиска и индексации"
  description: "С помощью GroupDocs.Search for Java вы можете оптимизировать поиск и индексацию документов более чем в 70 форматах, что упрощает поиск и организацию информации."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Основные возможности GroupDocs.Search"
  features:
    # feature loop
    - title: "Гибкий текстовый поиск"
      content: "Ищите в документах, таких как PDF, файлы Word, электронные таблицы и презентации. Используйте инструменты, такие как точное совпадение, нечеткий поиск и поддержка подстановочных знаков для уточнения ваших результатов."

    # feature loop
    - title: "Эффективное управление индексами"
      content: "Организуйте и индексируйте большие наборы данных, чтобы улучшить скорость поиска и производительность при обработке больших коллекций документов."

    # feature loop
    - title: "Поддержка глобальных языков"
      content: "Выполняйте поиск более чем на 80 языках, учитывая различные раскладки клавиатуры и языковые вариации для повышения точности."

    # feature loop
    - title: "Настраиваемые фильтры поиска"
      content: "Регулируйте параметры поиска с помощью таких опций, как чувствительность к регистру, фильтрация по диапазону дат и исключение нежелательных слов или данных во время индексации."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Пример: Запросы поиска с учетом регистра"
      content: |
        Этот пример демонстрирует, как реализовать чувствительные к регистру поиски для документов PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Определите каталог для индекса поиска
          Index index = new Index("c:/MyIndex");
              
          // Укажите местоположение папки с документами
          index.add("c:/MyDocuments");

          // Настройте запрос для поиска
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Активируйте чувствительность к регистру в параметрах поиска
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Выполните поиск документов
          SearchResult result = index.search(wordQuery, options);
          
          // Обработайте полученные результаты
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Копировать"
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
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.pptx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Search бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Обзор ключевых функций"
    exclude: "case-sensitive"
    description: "Откройте для себя мощные и эффективные возможности поиска, предлагаемые GroupDocs.Search for Java."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поддерживаемые форматы файлов для поиска"
    exclude: "PPTX"
    description: "GroupDocs.Search работает с более чем 70 популярными форматами документов, предлагая настраиваемые параметры поиска и эффективную индексацию."
    items: 
        # format loop 1
        - name: "Чувствительный к регистру поиск в DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Чувствительный к регистру поиск в PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Чувствительный к регистру поиск в PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Чувствительный к регистру поиск в TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Чувствительный к регистру поиск в XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---