
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: uk
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Буліевий пошук у DOCX з Java"
head_description: "З допомогою GroupDocs.Search for Java розробники можуть здійснювати пошук документів, використовуючи булеві оператори, такі як AND, OR та NOT."

############################# Header ############################
title: "Буліевий текстовий пошук" 
description: "Використовуйте GroupDocs.Search for Java для створення розширених булевих (AND, OR, NOT) запитів у ваших проектах Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Про GroupDocs.Search"
    link: "/search/java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) - це універсальна бібліотека, розроблена для пошуку тексту та індексації даних у документах. Вона підтримує понад 70 форматів файлів, включаючи PDF, Word, Excel, PowerPoint, зображення та ZIP-архіви, що дозволяє ефективно шукати у великих сховищах даних.

############################# Steps ############################
steps:
    enable: true
    title: "Як здійснити булеві пошуки в документах DOCX"
    content: |
      [GroupDocs.Search](/search/java/) дозволяє здійснювати текстові пошуки в документах DOCX. Завдяки підтримці булевих умов ви можете покращити точність пошуку в програмах Java.
      
      1. Вкажіть папку для зберігання індексу пошуку.
      2. Виберіть папку з документами DOCX.
      3. Виконайте запит пошуку та отримайте результати.
      4. Обробіть отримані результати.
   
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
        // Встановіть шлях до папки для індексу
        Index index = new Index("c:/MyIndex");

        // Вкажіть шлях до папки з документами для пошуку
        index.add("c:/MyDocuments");

        // Запустіть пошук з комплексним запитом
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Потужні інструменти для пошуку документів та індексації"
  description: "GroupDocs.Search for Java спрощує пошук тексту та індексацію даних для понад 70 форматів. Його розширені інструменти дозволяють знаходити та управляти контентом без зайвих зусиль."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Ключові особливості GroupDocs.Search"
  features:
    # feature loop
    - title: "Комплексний текстовий пошук"
      content: "Шукайте у різних форматах, таких як PDF, документи Word, презентації, електронні таблиці та інші. Використовуйте опції, такі як точне співпадіння, нечіткий пошук та запити з підстановковими знаками для уточнення результатів."

    # feature loop
    - title: "Ефективна індексація даних"
      content: "Створюйте та підтримуйте індекси для швидшого пошуку документів. Ця функція організовує дані результативно, що спрощує роботу з великими колекціями документів."

    # feature loop
    - title: "Підтримка багатьох мов"
      content: "Шукайте у документах, написаних понад 80 мовами. Покращуйте точність, використовуючи морфологічні форми слів та різні розкладки клавіатури."

    # feature loop
    - title: "Гнучка настройка пошуку"
      content: "Налаштуйте параметри пошуку за допомогою таких функцій, як чутливість до регістру, фільтри за датою та виключення, щоб уточнити ваші результати."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання складних булевих запитів"
      content: |
        Цей приклад демонструє, як виконувати булеві пошуки у файлах DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Встановіть папку для індексу пошуку
          Index index = new Index("c:/MyIndex");
              
          // Вкажіть шлях до документів для пошуку
          index.add("c:/MyDocuments");

          // Сформулюйте запит, використовуючи булеву логіку
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Отримайте результати пошуку
          SearchResult result = index.search(booleanQuery);
          
          // Обробіть знайдені результати
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
            link: "/examples/search/formats/searchboolean.docx"
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
    title: "Ключові особливості в одному погляді"
    exclude: "boolean"
    description: "Відкривайте потужні та ефективні можливості пошуку"
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
    title: "Пошук популярних форматів документів"
    exclude: "DOCX"
    description: "GroupDocs.Search підтримує понад 70 форматів файлів, що дозволяє вам налаштовувати правила пошуку та використовувати індексацію для оптимізації продуктивності."
    items: 
        # format loop 1
        - name: "Логічний пошук у DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Логічний пошук у PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Логічний пошук у PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Логічний пошук у TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Логічний пошук у XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---