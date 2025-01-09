---
############################# Static ############################
layout: "family"
date:  2025-01-09T15:38:59
draft: false

product: "Search"
product_tag: "search"

lang: ru

############################# Head ############################
head_title: "Поиск текста в документах и индексирование | API и бесплатное веб-приложение"
head_description: "Эффективный поиск текста и индексирование данных в PDF, MS Office, OpenDocument и других популярных форматах файлов с помощью наших API или бесплатного онлайн приложения для поиска документов."

############################# Header ############################
title: "Полное решение для поиска и индексирования документов"
description:  |
  Выполняйте поиск текста и индексирование в PDF, Microsoft Office, OpenOffice и многих других форматах документальных файлов.

  Быстро находите информацию в больших коллекциях документов с помощью расширенных возможностей полнотекстового поиска.

  Настройте функции поиска, такие как синонимы, нечеткий поиск и стемминг для повышения точности и результатов.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Выберите свою платформу"
  title: "Независимость от платформы"
  description: "GroupDocs.Search совместим с следующими операционными системами и фреймворками:"
  details_link_title: "Узнать больше"

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
                    Atom <br> Visual Studio Code <br> Любой другой текстовый редактор
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Ключевые функции GroupDocs.Search"
  description: "GroupDocs.Search предоставляет мощные инструменты для индексирования и поиска текста в популярных форматах документов. Упрощайте и улучшайте управление документами с помощью расширенной функциональности поиска."

  items:
    # items loop
    - icon: "view"
      title: "Расширенный текстовый поиск"
      content: "Выполняйте быстрые и точные текстовые поиски по индексированным документам."

    # items loop
    - icon: "manipulate"
      title: "Настраиваемые параметры поиска"
      content: "Используйте функции, такие как нечеткий поиск, синонимы и стемминг для более точных результатов."

    # items loop
    - icon: "merge"
      title: "Поддержка множества форматов"
      content: "Индексируйте и ищите содержимое в Microsoft Office, PDF, OpenOffice и других общих форматах."

    # items loop
    - icon: "additional"
      title: "Эффективное индексирование"
      content: "Быстро создавайте и поддерживайте индексы для больших коллекций документов."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Поиск текста в популярных форматах документов"
  description: "GroupDocs.Search примеры кода"
  items:
    # code sample loop
    - title: "Поиск текста"
      content: |
       GroupDocs.Search — это мощный инструмент для поиска текста в документах. Вы можете искать в нескольких документах в различных форматах, хранящихся в определенной папке. Результаты поиска сохраняются в отдельной папке, что позволяет вам получить доступ к ним и повторно использовать их без повторного поиска.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Создайте экземпляр класса Index, указав папку для хранения индексов.
            Index index = new Index("\\Index Folder");

            //Укажите путь к документам, где будет выполнен поиск.
            index.Add("\\Documents Folder");

            //Создайте экземпляр объекта SearchOptions.
            SearchOptions options = new SearchOptions();

            //Выполните поиск нужного текста.
            SearchResult result = index.Search("ipsum dolor", options);

            //Обработайте и проанализируйте результаты поиска.
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
            // Создайте экземпляр класса Index, указав папку для хранения индексов.
            Index index = new Index("\\Index Folder");

            //Укажите путь к документам, где будет выполнен поиск.
            index.add("\\Documents Folder");

            //Создайте экземпляр объекта SearchOptions.
            SearchOptions options = new SearchOptions();

            //Выполните поиск нужного текста.
            SearchResult result = index.search("ipsum dolor", options);

            //Обработайте и проанализируйте результаты поиска.
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

            // Создайте экземпляр класса Index, указав папку для хранения индексов.
            const index = new searchLib.Index('\\Index Folder');

            //Укажите путь к документам, где будет выполнен поиск.
            index.add('\\Documents Folder');

            //Создайте экземпляр объекта SearchOptions.
            const options = new searchLib.SearchOptions();

            //Выполните поиск нужного текста.
            const result = index.search('ipsum dolor', options);

            //Обработайте и проанализируйте результаты поиска.
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
  title: "Поддержка 70+ форматов файлов"
  description: "GroupDocs.Search поддерживает почти все широко используемые форматы файлов."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Статистика нашего продукта"
  description: "Узнайте ключевые показатели, демонстрирующие нашу производительность, охват и рост."

  items:
    # items loop
    - number: "70+"
      title: "Поддерживаемые форматы"
      content: "Мы обеспечиваем совместимость более чем с 70 популярными форматами документов."

    # items loop
    - number: "500k"
      title: "Скачивания NuGet"
      content: "GroupDocs.Search для .NET был загружен более 500,000 раз на NuGet."

    # items loop
    - number: "12k"
      title: "Скачивания Maven"
      content: "Разработчики на Java загрузили GroupDocs.Search более 12,000 раз из Maven."

    # items loop
    - number: "150+"
      title: "Удовлетворенные клиенты"
      content: "Разработчики и передовые компании по всему миру полагаются на наши продукты для внедрения инновационных решений."


############################# Customers ###############################
customers:
  enable: true
  title: "Наши довольные клиенты"
  description: "Библиотеки GroupDocs пользуются доверием ведущих брендов и организаций по всему миру."

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
  title: "Начните ваше путешествие сегодня!"
  description: "Используйте GroupDocs.Search бесплатно на вашей предпочитаемой платформе."

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
  title: "Часто задаваемые вопросы"
  description: "Найдите ответы на общие вопросы о GroupDocs.Search."

  items:
    # items loop
    - question: "Требует ли GroupDocs.Search внешние инструменты для поиска документов?"
      answer: "Нет, GroupDocs.Search работает как самостоятельное решение и не требует дополнительных инструментов или программного обеспечения, таких как Adobe Acrobat или Microsoft Office для выполнения поиска."

    # items loop
    - question: "Могу ли я протестировать GroupDocs.Search перед покупкой?"
      answer: "Да, вы можете! GroupDocs.Search предлагает бесплатный пробный период. Вы можете исследовать его функции, хотя пробная версия может включать ограничения, такие как водяные знаки или ограниченная функциональность. Чтобы разблокировать все функции, вы можете запросить бесплатную 30-дневную временную лицензию. Узнайте больше на странице [временной лицензии](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Какие варианты лицензирования доступны?"
      answer: "Мы предоставляем несколько моделей лицензирования для GroupDocs.Search, адаптированных под различные нужды. Выберите лицензию в зависимости от размера вашей команды, сценария использования или необходимости в SDK/API для распространения клиенту. Для гибкого использования рассмотрите вариант лицензии с оплатой по факту использования, где вы платите на основе фактического потребления. Узнайте больше о ваших вариантах на странице [ценообразования](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Веб-приложения"
  description: "Изучите GroupDocs.Search с помощью нашего бесплатного веб-приложения. Выполняйте текстовый поиск и индексирование более чем в 70 популярных форматах файлов непосредственно в вашем браузере — совершенно бесплатно."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Ищите в PDF, Excel, Word, PowerPoint и других типах файлов прямо из вашего веб-браузера."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Загрузите DOCX, чтобы выполнить расширенный текстовый поиск без необходимости установки программного обеспечения."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Протестируйте возможности индексирования PDF и извлечения информации по различным форматам бесплатно."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---