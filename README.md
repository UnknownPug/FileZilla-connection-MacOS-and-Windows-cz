# FileZilla connection pro MacOS a Windows v rámci předmětu B6B39ZWA

## Autor: Dmitrij Rastvorov

## Tento popis slouží studentům k připojení k serveru wa.toad.cz pomocí aplikaci FileZilla na počítačích Mac a Windows.

## Obsah

### [Instalace na macOS](#macOS)

### [Instalace na Windows](#Windows)

### [Video na YouTube](#youtube)

### [DŮLEŽITÉ KROKY při používání aplikace FileZilla v budoucnu](#impFileZilla)

-- -- --

<a name="macOS"><h2>Instalace na macOS (Program pracuje s čipem M1)</h2></a>

1) Nejprve se připojte k serveru pomocí příkazu `ssh username@wa.toad.cz`. Dále, pokud se objeví **Are you sure you want to continue connecting (yes/no/[fingerprintl)?** napište **yes** a stiskněte Enter. 

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/1a59235c7242b0b46ba4d5dbfcb599d3/1__ssh_username_wa.toad.cz.png)

### (username - Vaše přihlašovací jméno na ČVUT)

### (password - Vaše uživatelské heslo na ČVUT)

2) V novém okně prohlížeče zadejte do vyhledávacího pole `http://wa.toad.cz/~username/` , kde se zobrazí chyba 404 s popisem (nebo 403 Forbidden).

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/b7784bf3285bf16b95f86f47da3f3b77/2__403.png)

### • Po tomto kroku nainstalujte program FileZilla:

3) Přejděte na tento odkaz: `https://filezilla-project.org/download.php?platform=osx` .

4) Klikněte na **Download FileZilla Client** a poté si stáhněte standardní verzi programu FileZilla **(nikdy ne manuální nebo profesionální verzi)**.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/891e75b8ae45eea55f9a121407678f2c/3__FileZilla.png)
![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/dd5130111172bd6c47ecccf20f77b41c/4__FileZilla_download.png)

5) Stáhněte si aplikaci, přejděte do složky **Downloads**, otevřete archiv a přeneste aplikaci do složky **Applications**.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/d06059873530c569569e0797e4287679/5__Move_to_Applications.png)

6) Spusťte FileZillu a udělte ji oprávnění v případě, že si to program vyžádá.

7) V levém horním poli **Host** napište adresu, kterou budeme používat v tomto předmětu: `sftp://wa.toad.cz`. Poté do pole **Username** napište přihlašovací jméno ČVUT a do pole **Password** napište Vaše uživatelské heslo ČVUT. Po vyplnění všech tří sloupců klikněte na tlačítko **Quickconnect**.

(Pokud se Vaše složka nezobrazuje, klikněte znovu na Quickconnect a program Vaši složku zobrazí)

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/bf9139b28f6b9ef0fcd6f891202bcd50/6__Quickconnect.png)
    
8) Potvrďte připojení. Poté se na pravé straně zobrazí složka s Vaším přihlašovacím jménem.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/2d0a98e05e333fe20e8719aa1a8f4416/7__OK.png)
![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/8c945da0190ed8d72cb496b0c7c85269/7_5__Connected.png)

<a name="macOS9To14">9.</a> Otevřete tuto složku a vytvořte v ní složku `www/01` kliknutím pravým tlačítkem myši na složku s uživatelským jménem a výběrem možnosti **Create directory** (můžete to také udělat postupně, na začátku vytvořit složku `www` a poté složku `01`).

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/3cd6d34eb19c215a9eab78213c8b372d/8__New_directory.png)
![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/9b909a1bd43679bcf7fa51fa143a5164/9__Created_new_directory.png)

10) Otevřete terminál a přejděte do složky 01 (`cd www/01` nebo `cd www` a pak `cd 01`), když už jste na serveru.

11) Uvnitř složky 01 vytvořte soubor **index.html** (`touch index.html`) a poté se vraťte do FileZilly. 

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/fd8e1f5fd96f12479fbba0903d490d02/10__Creating_html.png)

12) V aplikaci FileZilla klikněte na tlačítko Aktualizovat v horní části lišty a aktualizujte soubory.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/b7dc62e3f18b913fd1d260323a2cec6b/11__Updating.png)

13) Otevřete složku 01, klikněte pravým tlačítkem myši na index.html a vyberte možnost **View/Edit**.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/b0b4131e7882d8ee9826f0c2e7b7fcef/12__Editing_html.png)

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

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/16f0d1ac0d80ac92810826dbd7d68fb4/13__Commit.png)

18) Otevřete stránku serveru wa.toad.cz a znovu ji načtěte **(Cmd + R)**. Pak se zobrazí text, který byl napsán v index.html, nebo se zobrazí složka 01, kde se nachází soubor index.html. Pokud se vrátíme na stránku, uvidíme složku 01, kde se nachází soubor index.html.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/31773f103734f67d0e5392d867b3b8ad/15__wa.toad.cz_result__1.png)
![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/05a042cd9bb187fdce8e719a5a3a1cb2/15__wa.toad.cz_result__2.png)

19) Pokud otevřeme terminál a zadáme `telnet wa.toad.cz 80`, napíšeme `GET / HTTP/1.0` a **dvakrát stiskneme Enter**, vidíme, že spojení skutečně existuje a že vše funguje!

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/8b56d02c96002ca3bdcad013b2ae0895/16__telnet.png)
-- -- --

<a name="Windows"><h2>Instalace na Windows</h2></a>

