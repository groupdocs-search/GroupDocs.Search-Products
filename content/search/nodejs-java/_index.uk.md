---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: uk
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Бібліотека пошуку тексту та індексації Node.js для документів, PDF, Office та веб"
head_description: "Розширене рішення для пошуку тексту для програм Node.js, щоб здійснювати пошук, індексацію та збір даних з документів: PDF, Word, Excel, презентацій, електронних листів та веб-форматів."

############################# Header ############################
title: "Пошук та індексація документів за допомогою API Node.js"
description: "Покращте програми Node.js, реалізуючи текстовий пошук у всіх популярних форматах документів."
words:
  for: "для"

actions:
  main: "Безкоштовне завантаження NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Розпочніть свою подорож сьогодні!"
  description: "Вивчіть можливості GroupDocs.Search безкоштовно або отримайте ліцензію, щоб розблокувати її повний потенціал."

release:
  title: "Версія {0} випущена"
  notes: "Дивіться, що нового"
  downloads: "Завантаження"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Виконати текстовий пошук у папці за допомогою JavaScript"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Створіть індекс для ваших документів
    const index = new searchLib.Index('c:/MyIndex');

    // Додайте документи до індексу для ефективного пошуку
    index.add('c:/MyDocuments');
    
    // Шукайте конкретні слова або фрази, такі як
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Search"
  description: "Бібліотека Node.js JavaScript для пошуку тексту"
  features:
    # feature loop
    - title: "Операції індексації та пошуку Node.js"
      content: "Індексація в GroupDocs.Search for Node.js via Java збирає, зберігає та обробляє дані для точних та ефективних операцій пошуку. Ці індекси часто використовуються для виконання пошуків."

    # feature loop
    - title: "Об'єднуйте кілька індексів для підвищення ефективності пошуку"
      content: "GroupDocs.Search for Node.js via Java API дозволяє об'єднувати кілька індексів в один. Часті модифікації створюють декілька дельта-індексів, які можуть сповільнити продуктивність пошуку. Наше рішення об'єднує ці дельта-індекси в загальний індекс, що містить всю інформацію з об'єднаних дельта-індексів, що значно підвищує ефективність пошуку, зберігаючи при цьому дельта-індекси незмінними. Різні функції можуть бути налаштовані для точного керування цим процесом."

    # feature loop
    - title: "Розпізнавання пошукових запитів з різних клавіатурних розкладок"
      content: "GroupDocs.Search for Node.js via Java розпізнає пошукові запити, які не відповідають клавіатурній розкладці. Наразі підтримується 88 мов та 164 різні клавіатурні розкладки."

    # feature loop
    - title: "Пошук із застосуванням морфологічних форм слів"
      content: "З GroupDocs.Search for Node.js via Java ви можете шукати різні форми слів, такі як однина і множина, або всі форми дієслова. Англійська та інші мови можуть бути налаштовані для специфічних форм слів."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність від платформи"
  description: "GroupDocs.Search for Node.js via Java сумісний з усіма популярними операційними системами та менеджерами пакетів."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Search for Node.js via Java дозволяє обробку широкого спектра форматів файлів. [Досліджуйте повний список](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Популярні офісні формати
        * **Портативний:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Текст:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Медіа формати
        * **Популярні формати зображень:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Багатосторінкові зображення:** GIF, WEBP, TIFF
        * **Аудіо:** MP3, WAV
        * **Відео:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Інші
        * **Електронна пошта:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Веб:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Інші:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java можливості"
  description: "Контролюйте вміст бізнес-документів за допомогою нашого розширеного пошукового механізму, що підтримує популярні формати файлів, включаючи PDF, DOCX, XLSX, PPTX та інші."

  items:
    # feature loop
    - icon: "document_info"
      title: "Гнучкі параметри"
      content: "Використовуйте діапазони дат та чутливість до регістру як параметри пошуку"

    # feature loop
    - icon: "detect"
      title: "Пошук з перевіркою правопису"
      content: "Використовуйте фрази пошуку з перевіркою правопису та підстановочними знаками та пропускайте спеціальні символи в запитах"

    # feature loop
    - icon: "collect"
      title: "Фільтрація результатів"
      content: "Налаштуйте фільтрацію документів у результатах пошуку"

    # feature loop
    - icon: "get"
      title: "Імпорт та експорт"
      content: "Виконуйте імпорт або використовуйте список для зміни символів під час індексації та експортуйте в файл"

    # feature loop
    - icon: "remove"
      title: "Пропустити непотрібні дані"
      content: "Вибірково пропускайте індексацію для певних файлів та пропускайте конкретні слова для швидшої індексації"

    # feature loop
    - icon: "style"
      title: "Обробка URL"
      content: "Витягуйте текст у форматі HTML в файл і генеруйте URL, щоб переходити до результатів пошуку в HTML"

    # feature loop
    - icon: "detect"
      title: "Швидкий пошук"
      content: "Розділіть пошук на менші частини, щоб швидко шукати у великих індексах"

    # feature loop
    - icon: "manipulate"
      title: "Обробка потоків"
      content: "Індексуйте документи з потоків та структур даних"

    # feature loop
    - icon: "compare"
      title: "Обробка помилок у написанні"
      content: "Дозвольте точну кількість появ кожного знайденого слова, щоб пропонувати альтернативи у разі помилки в написанні"

    # feature loop
    - icon: "unreadable_characters"
      title: "Підтримка архівів"
      content: "Індексуйте ZIP-архіви всередині інших ZIP-архівів і отримуйте список проіндексованих файлів в архіві"

    # feature loop
    - icon: "hidden_print"
      title: "Економія місця на диску"
      content: "Зберігайте місце завдяки компактній індексації та індексуйте документи, що захищені паролем"

    # feature loop
    - icon: "style"
      title: "Власні синоніми"
      content: "Додавайте англійські синоніми до стандартного словника синонімів"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Приклади коду"
  description: "Вивчайте можливості GroupDocs.Search for Node.js via Java за допомогою прикладів"
  items:
    # code sample loop
    - title: "Використовуйте 'нечіткий' пошук, щоб підвищити продуктивність"
      content: |
        Отримайте вигоду від гнучкого функціоналу GroupDocs.Search for Node.js via Java, щоб покращити контроль вмісту документів завдяки складним алгоритмам пошуку. [Дізнайтеся більше](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Як обробити результати пошуку">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Створіть індекс
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Налаштуйте параметри пошуку
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Шукайте документи, що містять слово 'вода' або фразу 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Обробіть результати пошуку
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Регулярні вирази доступні для розширених сценаріїв пошуку"
      content: |
        GroupDocs.Search for Node.js via Java дозволяє використовувати регулярні вирази для звуження результатів пошуку. [Зануртесь у розширені пошукові техніки](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Як шукати за допомогою регулярних виразів">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Створіть індекс
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Шукайте фразу у текстовій формі

        // Перший символ каретки на початку вказує, що це запит пошуку регулярного виразу
        const query = '^^(.)\\1{1,}';
        // Шукайте дві або більше ідентичні літери на початку слова
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
