### EVM-1

 Zaczynamy od scanowania za pomocą nmapa.

![27](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2016-08-27.png)

 Jak widzimy http od razu sprawdzamy stronę

![strona](https://github.com/utlik/Images/blob/EVM-1/strona.PNG)

 Możemy zauważyć wskazówkę: `you can find me at /wordpress/ im vulnerable webapp :)`
Dla tego zaczynamy szukać dirbem

![03](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2016-33-03.png)

Widzimy, że jest jakaś strona 192.168.56.103/wordpress. Sprawdzamy:

![snimok](https://github.com/utlik/Images/blob/EVM-1/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA.PNG)

Co? Komentarze? 

![corru](https://github.com/utlik/Images/blob/EVM-1/corru.PNG)

`you can run wpscan (aggressive scan mode)` okej, co to jest na narzędzie? Zainstalujmy go

![install](https://github.com/utlik/Images/blob/EVM-1/install.PNG)

Patrzymy dokumentację wpscana i zaczynamy skanować:

![26](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-02-26.png)

![53](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-02-53.png)

![44](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-03-44.png)


Znależliśmy usera, który i był komentatorom :)

Za pomocą tego wpscan szukamy hasło:

![41](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-32-41.png)

![06](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-33-06.png)

Udało się, a teraz możemy popatrzeć na stronę wewnątrz.

![1](https://github.com/utlik/Images/blob/EVM-1/1.PNG)

![weszlismy](https://github.com/utlik/Images/blob/EVM-1/weszlismy.PNG)

![comments](https://github.com/utlik/Images/blob/EVM-1/comments.PNG)

Za pomocą exploitu próbujemy wejść:

![login](https://github.com/utlik/Images/blob/EVM-1/login.PNG)

![06](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-53-06.png)

![16](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-53-16.png)

![13](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-55-13.png)

I już mamy hasło od roota.

![57-01](https://github.com/utlik/Images/blob/EVM-1/Screenshot%20from%202020-01-16%2017-57-01.png)

Sukces!

























