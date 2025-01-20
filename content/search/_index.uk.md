---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: uk

############################# Head ############################
head_title: "Пошук тексту документів та індексація | APIs та безкоштовний веб-додаток"
head_description: "Виконуйте ефективний пошук тексту та індексацію даних у PDF, MS Office, OpenDocument та інших популярних форматах файлів за допомогою наших API або безкоштовного онлайн-додатку Document Search."

############################# Header ############################
title: "Всеосяжне рішення для пошуку документів та індексації"
description:  |
  Виконуйте пошук тексту та індексацію в PDF, Microsoft Office, OpenOffice та багатьох інших форматах документів.

  Швидко знаходьте інформацію у великих колекціях документів за допомогою розширених можливостей повнотекстового пошуку.

  Налаштуйте функції пошуку, такі як синоніми, нечіткий пошук та стемінг, щоб покращити точність та результати.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Виберіть вашу платформу"
  title: "Незалежність від платформи"
  description: "GroupDocs.Search сумісний з наступними операційними системами та фреймворками:"
  details_link_title: "Дізнайтеся більше"

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
                    Atom <br> Visual Studio Code <br> Будь-який інший текстовий редактор
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Ключові можливості GroupDocs.Search"
  description: "GroupDocs.Search надає потужні інструменти для індексації та пошуку тексту у популярних форматах документів. Спростіть та покращте управління документами з допомогою розширених функцій пошуку."

  items:
    # items loop
    - icon: "view"
      title: "Розширений пошук тексту"
      content: "Швидкі та точні пошуки тексту по проіндексованих документах."

    # items loop
    - icon: "manipulate"
      title: "Налаштовувані параметри пошуку"
      content: "Використовуйте функції, такі як нечіткий пошук, синоніми та стемінг для більш точних результатів."

    # items loop
    - icon: "merge"
      title: "Підтримка кількох форматів"
      content: "Індексуйте та шукайте вміст у Microsoft Office, PDF, OpenOffice та інших звичних форматах."

    # items loop
    - icon: "additional"
      title: "Ефективна індексація"
      content: "Швидко створюйте та підтримуйте індекси для великих колекцій документів."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Пошук тексту в популярних форматах документів"
  description: "GroupDocs.Search приклади коду"
  items:
    # code sample loop
    - title: "Пошук тексту"
      content: |
       GroupDocs.Search є потужним інструментом для знаходження тексту в документах. Ви можете шукати серед кількох документів різних форматів, збережених у конкретній папці. Результати пошуку зберігаються в окремій папці, що дозволяє вам отримувати доступ і повторно використовувати їх без повторного виконання пошуку.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Створіть екземпляр класу Index, вказавши папку для зберігання індексів.
            Index index = new Index("\\Index Folder");

            //Вкажіть шлях до документів, в яких буде виконуватися пошук.
            index.Add("\\Documents Folder");

            //Створіть екземпляр об'єкта SearchOptions.
            SearchOptions options = new SearchOptions();

            //Виконайте пошук необхідного тексту.
            SearchResult result = index.Search("ipsum dolor", options);

            //Обробіть результати пошуку.
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
            // Створіть екземпляр класу Index, вказавши папку для зберігання індексів.
            Index index = new Index("\\Index Folder");

            //Вкажіть шлях до документів, в яких буде виконуватися пошук.
            index.add("\\Documents Folder");

            //Створіть екземпляр об'єкта SearchOptions.
            SearchOptions options = new SearchOptions();

            //Виконайте пошук необхідного тексту.
            SearchResult result = index.search("ipsum dolor", options);

            //Обробіть результати пошуку.
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

            // Створіть екземпляр класу Index, вказавши папку для зберігання індексів.
            const index = new searchLib.Index('\\Index Folder');

            //Вкажіть шлях до документів, в яких буде виконуватися пошук.
            index.add('\\Documents Folder');

            //Створіть екземпляр об'єкта SearchOptions.
            const options = new searchLib.SearchOptions();

            //Виконайте пошук необхідного тексту.
            const result = index.search('ipsum dolor', options);

            //Обробіть результати пошуку.
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
  title: "Підтримка понад 70 форматів файлів"
  description: "GroupDocs.Search підтримує майже всі широко використовувані формати файлів"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Статистика нашого продукту"
  description: "Відкрийте ключові показники, що демонструють нашу продуктивність, охоплення та зростання."

  items:
    # items loop
    - number: "70+"
      title: "Підтримувані формати"
      content: "Ми забезпечуємо сумісність з понад 70 популярними форматами документів."

    # items loop
    - number: "500k"
      title: "Завантаження з NuGet"
      content: "GroupDocs.Search для .NET було завантажено більше 500,000 разів на NuGet."

    # items loop
    - number: "12k"
      title: "Завантаження з Maven"
      content: "Розробники Java завантажили GroupDocs.Search більше 12,000 разів з Maven."

    # items loop
    - number: "150+"
      title: "Задоволені клієнти"
      content: "Розробники та провідні компанії у всьому світі покладаються на наші продукти для інноваційних рішень."


############################# Customers ###############################
customers:
  enable: true
  title: "Наші задоволені клієнти"
  description: "Бібліотеки GroupDocs користуються довірою провідних брендів та організацій в усьому світі."

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
  title: "Розпочніть свою подорож сьогодні!"
  description: "Спробуйте GroupDocs.Search безкоштовно на вашій улюбленій платформі."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Часто задавані питання"
  description: "Знайдіть відповіді на поширені питання про GroupDocs.Search."

  items:
    # items loop
    - question: "Чи потрібні GroupDocs.Search зовнішні інструменти для пошуку документів?"
      answer: "Ні, GroupDocs.Search працює як автономне рішення і не потребує додаткових інструментів або програмного забезпечення, таких як Adobe Acrobat або Microsoft Office для виконання пошуку."

    # items loop
    - question: "Чи можу я протестувати GroupDocs.Search перед покупкою?"
      answer: "Так, ви можете! GroupDocs.Search пропонує безкоштовну пробну версію. Ви можете дослідити його можливості, хоча пробна версія може включати обмеження, такі як водяні знаки або обмежена функціональність. Щоб розблокувати всі функції, ви можете запросити безкоштовну тимчасову ліцензію на 30 днів. Дізнайтеся більше на сторінці [тимчасова ліцензія](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Які варіанти ліцензування доступні?"
      answer: "Ми пропонуємо кілька моделей ліцензування для GroupDocs.Search, адаптованих до різних потреб. Виберіть ліцензію, виходячи з розміру вашої команди, сценарію використання або чи потрібен вам SDK/API для розподілу клієнтів. Для більшої гнучкості розгляньте ліцензію з обліком, де ви платите на основі фактичного використання. Дізнайтеся більше про ваші варіанти на сторінці [цін](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Веб-додатки"
  description: "Досліджуйте GroupDocs.Search за допомогою нашого безкоштовного веб-додатку. Виконуйте текстовий пошук та індексацію у понад 70 популярних форматах файлів безпосередньо у вашому браузері — абсолютно безкоштовно."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Шукайте в PDF, Excel, Word, PowerPoint та інших типах файлів безпосередньо з вашого веб-браузера."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Завантажте DOCX для виконання розширених текстових пошуків без необхідності встановлювати програмне забезпечення."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Перевірте можливості індексації та отримання PDF у різних форматах безкоштовно."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---