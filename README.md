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

Змінимо вміст файлу hello.html на наступний: "<h1>Hello, World!</h1>". Перевіримо статус репозиторію ще раз і отримаємо повідомлення про те що наявні не збережені зміни:

![image alt](https://github.com/VladislavKostyuk-1/RPKS-lb1/blob/55ff34de05653060b0c72459b8099375429dde55/Screenshots/4.2.jpg)
