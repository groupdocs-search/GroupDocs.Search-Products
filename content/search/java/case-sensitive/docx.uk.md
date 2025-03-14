
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: uk
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Виконання пошуків з урахуванням регістру у DOCX з Java"
head_description: "API GroupDocs.Search for Java допомагає розробникам Java здійснювати пошук з урахуванням регістру у різних типах документів."

############################# Header ############################
title: "Пошук документів з урахуванням регістру" 
description: "GroupDocs.Search for Java дозволяє реалізувати точну функціональність пошуку з урахуванням регістру у ваших проектах на Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Отримати безкоштовно"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Дізнайтеся про GroupDocs.Search"
    link: "/search/java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) є універсальним інструментом для пошуку тексту та індексації у різних документах. Він підтримує понад 70 форматів, таких як PDF, файли Word, презентації PowerPoint, таблиці Excel, зображення та ZIP-файли, що дає змогу ефективно обробляти великий обсяг даних.

############################# Steps ############################
steps:
    enable: true
    title: "Посібник з пошуку з урахуванням регістру у файлах DOCX"
    content: |
      З використанням [GroupDocs.Search](/search/java/) ви можете здійснювати пошуки з урахуванням регістру у документах DOCX, підвищуючи ефективність ваших проектів на Java.
      
      1. Встановіть папку для зберігання індексу пошуку.
      2. Виберіть папку, що містить файли DOCX.
      3. Виконайте пошук з урахуванням регістру та зберіть результати.
      4. Обробіть та використайте результати пошуку.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат пошуку"
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
        copy_tip: "клікніть, щоб скопіювати"
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
        // Визначте місце для зберігання індексу
        Index index = new Index("c:/MyIndex");

        // Вкажіть папку, що містить документи для пошуку
        index.add("c:/MyDocuments");

        // Увімкніть режим чутливості до регістру у параметрах пошуку
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Виконайте пошук
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширені інструменти пошуку та індексації"
  description: "З GroupDocs.Search for Java ви можете оптимізувати пошук документів та індексацію для понад 70 форматів, спрощуючи знаходження та організацію інформації."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Основні переваги GroupDocs.Search"
  features:
    # feature loop
    - title: "Гнучкий текстовий пошук"
      content: "Шукайте через документи, такі як PDF, файли Word, електронні таблиці та презентації. Використовуйте такі інструменти, як точне збіг, нечіткий пошук та підтримка символів підстановки для уточнення результатів."

    # feature loop
    - title: "Ефективне управління індексами"
      content: "Організуйте та індексуйте великі обсяги даних для покращення швидкості пошуку та продуктивності при обробці великих колекцій документів."

    # feature loop
    - title: "Підтримка глобальних мов"
      content: "Виконуйте пошуки більше ніж на 80 мовах, забезпечуючи різноманітність клавіатурних макетів та лінгвістичних варіацій для кращої точності."

    # feature loop
    - title: "Кастомізація фільтрів пошуку"
      content: "Налаштуйте критерії пошуку з такими опціями, як чутливість до регістру, фільтрація за діапазоном дат та виключення небажаних слів або даних під час індексації."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Приклад: Запити на пошук з урахуванням регістру"
      content: |
        Цей приклад демонструє, як реалізувати пошуки з урахуванням регістру для документів DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Визначте директорію для індексу пошуку
          Index index = new Index("c:/MyIndex");
              
          // Вкажіть місце розташування папки документів
          index.add("c:/MyDocuments");

          // Налаштуйте запит на пошук
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Увімкніть чутливість до регістру у параметрах пошуку
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Виконайте пошук документів
          SearchResult result = index.search(wordQuery, options);
          
          // Обробіть отримані результати
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
          copy_tip: "клікніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
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
  title: "Готові розпочати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Огляд ключових функцій"
    exclude: "case-sensitive"
    description: "Познайомтеся з потужними та ефективними можливостями пошуку, які пропонує GroupDocs.Search for Java."
    items: 
          
        # operation loop 1
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Підтримувані формати файлів для пошуку"
    exclude: "DOCX"
    description: "GroupDocs.Search працює з понад 70 популярними форматами документів, пропонуючи можливості налаштування параметрів пошуку та ефективної індексації."
    items: 
        # format loop 1
        - name: "Чутливий до регістру пошук у DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Чутливий до регістру пошук у PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Чутливий до регістру пошук у PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Чутливий до регістру пошук у TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Чутливий до регістру пошук у XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---