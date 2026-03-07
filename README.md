# CS-go-legacy-pterodactyl-egg
Всем привет вот пропатченное яйцо дня преродактель панели
Гайд для создания сервера 

[h2]Всем привет[/h2]

Данный гайд затрагивает не только запуск сервера кс го на pterodactyl panel!!!
В гайде так же затрагивается настройки для запуска csgo сервера на linux

[h1]Pterodactyl[/h1]

Все что используется в гайде 
Custom CS Go egg [url=github.com/ftethg/CS-go-legacy-pterodactyl-egg] Ссылка [/url]
sourcemod[url=https://www.sourcemod.net/downloads.php]тык[/url]
Metamod:source [url=https://www.sourcemm.net/downloads.php?branch=stable]тык[/url]
no-lobby-reservatio [url=https://github.com/vanz666/NoLobbyReservation/releases/tag/0.0.2]тык[/url]


Для начала скачиваете отредактированный egg у меня на github [url=github.com/ftethg/CS-go-legacy-pterodactyl-egg] Ссылка [/url]

Дальше в настройках панели
Выбираем Nests / Import Egg [url=ibb.co/jZLyk2S2] тык [/url]
В открывшимся окне загружаем файл и выбираем в графе Associated Nest, Source engine .
Нажимаем import .

Думаю как создавать сервера вы знаете если есть pterodactyl panel 
Для создания потребуется токен его делаем на app-id 4465480[url=https://steamcommunity.com/dev/managegameservers]тык[/url]
Source AppID 740 в панели

[h1]Сборка сервера для запуска[/h1]
После загрузки всех файлов .
Заходим в файлы сервера папка /bin
ищем файл libgcc_s.so.1  и переименовываем в libgcc_s.so.1.old

Дальше 
Заходим в папку /csgo и в файле steam.inf изменяем значение appID на 4465480

Если у вас не показываются файлы.
попробуйте зайти через sftp 
либо введите в строке браузера после id сервера /files/edit#/csgo/steam.inf

На данный момент сервер запускается но зайти не получится. 
что бы это пофиксить надо поставить no-lobby-reservation

Для него нам понадобятся:
  sourcemod[url=https://www.sourcemod.net/downloads.php]тык[/url]
  Metamod:source [url=https://www.sourcemm.net/downloads.php?branch=stable]тык[/url]
  no-lobby-reservatio [url=https://github.com/vanz666/NoLobbyReservation/releases/tag/0.0.2]тык[/url]
 Скачиваем их с официальных сайтов и распаковываем 
   Подключаемся к серверу через sftp 
      заходим в папку csgo/ и перекидываем по порядку sourcemod , Metamod и no-lobby-reservation
 После можно запустить сервер и заходить в игре
