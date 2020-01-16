### DC-1

Zaczynamy od skanowania nmap

![14-53](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2016-14-53.png)

Widząc http szukamy stronę

![24-13](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2016-24-13.png)

![25-58](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2016-25-58.png)

Widząc drupal już 2 raz (na stronie i w vulnerabilities) szukamy exploit i używamy.

![33-51](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2017-33-51.png)

Weszliśmy, teraz sprawdzamy za jakiego użytkownika

![34-07](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2017-34-07.png)

whoami nie działa, ale działa getuid.

![47-39](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2017-47-39.png)

![34-30](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2017-34-30.png)

Flag Nr1 już u nas.

![34-46](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2017-34-46.png)

To wskazuje mi plik ustawień Drupal. Robię szybkie wyszukiwanie w Google i znajduję je w sites/default/settings.php.

![05-17](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2018-05-17.png)

![05-31](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2018-05-31.png)

![05-39](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2018-05-39.png)

Flag Nr2 +

Szukając więcej informacji wchodzę w `/etc` i widzę plik `passwd`. Muszę zobaczyć:

![54-05](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-14%2018-54-05.png)

Wskazówka na flag4. Kilka klików ...

![18-34](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2019-18-34.png)

...też mam. 
Flag Nr4 +

![25-45](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2019-25-45.png)

Ponieważ polecenie „find” ma ustawiony bit SUID, możemy wykonać to polecenie tylko jako użytkownik „root”. Tworzymy plik o nazwie „abc” i używamy polecenia „find”, 

![35-45](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2019-35-45.png)

Root!

![36-04](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2019-36-04.png)

Flag Nr5 +















