# Kioptrix: Level 1

1. Z wyniku skanowanie nmap widać, lakie porty są otwarte

![nmap 15](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-56-15.png)

Widzimy, że wlączony jest service https. Szukamy stronę w google:

![snimok](https://github.com/utlik/Images/blob/master/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA.PNG)

Przechodzimy po linku `DokumentRoot`

![1.png](https://github.com/utlik/Images/blob/master/1.PNG)

Szukamy versję Sumby

![40](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2021-02-40.png)

Poszukamy w exploitach `samba 2.2.`:

![searchsploit 11](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2020-24-11.png)

Konfigurujemy exploit i uruchomiamy.

![use exploit 38](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-46-38.png)

![set rhosts 59](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-46-59.png)

![payload, run 12](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-47-12.png)

Jesteśmy w Kioptrixu ako root.

![whoami 42](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-47-42.png)

Szukamy flagi

![ls -al 55](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-47-55.png)

![head 30](https://github.com/utlik/Images/blob/master/Screenshot%20from%202020-01-13%2019-48-30.png)

 HAPPY END



