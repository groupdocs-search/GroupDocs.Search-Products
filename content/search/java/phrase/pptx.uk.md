
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: uk
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Шукати фрази у PPTX за допомогою Java"
head_description: "GroupDocs.Search for Java покращує додатки Java розширеними можливостями пошуку фраз у вмісті документів."

############################# Header ############################
title: "Знайдіть фрази у документах" 
description: "Швидко знаходьте специфічні фрази з GroupDocs.Search for Java. Додайте потужні функції пошуку до ваших додатків Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Особливості GroupDocs.Search"
    link: "/search/java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) - це надійна бібліотека для індексування та пошуку тексту в документах. Вона підтримує понад 70 форматів файлів, включаючи PDF, документи Word, електронні таблиці Excel, зображення та ZIP-файли, гарантуючи швидкі та точні результати пошуку.

############################# Steps ############################
steps:
    enable: true
    title: "Як знайти фрази у документах PPTX"
    content: |
      [GroupDocs.Search](/search/java/) спрощує пошук фраз у документах PPTX. Використовуйте різні опції для звуження результатів пошуку в додатках Java.
      
      1. Створіть каталог для індексу пошуку.
      2. Вкажіть папку з файлами PPTX.
      3. Налаштуйте параметри пошуку.
      4. Отримайте та проаналізуйте результати пошуку.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        copy_tip: "клікніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Визначте шлях до індексу пошуку
        Index index = new Index("c:/MyIndex");

        // Вкажіть папку з документами
        index.add("c:/MyDocuments");

        // Встановіть параметри пошуку
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Виконайте запит на пошук
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Досліджуйте пошукову систему документів Java"
  description: "GroupDocs.Search for Java дозволяє виконувати пошуки фраз понад 70 форматами файлів. Знаходьте та організовуйте дані за допомогою розширених функцій пошуку."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Основні можливості GroupDocs.Search"
  features:
    # feature loop
    - title: "Пошук фраз"
      content: "Знайдіть точні фрази в ділових документах, таких як PDF, файли Word, презентації та електронні таблиці. Використовуйте джокери та інші параметри, коли точна фраза невідома."

    # feature loop
    - title: "Оптимізоване індексування даних"
      content: "Прискорте пошук документів, створюючи та повторно використовуючи індекси пошуку. Індексація організує дані ефективно для швидших і точніших пошуків."

    # feature loop
    - title: "Сумісність з кількома мовами"
      content: "Шукайте документи більш ніж 80 мовами. Підтримує різні розкладки клавіатури та морфологічний аналіз для підвищення точності пошуку."

    # feature loop
    - title: "Розширені параметри пошуку"
      content: "Настройте пошуки з урахуванням регістру, нечіткого пошуку, відповідності гомофонам, фільтрації документів та інших потужних функцій."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання розширених методів пошуку"
      content: |
        Дізнайтеся, як скласти запити для пошуку у PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Визначте каталог для індексу пошуку
          Index index = new Index("c:/MyIndex");
              
          // Встановіть шлях до цільових документів
          index.add("c:/MyDocuments");

          // Створіть запит на пошук для конкретної фрази
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Отримайте результати пошуку
          SearchResult result = index.search(query);
          
          // Обробіть та використайте отримані результати
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Копіювати"
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
          copy_tip: "клікніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pptx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "завантаження Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Розширені можливості пошуку"
    exclude: "phrase"
    description: "Скористайтеся передовими функціями пошуку для покращення точності та продуктивності."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Шукати фрази у ділових документах"
    exclude: "PPTX"
    description: "GroupDocs.Search дозволяє шукати фрази у більш ніж 70 форматах документів. Використовуйте розширені опції та індексування для ефективних пошуків."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---