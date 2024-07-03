<img align="center" src="img/kabezera2024.jpg">

# Zibersegurtasuna 2023-2024
**Tknikako Zibersegurtasun lan taldearen 2023 - 2024 kurtsoko memoria**

## Aurkibidea<img align="center" src="img/lerroa.png">

1. [Aurkezpena:](#1aurkezpena)
   - 1.1 [Lan Taldea:](#11-lan-taldea)
2. [2024ko zifrak:](#22024ko-zifrak)
3. [Lan ildoak:](#3lan-ildoak)
   - 3.1 [Proiektuak:](#31-proiektuak)
      - 3.1.0 Cyber-Lehia
      - 3.1.1 Erd/Def CTF azpiegitura:
      - 3.1.2 Erd/Def CTFrako ariketak (Zerbitzuak):
      - 3.1.3 Erd/Def CTFrako bistaratze sistemak:
         - 3.1.3.1 Markagailua
         - 3.1.3.2 Argiztapena
   - 3.2 [Pilotuak:](#32-pilotuak)
      - 3.2.1 Phishing
      - 3.2.2 Vishing
      - 3.2.3 Hack the box
      - 3.2.4 Pentesting 
   - 3.3 [Ikastaroak:](#33-ikastaroak)
      - 3.3.1 Kontzientziazio kanpañak: Phishing-Vishing
      - 3.3.2 Komunikazio industrial ez seguruei erasotzeko tailer praktikoa
      - 3.3.3 Sare industrialen segmentazio tailer praktikoa
      - 3.3.4 Web Garapen Segurua
      - 3.3.5 "Zibersegurtasuneko araudia irakaslearen ikuspuntutik". Webinar (Ruth Sala)
   - 3.4 [Sortutako edukiak:](#34sortutako-edukiak)
   - 3.5 [Zentruetako proiektuak:](#35zentruetako-proiektuak)
      - 3.5.1 Cyber car
      - 3.5.2 OT Erronkak
4. [Harremanak eta Komunikazioa:](#4harremanak-eta-komunikazioa)
   - 4.1 [Ekintzailetza Jardunaldiak:](#41-ekintzailetza)
---------------------------------------------------------------------------------------------------------------------------------------------
## 1.Aurkezpena:<img align="center" src="img/lerroa.png">
2023-24 ikasturtean zehar **Tknikako Zibersegurtasun** lantaldean jorratu diren edukiak agertzen dira jarraian. Edukiak zerrendatzeaz gain, erabilitako fitxategi edo sorturiko materialetara iristeko estekak ere badaude. 
### 1.1 Lan Taldea:
Kurtso honetan lan taldea osatu duten partaideak izan dira:

   - Garikoitz Etxeberria 
   - Paulino Insausti
   - Urko Zuñiga
   - Xabat Zabala
   - Ibai Peña

## 2.2024ko zifrak:<img align="center" src="img/lerroa.png">
<img align="left" src="img/ZIFRAK.png">  
Aurten 100. ikaslea izan dugu geure CyberRange-an. Ikasle guzti guztiek gomendatzen dute esperientzia. 


## 3.Lan ildoak:<img align="center" src="img/lerroa.png">
### 3.1 Proiektuak:
3.1.0 Cyber-Lehia
#### 3.1.0 Erd/Def CTF-a:
  - ##### Kokapena

Aurreko ikasturtean CyberRangea kontsolidatu ondoren, erasorako edo ikerketarako gaitasunez gain, defentsarako eta hutsuneak zuzentzeko gaitasunak ere eskatzen dituen CTF plataforma bat martxan jartzeari ekin diogu ikasturte honetan. CyberRangea orain arte Jeopardy motako CTF-a izan da, eta aurten eraso/defentsa motakoa menperatu eta erabiltzeko gaitasuna lortzea zen helburua.

Mota honetako plataformak dagoeneko existitzen direnez, lehenik State-of-the-art nolakoa zen begiratu dugu. Garatutako opensource aukera anitz zeudela ikustean, horietan oinarritzea egoki ikusi dugu, zehazki Friedrich-Alexander University Erlangen-Nürnberg (FAU) unibertsitateko segurtasun taldearen (FAUST) bi garapenetan. Bi garapen hauek urtero erabiliak dira Unibertsitateak burutzen duen ER/DEF nazioarteko proban.

Garapen hauei eraldaketa eta gehikuntzak egin dizkiogu guk behar genuenera hurbiltzeko. Gure garapenaren lehen bertsioa honela errepresentatu daiteke:

<img align="center" src="img/eskema-sinplea.png">

Azpiegitura hau <a href="https://cyberlehia.fpeuskadi.eus/"> Cyberlehia 2024</a>-n erabili da, Euskadiko Lanbide Heziketarako lehen zibersegurtasun txapelketan, finaleko jardunaldian, txapelketako talde irabazlea erabakitzeko.

Hemen txapelketaren laburpen bideoa.

<p align="center"><a href="https://www.youtube.com/watch?v=2AtvKaG9ahY"> <img align="center" src="img/Screenshot_CyberLehia.png" width=50% height=50%> </a></p>

#### 3.1.1 Erd/Def CTF azpiegitura:
  - ##### Kokapena

FAUST Taldearen erabilitako bi proiektuak hauek dira:

      - Gameserverra: https://github.com/fausecteam/ctf-gameserver
      - Ansible bidezko instalazioa: https://github.com/fausecteam/ctf-gameserver-ansible

Lan horietatik abiatuta, moldaketa garrantzitsuak egin behar izan dira, guk behar genuen eredua gauzatzeko, taldeen azpigitura osoa plataforman bertan gehitzea besteak beste. Terraform bidez Proxmoxen (AWS bertsio ere bidean) hedatzen den ERD/DEF CTF plataforma izan da emaitza.

<img align="center" src="img/gameserver-proxmox.png">

#### 3.1.2 Erd/Def CTFrako ariketak (Zerbitzuak):

Behin azpiegitura erabilgarri genuela, lehen proba batzuk sortu genituen hau probatzeko eta gero azpiegitura CyberLehiako finalean erabiliko genuela erabaki zenean hasierako horiei gehitutakoekin 6 ariketa edo zerbitzu sortu genituen; hona hemen zerbitzu horietako baten azalpentxoa, adibide modura: 
   Zertan datza? ssh zerbitzu bat dugu martxan. Baimenduta dauka erabiltzaile/pasahitza bitartez kautotzea; gainera, erabiltzaile baten pasahitzak ez die gomendio minimoei eusten. 
   Ahuleziaren saikapena: OWASP-i dagokionez, hainbat taldetan multzokatu genezake, baina nagusia A07:2021-Identification and Authentication Failures kontsideratu liteke. 
   Erasoa: hiztegi-eraso bat gauzatu daiteke hydra bezalako tresna bat erabilita; hiztegirik izan ezean, eraso gordina bideratu daiteke. 
   Defentsa: desgaitu egin behar da erabiltzaile/pasahitza bitartez kautotzeko aukera; hori egin ostean, erabiltzaileak kriptografia asimetrikoaren bidez kautotu beharko dira, giltz bat erabilita.

#### 3.1.3 Erd/Def CTFrako bistaratze sistemak:

MQTT brokerrera iritsitako gertaerak irakurri eta hauen bitartez gertatzen ari dena modu erakargarri batean erakustea da bistaratze sistemen helburua. Modu honetako 2 garapen burutu dira:

##### 3.1.3.1 Markagailua

   GameServerrak badu markagailu bat, baina informazio gehiegi ematen du modu konplexu batean. Garapen berri honen bitartez, automatikoki eguneratzen den markagailu sinple eta erakargarria lortu nahi izan da, eraso ezberdinei buruzko momentuko informazioa ere ematen duena.
   
   <p align="center"><img src="img/CyberLehia Bistaratzea.png" width=50% height=50%></p>

##### 3.1.3.2 Argiztapena

   Ikusgarritasuna handitu asmoz, led argiz osatutako sistema bat jarri da martxan, talde bakoitzarentzat 2 argi dituelarik. CTF-an gertaturiko egoera ezberdinen aurrean modu ezberdinean jokatuko dute argiek. Saioa hastean eta amaitzean, argi guztiek kolorezko patroi bat egingo dute. Eraso bat dagoenean, talde erasotzailearen argiek kolore berdea hartuko dute, talde erasotuarenek aldiz, gorria. 
   
   <p align="center"><img align="center" src="img/CyberLehia Argiztapena.jpg" width=50% height=50%></p>

### 3.2 Pilotuak:
#### 3.2.1 Phishing:
 - ##### Kokapena

Phishingaren inguruko kontzientziazio kanpañak landu asmoz, iaz Smartphense tresna testeatu ondoren, aurtengo ikasturtean **Gophish** software librearen pilotu bat jorratu da. Github-etik deskargatu daiteke, <a href="https://github.com/gophish/gophish/releases"> esteka </a> honetatik. Kontzientziazio kanpañaren lehendabiziko fasean, Tknikako instalazioetan egin da lehen lanketa. Bertako langileen epostetara, email desberdinak bidali dira igorle faltsu batetatik, webgune faltsu batetarako estekarekin. Tknikan eginiko lanketaren balorazio positiboa egin ostean, pilotu hau Lanbide Heziketako ikastetxeetara zabaltzea erabaki zen. Ikastetxe desberdinei proposamena egin ondoren, azkenean **Zubiri Manteo IES, Uni Eibar, Izarraitz LH** eta **Iurretako LHI** ikastetxeetan jorratu zen kanpañaren bigarren fasea. Bertako irakasleen emailetara, mezu desberdinak bidali zirelarik. 
Jarraitutako urratsen **GIDA** beheko dokumentuan klikatuta ikusiko duzue:
<p align="center"> <a href="docs/Gophish_gida.pdf" class="image fit"><img src="img/GOPHISH_GIDAimg.jpg" alt="" width="25%" height="25%"></a></p>

Tknikan jorraturiko pilotuaren exekuzioa azaltzen duen **bideo** laburra:

<p align="center"><a href="https://youtu.be/WRu7IkI5Jq4"> <img align="center" src="img/bideo_shot.jpg" width=50% height=50%> </a></p>

#### 3.2.2 Vishing:
 - ##### Kokapena
Iaz eta aurten phishing pilotuen lanketan ibili ondoren, **VISHING** kanpaña bat burutu da Tknikako instalazioetan eraso mota hauek izan dezaketen inpaktua lankideen artean jorratzeko. Dei telefoniko bidez eginiko kontzientziazio kanpaña bat izan da, eta beronen bueltan erabili diren teknikak eta tresnak gertuagotik ezagutzeko lagundu digu.
Kanpaña hau, <a href="https://www.bedisruptive.com/"> BeDisruptive </a> enpresari eskatu zaio eta jarraian duzuen dokumentuan aurkituko dituzue kanpaña honen inguruko xehetasunak:

<p align="center"> <a href="docs/TKNIKA_VISHING_github.pdf" class="image fit"><img src="img/Tknika_vishing.jpg" alt="" width="50%" height="50%"></a></p>

#### 3.2.3 Hack the box:
<p align="center"><img src="img/htb.png"></p>

 - ##### Kokapena
**Hack The Box** plataforma, Lanbide Heziketako Zibersegurtasun espezialitatean erabiltzearen ikuspegitik, **Txurdinagako LH** ikastetxean ikasturte osoan frogatu den tresna bat izan da. HTB-ek eskeintzen dituen laborategi desberdinak frogatu eta ikasleekin lan egiteko orduan ematen dituen abantailak testeatu dira. Horrez gain, ikasturte honetan <a href="https://cyberlehia.fpeuskadi.eus/es/">**CyberLehian**</a>, etab ere erabili da eta bertatik jasotako esperientzia eta ateratako ondorioak partekatu, hausnartu eta beste aukera posibleei buruz lanketa egin asmoz, jardunaldi bat antolatzea izan da helburua. Jardunaldi honetan, ondorioak partekatzeaz gain, HTB-ko erronka bat elkarlanean landu da.

#### 3.2.4 Pentesting Pilotua Iurreta LHI:
<p align="center"><img width="50%" height="50%" src="img/pentesting-iurreta.jpg"></p>

 - ##### Kokapena
Tknikako zibersegurtasun alorretik Pentesting-eko pilotu bat jarri da martxan bigarren urtez jarraian. Pilotu honetan, zibersegurtasunaren espezializazioa egin duen ikasle batek, sektoreko enpresa baten laguntzarekin (JakinCode), zentro baten (Iurreta LHI) segurtasun auditoretza egiten du.   

Iurreta LHI zentroan eginiko lana partekatu asmoz, Webinar bat egin da Ekainean. Webinarraren helburua lortutako emaitzak aurkeztea eta esperientzia prozesuan interesa dutenekin partekatzea izan da.

### 3.3 Ikastaroak:
#### 3.3.1 Kontzientziazio kanpañak: Phishing-Vishing
<p align="center"><img width="35%" height="35%" src="img/phishing.jpg"></p>

Tknikan landuriko pilotuen ildoa jarraituz, bertan bilduriko esperientzia partekatu asmoz, ikastaro bat eman da **Phishing/Vishing** tekniken kontzientziazioa landuz. Kontzientziazio kanpañak burutzeko metodologiak eta tresnak landu dira bertan. Kontzientziazio kanpañak burutzeko urratsetan sakondu da: 
 - 1.Informazioa topatu (**OSINT**)
 - 2.Eszenatokiak sortu (**SMTP zerbitzariak, GOPHISH ingurunea**)
 - 3.**Kanpañak** diseinatu.
 - 4.**Vishing** nola?

Ikastaroan erabilitako materiala, Githubek errepositorio honetan duzue ikusgai.
[Dokumentazio Gida](KONTZIENTZIAZIOA)
#### 3.3.2 Komunikazio industrial ez seguruei erasotzeko tailer praktikoa
<a href="https://drive.google.com/drive/folders/1RZYG0BOWVfZFVcp6iwW28reY7XXHdKKw"> Edukiak </a>
<p align="center"><img src="img/OTkurtsorako-irudia1.jpg"></p>

Lantegi praktiko honetan, industria-sistemak komunikazio ez-seguruen eta izan dezaketen arriskuen ikuspegitik aztertu dira. Sareko ekipoak ezagutzeko tresnak erabili dira (Nmap), komunikazioetan sortzen den trafikoa aztertu da (Wireshark) eta PLC sistemak "erasotzeko" hainbat teknika erabili dira. 22/23 ikasturtean, industria-kontroleko sistemetan zibersegurtasuna kontuan izateko ikastaroa eman zen. Bertan, sistema industrialak konfiguratzeko orduan zibersegurtasunaren ikuspegitik kontuan hartu beharreko atalak jorratu ziren. Sarrerako prestakuntzaren osagarri gisa, tailer praktiko batzuk planteatu dira, ikastaro horretan ikusitako hainbat atal modu praktikoan lantzeko. Lehen tailerrean industria-komunikazioen gabeziak eta seguruak ez diren industria-sistemetan gerta daitezkeen erasoak aztertu dira.Partaide kopurua: 14 irakasle.

#### 3.3.3 Sare industrialen segmentazio tailer praktikoa
<a href="https://drive.google.com/drive/folders/12DOwM5J-GNARspU_LaM2hmHa2buSFuWq"> Edukiak </a>
<p align="center"><img width="50%" height="50%"img src="img/red-ot.jpg"></p>
Lantegi praktiko honetan sare industrialak segmentatuta izatearen garrantzia aztertuko da. Segmentazio egoki bati esker, ekoizpen-sarean eragina izan dezaketen eta zabaldu ez daitezkeen segurtasun-intzidenteak arindu ditzakegu. Era berean, IEC 62443 segurtasun-araudiak IT/OT sareak bereizita izatera behartzen du. Siemens familiako gailuak, Scalance 615 suhesiak eta Switch 208,408 gailuak erabiliko dira konfigurazioak egiteko. 23/24 ikasturtean, industria-kontroleko sistemetan zibersegurtasuna kontuan izateko ikastaroa eman zen. Bertan, sistema industrialak konfiguratzeko orduan zibersegurtasunaren ikuspegitik kontuan hartu beharreko atalak jorratu ziren. Sarrerako prestakuntzaren osagarri gisa, tailer praktiko batzuk planteatuko dira, ikastaro horretan ikusitako hainbat atal modu praktikoan lantzeko.Partaide kopurua: 16 irakasle.

#### 3.3.4 Web Garapen Segurua
<p align="center"><img width="50%" height="50%" src="img/garapen-segurua.jpg"></p>

Prestakuntza honen helburua, segurtasuna web garapenaren bizi-zikloaren parte izan dadin, beharrezkoa den ezagutza zabaltzea izan da. Segurtasuna oso espazio zabaleko gaia den arren, prestakuntza honetan web inguruneetan (aplikazioak eta APIak) ematen diren ahulgune ohikoenetan enfokatuko gara. Aipatutako ahulguneak ekiditeko jarraitu beharreko praktika onak ezagutzera eman dira.
Prestakuntza honetan, web-inguruneetan modu seguruan garatzeko kontuan hartu beharreko alderdiak aztertu dira. Horretarako, OWASP erakundeak jasotako ahultasunen top 10ean oinarritu da. OWASP (Open Web Application Security Project) irabazi asmorik gabeko erakunde bat da, eta bere helburua softwarearen segurtasuna hobetzean datza.
“Juice Shop” open source aplikazioa erabili da ikasitakoa praktikan jartzeko. Aplikazio hau segurtasun arazoez beteta dago eta gamifikazio osagai bat du. Ahuleziak ustiatzen diren heinean, lorpenak desblokeatzen dira eta parte-hartzaileak sailkatzen dituen ranking bat sortzen da. Ahuleziak aurkitu ahala, erlazionatutako kodea aztertuko da eta funtzionalitatea modu seguruan garatzeko jarraitu beharreko irizpideak azaltzen dira.

#### 3.3.5 "Zibersegurtasuneko araudia irakaslearen ikuspuntutik". Webinar (Ruth Sala)
Irakaslearen ikuspuntutik Zibersegurtasun Araudiari buruzko webinarra burutu da. Webinar hau <a href="https://www.linkedin.com/in/ruthsala/?originalSubdomain=es">Ruth Sala</a> abokatuak eta gaian adituak eman du, eta bertan zibersegurtasunaren atalean burutzen diren hainbat praktiken legalitatearen inguruan egon daitezkeen galderak erantzun zituen bertan.
<p align="center"><a href="https://www.youtube.com/live/JUFNl8AUOO0"> <img align="center" src="img/screenshot_rsala.jpg" width=50% height=50%> </a></p>

Galdera/erantzunak lantzen dituen <a href="docs/Normativa de ciberseguridad desde el punto de vista del docente - Ruth Sala.pdf" class="image fit">dokumentua deskargatu dezakezu HEMEN.</a>
 

###  3.4Sortutako edukiak:

###  3.5Zentruetako proiektuak:
#### 3.5.1 Cyber car
#### 3.5.2 OT Erronkak
## 4.Harremanak eta Komunikazioa:
#### 4.1 Ekintzailetza Jardunaldiak:
