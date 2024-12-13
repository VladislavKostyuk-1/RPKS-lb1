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
