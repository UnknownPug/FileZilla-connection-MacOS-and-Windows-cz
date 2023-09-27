# FileZilla connection pro MacOS a Windows v rámci předmětu B6B39ZWA

## Autor: Dmitrij Rastvorov

## Tento popis slouží studentům k připojení k serveru zwa.toad.cz pomocí aplikaci FileZilla na počítačích Mac a Windows.

## Obsah

### [Instalace na macOS](#macos)

### [Instalace na Windows](#windows)

### [DŮLEŽITÉ KROKY při používání aplikace FileZilla v budoucnu](#impfz)

### [Video na YouTube](#youtube)

-- -- --

<a name="macos"><h2>Instalace na macOS (Program pracuje s čipem M1)</h2></a>

1) Nejprve se připojte k serveru pomocí příkazu `ssh username@zwa.toad.cz`. Dále, pokud se objeví **Are you sure you want to continue connecting (yes/no/[fingerprintl)?** napište **yes** a stiskněte Enter. 

<img width="1302" alt="1__ssh_username_wa toad cz" src="https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/965c88af-7760-424d-9873-19a58471d201">

### (username - Vaše přihlašovací jméno na ČVUT)

### (password - Vaše uživatelské heslo na ČVUT)

2) V novém okně prohlížeče zadejte do vyhledávacího pole `http://zwa.toad.cz/~username/` , kde se zobrazí chyba 404 s popisem (nebo 403 Forbidden).

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/8bf8dc33-a9b8-4bf3-9af2-b29a4e593e35)

### • Po tomto kroku nainstalujte program FileZilla:

3) Přejděte na tento odkaz: `https://filezilla-project.org/download.php?platform=osx` .

4) Klikněte na **Download FileZilla Client** a poté si stáhněte standardní verzi programu FileZilla **(nikdy ne manuální nebo profesionální verzi)**.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/c6c0d400-d0a1-491d-a73f-a9f86052ed1d)
![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/db9dd291-9217-4c09-b574-065430125ef5)


5) Stáhněte si aplikaci, přejděte do složky **Downloads**, otevřete archiv a přeneste aplikaci do složky **Applications**.

<img width="912" alt="5__Move_to_Applications" src="https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/234c451d-a75b-43e2-b824-2958145c7243">

6) Spusťte FileZillu a udělte ji oprávnění v případě, že si to program vyžádá.

7) V levém horním poli **Host** napište adresu, kterou budeme používat v tomto předmětu: `sftp://zwa.toad.cz`. Poté do pole **Username** napište přihlašovací jméno ČVUT a do pole **Password** napište Vaše uživatelské heslo ČVUT. Po vyplnění všech tří sloupců klikněte na tlačítko **Quickconnect**.

(Pokud se Vaše složka nezobrazuje, klikněte znovu na Quickconnect a program Vaši složku zobrazí)

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/54379ac7-534c-401b-80e8-ced7c591cee7)
    
8) Potvrďte připojení. Poté se na pravé straně zobrazí složka s Vaším přihlašovacím jménem.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/187bbe8f-64b6-4c95-9543-ed14efe978ef)
![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/1afcc9be-0931-4053-a695-4156c0106b26)

<a name="macOS9To14">9.</a> Otevřete tuto složku a vytvořte v ní složku `www/01` kliknutím pravým tlačítkem myši na složku s uživatelským jménem a výběrem možnosti **Create directory** (můžete to také udělat postupně, na začátku vytvořit složku `www` a poté složku `01`).

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/df761e33-a19e-4ddb-88fe-be59b03ebe1e)
![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/926f17ec-78b5-4758-a998-7901c171ade2)

10) Otevřete terminál a přejděte do složky 01 (`cd www/01` nebo `cd www` a pak `cd 01`), když už jste na serveru.

11) Uvnitř složky 01 vytvořte soubor **index.html** (`touch index.html`) a poté se vraťte do FileZilly. 

<img width="456" alt="10__Creating_html" src="https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/90a1c1c5-4baa-4d0b-b9d9-84d409997955">

12) V aplikaci FileZilla klikněte na tlačítko Aktualizovat v horní části lišty a aktualizujte soubory.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/5dd123da-74bb-42c7-8e56-0c2cba658a6b)

13) Otevřete složku 01, klikněte pravým tlačítkem myši na index.html a vyberte možnost **View/Edit**.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/5e4c310f-c255-4e5d-bac0-032e4fc9cf5a)

14) Klikněte na tlačítko **Browse** a vyberte prostředí IDE, které chcete použít k úpravě souborů **(Preferováno je Visual Studio Code)**.

15) Otevřete IDE a upravte soubor podle svých představ. Vytvořte například standardní kód html pro zobrazení textu na stránce:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Hello world!</title>
</head>
<body>
    <h1>Hello world!</h1>
</body>
</html>
```

16) Uložte změny **(Cmd + S)** a vraťte se do FileZilly.

<a name="macOS17To19">17.</a> Poté se zobrazí okno, ve kterém můžete změny uložit a odeslat na server. **V poli, kde se navrhuje lokální odstranění změn, neklikáme na nic!** Klikněte na tlačítko **YES** a soubor bude odeslán na server. (Výše v aplikaci můžete vidět výstup terminálu se informací, že soubor byl úspěšně odeslán na server).

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/1963577d-0758-4d98-8c86-d173dac38b43)

18) Otevřete stránku serveru zwa.toad.cz a znovu ji načtěte **(Cmd + R)**. Pak se zobrazí text, který byl napsán v index.html, nebo se zobrazí složka 01, kde se nachází soubor index.html. Pokud se vrátíme na stránku, uvidíme složku 01, kde se nachází soubor index.html.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/8c7cfff7-4bcd-4aef-adf7-a59ef6e44ab3)
![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/5fca0fd2-c639-4a2d-a7fa-1e1b1053b8e0)

19) Pokud otevřeme terminál a zadáme `telnet zwa.toad.cz 80`, napíšeme `GET / HTTP/1.0` a **dvakrát stiskneme Enter**, vidíme, že spojení skutečně existuje a že vše funguje!

<img width="939" alt="16__telnet" src="https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/a5a7a4bd-1644-4b68-9cbe-7f5a80709c7f">
-- -- --

<a name="windows"><h2>Instalace na Windows</h2></a>

1) Nejprve nainstalujte **terminál Ubuntu** (odkaz ke stažení z oficiálních stránek: `https://apps.microsoft.com/store/detail/ubuntu/9PDXGNCFSCZV`).

2) Poté otevřete Ubuntu a do terminálu zadejte příkaz `ssh username@zwa.toad.cz`. Dále potvrďte připojení **Are you sure you want to continue connecting (yes/no/[fingerprintl)?** napište **yes** a stiskněte Enter.

### (username - Vaše přihlašovací jméno na ČVUT)

### (password - Vaše uživatelské heslo na ČVUT)

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/2f3af8a6-cd38-468b-86dd-528835e8bcb2)

3) Přejděte na webovou stránku **FileZilla**: `https://filezilla-project.org/download.php?platform=win64`, klikněte na **Download FileZilla Client** a vyberte ke stažení standardní verzi programu FileZilla (nikdy ne manuální nebo profesionální verzi).

4) Otevřete aplikaci a projděte procesem instalace.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/10a1288d-8917-4d85-855c-682a1e7cfe69)

5) Aplikace vyzve k instalaci prohlížeče, před kliknutím na tlačítko Next si přečtěte popis. 

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/f334245e-2895-47ff-ae51-5f323b22657b)
 
6) Povolte přístup všem uživatelům tohoto počítače.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/350b3282-6a45-4bdc-bf9a-f03582369a12)


7) Vyberte **Desktop Icon**, chcete-li zobrazit zástupce na pracovní ploše. 

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/b0c5e605-00b8-4706-b8f5-48e13176422f)

