
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: uk
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Знайдіть текст у документах XLSX з GroupDocs.Search для Java"
head_description: "GroupDocs.Search for Java допомагає розробникам Java швидко шукати текст у різних форматах документів."

############################# Header ############################
title: "Розумний пошук тексту в документах" 
description: "З GroupDocs.Search for Java ви можете безперешкодно шукати та витягувати текст з кількох типів документів у ваших додатках Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Отримати безкоштовну версію"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Що робить GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) — це потужна бібліотека для пошуку та індексування документів, яка підтримує понад 70 форматів файлів, включаючи PDF, Word, PowerPoint, Excel, зображення та ZIP-архіви. Вона забезпечує швидкі, точні та масштабовані можливості пошуку для великих колекцій документів.

############################# Steps ############################
steps:
    enable: true
    title: "Виконання текстових пошуків у файлах XLSX"
    content: |
      [GroupDocs.Search](/search/java/) спрощує пошук у файлах XLSX за допомогою складної логіки та індексування, підвищуючи точність пошуку в додатках Java.
      
      1. Налаштуйте каталог для зберігання індексу пошуку.
      2. Виберіть папку, що містить файли XLSX.
      3. Визначте додаткові параметри пошуку.
      4. Виконайте пошук та проаналізуйте результати.
   
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
        // Встановіть каталог для зберігання індексу пошуку
        Index index = new Index("c:/MyIndex");

        // Вкажіть папку, що містить документі, які можна шукати
        index.add("c:/MyDocuments");

        // Увімкніть пошук для омонімів, щоб знайти слова з подібною вимовою
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Виконайте розширений запит пошуку
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Покращені можливості пошуку та індексування"
  description: "GroupDocs.Search for Java спрощує пошук тексту та індексування в понад 70 форматах документів, надаючи ефективні інструменти для швидкого управління та пошуку інформації."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Основні можливості GroupDocs.Search"
  features:
    # feature loop
    - title: "Всебічний пошук тексту"
      content: "Знайдіть текст у різних форматах документів, таких як PDF, документи Word, презентації PowerPoint та електронні таблиці. Використовуйте точні відповідності, нечіткий пошук та оператори підстановки для підвищення точності результатів."

    # feature loop
    - title: "Оптимізоване індексування для великих даних"
      content: "Створюйте структуровані індекси, щоб прискорити пошук, спрощуючи навігацію через величезні репозиторії документів."

    # feature loop
    - title: "Підтримка багатьох мов"
      content: "Виконуйте пошуки більш ніж 80 мовами з вбудованою підтримкою різних розкладок клавіатури та варіацій морфології слів, що підвищує точність."

    # feature loop
    - title: "Гнучкі налаштування пошуку"
      content: "Налаштуйте пошуки зі змінними, такими як чутливість до регістру, фільтрація за датою та можливість виключення певних слів для точних результатів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Реалізація розширених запитів пошуку"
      content: |
        Цей приклад ілюструє, як використовувати запити пошуку для ефективного пошуку у документах XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Визначте каталог для індексування пошуку
          Index index = new Index("c:/MyIndex");
              
          // Вкажіть шлях до файлів документів
          index.add("c:/MyDocuments");

          // Введіть пароль для зашифрованих документів
          index.getDictionaries().getDocumentPasswords().add("protected.xlsx", "123456");

          // Увімкніть нечіткий пошук для виявлення схожих слів
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Отримайте результати пошуку
          SearchResult result = index.Search("Loarem", options);
          
          // Обробіть та проаналізуйте результати пошуку
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    exclude: "document"
    description: "Відкрийте високопродуктивні функціоналізми для пошуку тексту, розроблені для ефективності та точності."
    items: 
          
        # operation loop 1
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Знайдіть інформацію у документах XLSX з GroupDocs.Search"
    exclude: "XLSX"
    description: "GroupDocs.Search підтримує понад 70 форматів, включаючи офісні файли, що дозволяє швидко шукати з просунутими можливостями індексування."
    items: 
        # format loop 1
        - name: "Пошук у документі DOCX"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Пошук у документі PDF"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Пошук у документі PPTX"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Пошук у документі TXT"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Пошук у документі XLSX"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---