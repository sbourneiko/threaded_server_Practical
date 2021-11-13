<!----- Conversion time: 0.718 seconds.
Using this Markdown file:

1. Cut and paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β17
* Wed Sep 18 2019 01:52:00 GMT-0700 (PDT)
* Source doc: https://docs.google.com/open?id=1SEODmwLcgVdQijJMZ6Xc3YQ0lqnkc72w-gccG4AkpqU
----->

## Создание простого многопоточного сервера

### Цель работы

Познакомиться с приемами работы с многопоточностью на примере создания сокетного TCP-сервера, способного работать с несколькими клиентами одновременно



### Дополнительные задания

2. Модифицировать простой эхо-сервер таким образом, чтобы при подключении клиента создавался новый поток, в котором происходило взаимодействие с ним.

![image](https://user-images.githubusercontent.com/70803921/141646409-d53f5d27-cbd3-485a-8720-8993885ce105.png)


3. Реализовать простой чат сервер на базе сервера аутентификации. Сервер должен обеспечивать подключение многих пользователей одновременно, отслеживание имен пользователей, поддерживать историю сообщений и пересылку сообщений от каждого пользователя всем остальным. 

![image](https://user-images.githubusercontent.com/70803921/141646332-8f3efaa2-57af-4349-8aa1-94ebfc5fb5e6.png)
![image](https://user-images.githubusercontent.com/70803921/141646342-c583de74-3d81-4c91-96e1-d3e3c162ee27.png)
![image](https://user-images.githubusercontent.com/70803921/141646364-379f308d-2ca3-4777-a86d-1039cc25b3ce.png)



4. Реализовать сервер с управляющим потоком. При создании сервера прослушивание портов происходит в отдельном потоке, а главный поток программы в это время способен принимать команды от пользователя. Необходимо реализовать следующие команды:

![image](https://user-images.githubusercontent.com/70803921/141646483-62c1d2af-c528-468c-9a07-5b8aebb2f695.png)
![image](https://user-images.githubusercontent.com/70803921/141646487-e404c7e2-987d-40a1-b5c5-a069d27c5553.png)

    1. Отключение сервера (завершение программы);
    
![image](https://user-images.githubusercontent.com/70803921/141646518-71ccfeb9-d589-458b-828d-027c126d9e59.png)

    2. Пауза (остановка прослушивание порта);

![image](https://user-images.githubusercontent.com/70803921/141646564-bf01d3f6-bb98-406a-96de-487c8743f846.png)
![image](https://user-images.githubusercontent.com/70803921/141646554-764beb19-13b6-44a8-b6df-888df9f1cf87.png)

    3. Показ логов;

![image](https://user-images.githubusercontent.com/70803921/141646601-1ff8fa6b-f9ab-4bdd-98e5-d5bb6c8c7af9.png)

    4. Очистка логов;

![image](https://user-images.githubusercontent.com/70803921/141646622-64671424-8c65-4f2d-859a-ff18d376a5c4.png)

    5. Очистка файла идентификации.

![image](https://user-images.githubusercontent.com/70803921/141646664-e70d7d81-11de-48cd-b613-4c9c09b62441.png)
![image](https://user-images.githubusercontent.com/70803921/141646703-0aa292e1-4bdb-4b54-8ad8-dcc7ef2ad320.png)
![image](https://user-images.githubusercontent.com/70803921/141646714-b48595a5-0e3a-4180-903c-349806023c43.png)


<!-- Docs to Markdown version 1.0β17 -->