8) Vyberte cestu pro instalaci aplikace. 

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/b0b06ebb-f9f6-45b5-8340-16099348114f)

9) Po stažení klikněte na tlačítko **Finish**. Spustí se aplikace FileZilla.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/a6e812e4-02d8-4c30-b522-4eba5e59bbd5)

10) V levém horním poli Host napište adresu, kterou budeme používat v tomto předmětu: sftp://zwa.toad.cz. Poté do pole Username napište přihlašovací jméno ČVUT a do pole Password napište Vaše uživatelské heslo ČVUT. Po vyplnění všech tří sloupců klikněte na tlačítko Quickconnect.

11) Poté se zobrazí okno s žádostí o uložení zadávaných údajů, abyste je nemuseli zadávat znovu. Vyberte Vámi preferovanou možnost a stiskněte tlačítko **OK**.

#### IMPORTANT: Pokud vyberete možnost "Neukládat hesla", bude k dispozici alternativní možnost připojení, jak je uvedeno v kroku 3 [(DŮLEŽITÉ KROKY při používání aplikace FileZilla v budoucnu)](#windowsAlternative).

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/53b62398-de38-48f7-ac2f-e457e047468f)

12) Potvrďte připojení. Stiskněte tlačítko **OK**.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/758339fb-2e6f-49f8-bf3c-35f25863c416)

##### 13. Postupujte podle bodů popsaných při instalaci aplikace FileZilla v systému macOS [(kroky 9-14)](#macOS9To14)

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/dd1bb9b0-f78b-40ef-98db-8606a66c4509)
![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/db18f267-d61e-4cd3-87e3-6cddbe113c6b)

14) Otevřete IDE a zadejte zadaný kód:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Hello Windows world!</title>
</head>
<body>
    <h1>Hello Windows world!</h1>
</body>
</html>
```

15) Uložte změny (`Ctrl + S`).

##### 16. Postupujte podle kroků popsaných v instalaci aplikace FileZilla v systému macOS [(kroky 17-19)](#macOS17To19).

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/f7c42388-dafd-4c3d-8872-6fb1fe88bc00)

-- -- --
<a name="impfz"><h2>DŮLEŽITÉ KROKY při používání aplikace FileZilla v budoucnu</h2></a>

#### 1) Při dlouhodobém používání aplikaci FileZilla, budeme soubory spouštět kliknutím pravým tlačítkem myši na soubor a výběrem možnosti Zobrazit/Upravit (View/Edit).

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/fad85baf-9a65-45c4-acf5-72a140ab2dd3)

#### 2) Při nahrávání semestrálního projektu na server zwa.toad.cz je možné nahrávat z lokálního počítače. Za tímto účelem vyhledejte složku s projektem v levém okně a přeneste ji na server, jak je uvedeno na obrázku:

<img width="1440" alt="13_Next_usage" src="https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/fc8b42df-7fc2-4cc2-b384-e0f6fe970285">

#### <a name="windowsAlternative">3)</a> Pro další připojení není třeba zadávat **Host, Username** a **Password**. Klikněte na šipku vedle položky **Quickconnect** a vyberte **svůj Host**. Dále je třeba zadat heslo a kliknout na tlačítko **OK**, poté je třeba potvrdit připojení a objeví se naše složka se soubory.

![](https://github.com/UnknownPug/FileZilla-connection-MacOS-and-Windows-cz/assets/73190129/789ff035-3d60-4f3c-9264-de39b1235bad)

-- -- --
<a name="youtube"><h2>Níže naleznete videonávod pro instalaci a práci s FileZillou v počítači Mac po jednotlivých krocích:</h2></a>

[![Watch the video](https://user-images.githubusercontent.com/73190129/256059107-9c9a4db4-6c67-4baf-836f-a1334f8acd2d.png)](https://www.youtube.com/watch?v=rX1lpdObLOQ)



-- -- --
#### To je ode mě všechno! Doufám, že Vám tento popis pomůže pochopit tuto aplikaci!

#### Hodně štěstí! 😉
