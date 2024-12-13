# Вивчення GIT

Для початку, задамо ім'я та електронну пошту користувача. В якості імені введемо "Vladislav", а в якості пошти - "vladkostuk96@gmail.com".
Також встановимо main як гілку за замовчуванням, та увімкнемо автоматичне переведення рядків:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/8db9830f12d1fe209a453be14a684461beec0639/Screenshots/2.1.jpg)

У папці repositories, створимо порожню папку work, в цій папці за допомогою команди echo створимо файл hello.html з наступним текстом: "Hello, World!":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/55ff34de05653060b0c72459b8099375429dde55/Screenshots/2.2.jpg)

Створимо наш перший репозиторій, в який включимо файл hello.html. Зробимо наш перший коміт під назвою "Initial Commit":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/55ff34de05653060b0c72459b8099375429dde55/Screenshots/2.3.jpg)

Перевіримо поточний статус репозиторію ввіши "git status". З отриманого повідомлення впеннимося що після попереднього коміту не відбулося ніяких змін:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/55ff34de05653060b0c72459b8099375429dde55/Screenshots/3.1.jpg)

Змінимо вміст файлу hello.html на наступний: "<h1Hello, World!/h1>". Перевіримо статус репозиторію ще раз і отримаємо повідомлення про те що наявні не збережені зміни:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/55ff34de05653060b0c72459b8099375429dde55/Screenshots/4.2.jpg)

Підготуємо файл hello.html до коміту увівши "git add hello.html" та переконаймося що файл став підготовленим ще раз перевіривши статус. При наступному коміті зміні у файлі будуть збережені:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/5.1.jpg)

Спробуємо створити коміт за домогою редактору VisualStudio Code, для цього введемо команду "git commit" та побачимо наступне вікно:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/7.1.jpg)

Додамо до найпершої лінії коментар, що описуватиме зміни, та закриємо редактор, після чого консоль повідомить нас про успіх коміту:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/7.1_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/7.1_3.jpg)

Перевіримо статус щоб переконатися що не збережені зміни відстуні:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/7.2.jpg)

Додамо теги до hello.html та внесемо ці зміни до коміту:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.2.jpg)

Внесемо до файлу ще одну зміну, додавши секцію head, після цього перевіримо статус репозиторію не додавши останні зміни до коміту:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.3.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.4.jpg)

Можна помітити, що на цьому скриншоті файл hello.html згадується двічі, це свідчить про те, що кожен коміт зберігає не самі файли, а лише їхні зміни. Також, якщо ми зараз проведемо коміт, то другі зміни файлу не будуть використані:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.5.jpg)

В статусі говориться, що в нас все ще є незбережені зміни. Підготуємо зміни до коміту та перевіримо статус ще раз. Щвидко підготувати відразу всі зміни можна ввівши "git add .":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.6.jpg)

Проводимо коміт:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/8.7.jpg)

Переглянемо історію змін через "git log":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/9.0.jpg)

Історію змін також пожна переглянути в однострочному режимі додавши флаг --oneline

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/9.1.jpg)

На останньому скриншоті можемо побачити, що кожний коміт має свій хеш. Ми можемо повернутися до найпершого коміту через команду chekout з використанням хешу:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/10.1.jpg)

Перевіримо поточний вміст hello.html за допомогою команди cat. Як можемо бачити, поточний вміст ідентичний початковому:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/10.1_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/10.1_3.jpg)

Тепер повернемося до осттаньої версії гілки main:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/10.2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/10.2_2.jpg)

Коли мова йде про переключення між версіями, то з хешами може бути незручно працювати, для облегшення роботи можна використовувати теги, присвоїмо до поточної версії коміту тег v1 та подивимося як він відобразиться в історії змін:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.1.jpg)
![image_alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.1_2.jpg)

Давайте додамо тег v1-beta до передостанньої версії. Для початку треба переключитися на передостанню версію, зробити це можна без використання хешів увівши наступну комнаду - "git chekout v1~1", ця команда по суті означає "переключитися на одну версію до версії з тегом v1", після чого переглянемо вміст hello.html і переконаємося що ми дійсно на попередній версії:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.2.jpg)
![iamge alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.2_2.jpg)

Тепер можемо присвоїти цій версії тег v1-beta:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.2_3.jpg)

Тепер перевіримо наскільки зруно перемикатися між версіями використовуючи теги:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.3.jpg)

Ми можемо переглянути список усіх наявних тегів використавши команду "git tag":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.4.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/11.5.jpg)

Перед тим як продовжити виконання роботи, упевнимося що ми знаходимося на останній версії гілки main:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/12.1.jpg)