1) Nejprve nainstalujte **terminál Ubuntu** (odkaz ke stažení z oficiálních stránek: `https://apps.microsoft.com/store/detail/ubuntu/9PDXGNCFSCZV`).

2) Poté otevřete Ubuntu a do terminálu zadejte příkaz `ssh username@wa.toad.cz`. Dále potvrďte připojení **Are you sure you want to continue connecting (yes/no/[fingerprintl)?** napište **yes** a stiskněte Enter.

### (username - Vaše přihlašovací jméno na ČVUT)

### (password - Vaše uživatelské heslo na ČVUT)

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/d76b73844358c37853fad090faad6501/1__Open_Ubuntu_terminal__verify.png)

3) Přejděte na webovou stránku **FileZilla**: `https://filezilla-project.org/download.php?platform=win64`, klikněte na **Download FileZilla Client** a vyberte ke stažení standardní verzi programu FileZilla (nikdy ne manuální nebo profesionální verzi).

4) Otevřete aplikaci a projděte procesem instalace.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/ddca425499064d392b018bca79717d10/2__Download_FileZilla.png)

5) Aplikace vyzve k instalaci prohlížeče, před kliknutím na tlačítko Next si přečtěte popis. 

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/b8e035b1da7e6e1a227d940aab3cc539/3__Decline_browser_download.png)
 
6) Povolte přístup všem uživatelům tohoto počítače.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/e28fef9c263a44b783d99170e07203c5/4__Giving_permition_to_users.png)

7) Vyberte **Desktop Icon**, chcete-li zobrazit zástupce na pracovní ploše. 

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/92c9338fed18edef42a14f15877fceec/5__Setting_Desktop_Icon.png)

8) Vyberte cestu pro instalaci aplikace. 

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/2ee200092b24b7540e65e8d0adc23f63/6__Choosing_Disk_Folder.png)

9) Po stažení klikněte na tlačítko **Finish**. Spustí se aplikace FileZilla.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/237011176786711ce5ddb910c0580691/7__Starting_FileZilla.png)

10) V levém horním poli Host napište adresu, kterou budeme používat v tomto předmětu: sftp://wa.toad.cz. Poté do pole Username napište přihlašovací jméno ČVUT a do pole Password napište Vaše uživatelské heslo ČVUT. Po vyplnění všech tří sloupců klikněte na tlačítko Quickconnect.

11) Poté se zobrazí okno s žádostí o uložení zadávaných údajů, abyste je nemuseli zadávat znovu. Vyberte Vámi preferovanou možnost a stiskněte tlačítko **OK**.

#### IMPORTANT: Pokud vyberete možnost "Neukládat hesla", bude k dispozici alternativní možnost připojení, jak je uvedeno v kroku 3 [(DŮLEŽITÉ KROKY při používání aplikace FileZilla v budoucnu)](#windowsAlternative).

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/1ab71ecc4bf926fb3dfa131dc8a8128b/8__Save_Not_save_password.png)

12) Potvrďte připojení. Stiskněte tlačítko **OK**.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/f556205ec19ddbc62a7a025ede6d6f77/9__Giving_permition_to_connect.png)

##### 13. Postupujte podle bodů popsaných při instalaci aplikace FileZilla v systému macOS [(kroky 9-14)](#macOS9To14)

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/fc2bbb6a9ef60084a1ab7fc5a2a970e8/10__Setting_IDE__1.png)

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/780b2e8c329997bdae703be60d077b87/11__Setting_IDE__2.png)

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

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/4c2a7ec4b322fe843b7a0ffdf791d534/12__Output.png)

-- -- --
<a name="impFileZilla"><h2>DŮLEŽITÉ KROKY při používání aplikace FileZilla v budoucnu</h2></a>

#### 1) Při dlouhodobém používání aplikaci FileZilla, budeme soubory spouštět kliknutím pravým tlačítkem myši na soubor a výběrem možnosti Zobrazit/Upravit (View/Edit).

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/b0b4131e7882d8ee9826f0c2e7b7fcef/12__Editing_html.png)

#### 2) Při nahrávání semestrálního projektu na server wa.toad.cz je možné nahrávat z lokálního počítače. Za tímto účelem vyhledejte složku s projektem v levém okně a přeneste ji na server, jak je uvedeno na obrázku:

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/9b92db5cb603e64234264a4a71c0148e/13_Next_usage.png)

#### <a name="windowsAlternative">3)</a> Pro další připojení není třeba zadávat **Host, Username** a **Password**. Klikněte na šipku vedle položky **Quickconnect** a vyberte **svůj Host**. Dále je třeba zadat heslo a kliknout na tlačítko **OK**, poté je třeba potvrdit připojení a objeví se naše složka se soubory.

![[]](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/01e13f297ddc5a76b6a8354c8b14ac04/0__Mac_Add.png)

-- -- --
<a name="youtube"><h2>Níže naleznete videonávod pro instalaci a práci s FileZillou v počítači Mac po jednotlivých krocích:</h2></a>

[![Watch the video](https://gitlab.fel.cvut.cz/rastvdmy/filezilla-connection-pro-macos-a-windows/-/wikis/uploads/e92941fbcf205273821e1f1be714cb45/YouTube_video.png)](https://www.youtube.com/watch?v=rX1lpdObLOQ)

-- -- --
#### To je ode mě všechno! Doufám, že Vám tento popis pomůže pochopit tuto aplikaci!

#### Hodně štěstí! 😉