Давайте додамо до hello.html зайвий коментар, щоб перевірити як за допомогою контролю версій можна легко відміняти незвані зміни:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/12.2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/12.3.jpg)

Повернемо стан hello.html до його версії з репозиторію за допомоги команди chekout, після чого перевіримо вміст файлу і впенимося, що зайвий коментар дійсно зник:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/12.4.jpg)

Тепер спробуємо відмінити підготовлену до коміту зміну. Додами до hello.html ще один зайвий коментар та підготуємо його, після чого перевіримо статус зміни:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/13.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/13.1_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/13.2.jpg)

Процедура відміни підготовленої до коміту зміни дуже схожа до попередньої, але спочатку треба додатково ввести команду "git reset HEAD hello.html":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/13.3.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/13.4.jpg)

Додамо ще один зайвий коментар, але цього разу збережений в коміт:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/14.2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/14.2_2.jpg)

Для того щоб вімінити зміни з останнього коміту, необхідно створити ще один коміт, що видалить їх:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/14.3.jpg)

Нам відкривається редактор VisualStudio Code, закриємо його без внесення змін:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/14.3_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/14.3_3.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/14.4.jpg)

Помітимо останній коміт тегом oops:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/15.3.jpg)

Зтираємо всі коміти після коміту з тегом v1:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/15.4.jpg)

Ми хоч і зтерли всі останні коміти, але вони не являються видаленими, ми все ще можемо побачити їх використавши флаг --all після команди log:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/15.5.jpg)

Тег oops нам більше не потрібен, видалемо його та перевіримо його наявність через log:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/16.1.jpg)

Давайте вкажемо у файлі hello.html його автора то додамо цю зміну до коміту:
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/17.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/17.1_2.jpg)

Тепер, скажімо, що ми забули додати до останнього коміту електронну пошту автора, а створювати ще один коміт заради цього не є раціональним, тому зробимо цю зміну частиною останнього коміту та змінимо його опис за допомогою флагу --ammend:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/17.2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/17.3.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/86f24b367d77350fdb2bbc84b10ed0d312b28e25/Screenshots/17.4.jpg)

Попрактикуємося в роботі з декількома гілками, створимо гілку style в якій будемо працювати з css файлом:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/a26f32a958c42794bee69cf9daea88e148e9f27e/Screenshots/18.1.jpg)

Тепер створімо в цій гілці файл style.css:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/a26f32a958c42794bee69cf9daea88e148e9f27e/Screenshots/18.2_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/a26f32a958c42794bee69cf9daea88e148e9f27e/Screenshots/18.2.jpg)

Підключаємо style.css до hello.html:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/a26f32a958c42794bee69cf9daea88e148e9f27e/Screenshots/18.3.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/a26f32a958c42794bee69cf9daea88e148e9f27e/Screenshots/18.3_2.jpg)

Тепер ми маємо дві гілки:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/a26f32a958c42794bee69cf9daea88e148e9f27e/Screenshots/19.0.jpg)

Переключатися між гілками можна через команду "git switch". Переключившись на гілку main переглянемо вміст hello.html і побачимо, що зміни внесені в гілці style не торкнулися цієї гілки:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/19.1.jpg)

Тепер повернімося до гілки style і побачимо внесені нами зміни:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/19.2.jpg)

Ми можемо перегляди історію змін конкретних файлів:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/20.1.jpg)

Також можемо переглянути зміни внесені кокретним комітом:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/20.2.jpg)

Перейменуємо hello.html в index.html за домомогою команди mv і переглянемо яким чином на це відреагує репозиторій:

![iamge alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/20.3.jpg)

Гіт інтерпретував перейменування файлу як те, що ми видалили файл і створили новий, це можна виправити підготувавши файл до коміту:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/20.3_2.jpg)

Давайте перекинемо файл style.css в нову папку css. По суті, перейменування і пересування файлу - одна й таж сама операція. Але цього разу використаємо "git mv", аби гіт побачив пересування файлу саме як пересування, а не як видалення:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/20.4.jpg)

Зробимо коміт, та переглянемо історію змін файлу style.css. Якщо використаємо флаг --follow, то нам також відобразиться історія файлу до зміни його локації. Введемо команду із та без цього флагу щоб пеервірити різницю:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/20.4_2.jpg)

Перейдемо назад на гілку main, створимо файл README та закомітимо його:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/21.2.jpg)

Переглянемо наскільки відрізняється історія обох гілок, додоваши до команди log флаг --graph:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/22.1.jpg)

Давайте перейдемо до гілки style і спробуємо поєднати її з гілкою main через команду merge:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/23.1.jpg)

Давайте перевіримо як себе поведе репозиторій, якщо ми спробуємо внести зміну, що конфліктуватиме між гілками. Для цього перейдемо до гілки main та внесемо наступні зміни до hello.html (цей файл не був перейменований у цій гілці):

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/24.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/24.1_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/24.1_3.jpg)

Після коміту файлу REAME, гілка main була поєднана з гілкою style, але в гілці main присутнінй додатковий коміт, що не був поєднаний до гілки style:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/24.2.jpg)

Давайте спробуємо вирішити конфлікт. Переключаємося на гілку style та поєднуємо її з гілкою main:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.1.jpg)

Ми не можемо виконати поєднання через наявність конфлікту. Переглянемо статус репозиторію та вміст index.html. Вміст між <<<<<<< та >>>>>>> реперезентує конфлікт:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.1_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.1_3.jpg)

Ми можемо покинути процес поєднання гілок додавши до команди merge флаг --abort:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.2.jpg)

Трохи подумавши, ми тепер знаємо як вирішити конфлікт. Знову починаємо процес поєднання та редагуємо index.html до наступного вигляду:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.3.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.3_2.jpg)

Спробуємо зробити коміт та переглянемо поточний статус репозиторію:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.4.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/25.4_2.jpg)

Давайте повернемося до гілки style, але до того моменту перед тим як вона була поєднана з main. Це відбулося за 2 коміта до коміту з HEAD, тому використаємо команду "git reset --hard HEAD~2":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/27.1.jpg)

Тепер перевіримо істрію гілки style, в ній не повинно бути коміту з merge:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/27.2.jpg)

Поєднаємо main та style ще раз, але цього разу використавши команду rebase:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/28.1.jpg)

У нас знову виник конфлікт. Вирішимо його редагуванням файлу hello.html:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/28.1_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/28.1_3.jpg)


Після редагування файлу нам не треба робити коміт, ми можемо просто ввести команду "git add ." і продовжити процес поєднання. Після введення команди відкриється редактор, його можна закрити без змін:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/28.2_2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/fe4d1e728fb0b31375e235eee51a321f84975fc3/Screenshots/28.2.jpg)

Тепер проведемо оберенену операцію - переключимося на main та об'днаємо зі style:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/29.1.jpg)

Перевіримо історію змін гілки. Тепер main та style мають бути ідентичними:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/29.2.jpg)

Повернемося до папки з репозиторіями. Команда ls виводить назви папок та файлів в поточній папці:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/30.1.jpg)

Давайте зклонуємо репозитрій work та назвемо клоновану версію - home:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/30.2.jpg)

Відкриємо репозиторій home та перевіримо його вміст, як можемо бачити - він ідентичний репозиторію work:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/31.1.jpg)

Історія репозиторію теж була клонована:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/31.2.jpg)

Ввіши команду "git remote" побачимо, що клонований репозиторій знає назву віддаленого репозитрію за замовчуванням. щоб отримати додаткову інформацію про репозиторій origin, можемо використати команду "git remote show origin":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/32.0.jpg)

Якщо введемо команду "git branch", що повинна відображати наявні гілки в репозиторії, то отримаємо лише гілку main. Це тому-що, за замовчуванням, ця команда вказує лише локальні гілки:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/33.0.jpg)

Аби побачити список всіх гілок додамо до попередньої команди флаг -a:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/33.1.jpg)

Повернемося до репозиторію work та внесемо деякі зміни до файлу README, після чого зробимо коміт:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/34.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/34.1_2.jpg)

Повернемося до репозиторію home та введемо команду "git fetch", що завантажить коміти з віддаленого репозиторію в локальний:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/35.0.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/35.0_2.jpg)

Впевнимося, що клонований README не був змінений:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/35.1.jpg)


Об'єднаємо origin з main:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/36.1.jpg)

Створимо локальну гілку, що відстежуватиме віддалену. Флаг --max-count в команді log дозволяє обмежити кількість комітів що відобразиться в історії:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/37.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/37.1_2.jpg)

Створимо порожній репизиторій, в якого можна вільно додавти/брати файли:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/38.1.jpg)

Додамо репозиторій work.git як віддалений до нашого початкового репозиторію:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/39.0.jpg)

Відредагуємо файл README за допомогою текстового редактора vi, зробимо коміт та надішлемо зміни в відлаений репозиторій через команду "git push shared main":

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/40.1.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/40.2.jpg)
![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/40.3.jpg)

Переключимося на репозиторій home та вилучимо зміни зі спільного репозиторію:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/549bc6608eb6209971b6aeea6e63994f23d3fd5e/Screenshots/41.0.jpg)
