# Witaj w tym tekście wyjaśnie ci pisanie w html zapraszam
Ważne rzeczy które napisalem są oznaczone # ale radze przeczytać całość zeby zrozumieć pisanie w języku html
zały tem tekst jest wyjaśnieniem na czyniki pierwsze pliku pod nazwą div.html

# F&Q

jak zacząć pisać?
pisanie w html nie jest ani trudne ani łatwe i właśnie w tym tekście pokaże ci wiedze którą się nauczyłem
na początek polecam pobrac jakiś program do edycji kodu
polecam visual studio code, note pad ++

jak nazwać naszą strone?
w naszym kodzie w linijce 6 mamy napisany kod <title>tytuł</title.
title to po angielsku tytuł więc możemy wywnioskować że chodzi w tym kodzie o tytuł
czyli każemy przeglądarce nazwać tą strone w dany sposób
tylko gdzie napisać tem tytuł. Tytuł piszemy pomiędzy kodem title
 
oco chodzi z head i body?
spójrzmy na to jak na człowieka
czyli to co mamy w głowie tego nie widzimy ale tam się rozpoczynają każde rozkazy do całego ciała czyli

w sekcji head dajemy znać przeglądarce naprzykład jak ma się nazywać strona 

w sekcji body wpisujemy cały kod który ma zobaczyć klient który wejdzie na naszą strone czyli naprzykład
tekst który tam przygotowaliśmy

czy strona będzie odrazu dostępna dla każdego?
nie będzie. Będziemy tylko wtedy mogli ją włączyć przez pliki lokalne ale w późniejszym czasie można kupić maszyne i domene.

dlaczego wpisujemy w sekcji head jedną dziwny kod?
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
tem kod daje znać przeglądarce edge lub inych przeglądarkach pisanych na IE żeby poprawnie wyświetliło twoją strone 
u klientów którzy kożystają z przeglądarki microsoftu

# okej mam nadzieje że na większość pytań odpowiedziałem to teraz przejdzmy do części pisania

<a href="link"></a>
a to inaczej hiperłącze czyli klikasz na to i cie przenosi do linka który został wpisany 
Pewnie się spytasz po co te znaki < na początku i > na końcu i jeszcze po co </a>
< to jest początek wierszu każdy wiersz tak zaczynamy w html a kończymy > żeby przeglądarka się domyśliła żeby skończyć w danym miejscu koniec linijki
po co na końcu musi byc taki sam znak co na początku tylko z / 
/ oznacza zakończenie danej rzeczy naprzykład hiperłącza

<div></div>
divy służą do budowania elementów strony www bez takich elementów byśmy osiągneli tylko tekst na naszej stronie
czemu po div jest id i w cudzysłowiu jakieś słowo?
id oznacza nazwe danego diva, po co piszemy id?
po to piszemy żeby łatwiej edytować w css tego diva 
co to znaczy align?
align to jest kod do dawania tesktu w ją chcemy strone
możemy ją dać w prawą strone lewą i wyśrodkować
żeby to zrobić musimy w środku diva wpisać align="strona"
wtedy nam się wszystko wyśrodkuje
naszą strone internetową można napisać w 2 sposoby żeby to się dobrze prezentowało na tabelach:
można napisac na divach i na tabelach
divy + nie czeba pisać bardzo długiego kodu + można go łatwo edytowac w css
tabele - bardzo dużo kodu który musimy napisać - ciężko go edytować w css

co to css?
css w rozwinięciu oznacza Kaskadowe arkusze stylów
czyli edytor wyglądu
w css możemy naprzykład zrobić customową czcionke na stronie 
czy można napisać css odrazu w pliku html?
można dla takiej operacji używamy w sekcji head wiersza <style>
w środku teko kodu nie piszemy jak w html tylko jak w css 
przykład mamy pokazany w kodzie div.html
  
Jak moge powiększyć czcionke?
żeby powiększyć czcionke musimy wpisać koc <h(liczba od 1 do 5)></h[liczba]>
po co dawać po h liczbe?
liczba oznacza jak ma być powiększony tekst najmniej to 5 a najwięcej to 1

Jak można miec customową czcionke w naszej stronie?
wchodzimy na stronie google fonts i tam sobie szukamy potem tam wyszukujemy sobie czcionke
ja wybrałem sobie czcionke Josefin Sans
szukamy odpowiedniego rozmiaru ja wziołem 300
klikamy select this style i po prawej wyskakuje nam panel 
w nim kopiujemy pierwszy kod i wklejamy go do sekcji head
a pod spodem mamy 2 kod on nam będzie potrzebny do dodania go w stronie jak i 1

# Teraz przechodzimy do sekcji jak to napisałem

na początku zrobiłem jednego diva w którym pomieszcze reszte divów i nazwałem go "container"
jak już zrobimy danego diva to przechodzimy do sekcji style
tam wpisujemy #container i otwieramy nawiasy {}
pamiędzy tymi nawiasami wpisujemy kod
naprzykład chcemy mieć szare tło
to pomiędzy nawiasami wpisujemy
background color ( kolor w moim przypadku będzie to szary to wspisuje gray)
i naprzykład mamy dodaną customową czcionke 
żeby uzyskać czcionke na całej stronie wpisujemy w sekcji head 1 kod który skopiowaliśmy z google fonts
i potem w sekcji container pod bacground color wpisujemy kod który był pod spodem kodu który skopiowaliśmy do sekcji head

pod divem container zrobiłem kolejnego diva który się nazywa logo
po między tym divem wpisałem co ma być w logo czyli dałem powiększony tekst i tam wpisałem swoje logo
teraz przechodzimy do sekcji style
tam został utworzony kod #logo
tam mamy określone wytyczne jak powienien wyglądać te logo
teraz wytłumacze co robi każdy kod
background color - dodaje kolor który ma być w tym divie
color - kolor tekstu jaki ma tam być ja dałem biały bo miałem czarne tło
width - szerokość naszego diva
min-height - minimalna wysokość naszego diva
padding - odstęp od naszego tekstu
okej czyli wytumaczyłem wam co każdy z tego kodu robi więc przejdzmy do kolejnego diva

następnym divem będzie nav
nav to inaczej panel po lewej stronie
tem div w samym html dodaje nam nowy kod
który się nazywa <br>
<br> to inaczej nowa linijka bo jak piszemy strony to piszmy na różne systemy operacyjne
a naprzykład windows odczytuje inaczej konic linijki niż linux
więdz temu zostało tak zrobione że br to koniec linijki
ale dobra tak pozatym to nic nowego nie jest
oczywiście robimy to samo w style co z divem logo ale tam mamy jedną nową rzecz
float: (kierunek: left right); - tem kod oznacza przyklejenie się do danego kierunku który tam napisaliśmy

kolejny div to jest div content
najważnieszy div to w nim właśnie napiszemy główne rzeczy które chcemy żeby klient je zobaczył
tem div to jest jakby środek strony
poznajemy tam nowy kod pod nazwą
<img - tem kod to jest wyświetlenie zdjęcia na naszej stronie
czemu tam jest napisane src?
src czyli jak się nazywa te zdjęcie
jak jest w jakimś folderze to musimy w cudzysłowiu wpisać całą ścieżke do tego zdjęcia a jak jest w tym samym folderze co nasza praca to wpisujemy 
tylko nazwe w moim przypadku to jest sadgunie.png
czyli poprawnie by to wyglądało
<img src="(plik zdjęcia z napisaną końcówką naprzykład .jpg, .png)">
ale i też tam mamy hiper łącze
hiper łącza czyli linki już potrafimy zrobić więc pomine tem szczegół
dodajemy taki sam kod do style co do reszty ale tam usuwamy min-hight
czemu? bo chyba nie chcemy żeby nasz tekst jak jest zaduży żeby przechodził przez inne divy albo ba żeby go nie było pokaanego na ekranie

następnym divem jest ad
tem div to kolejny panel ale po prawej stronie
div piszemy jak div nav

i ostani div czyli footer
footer inaczej to stópka 
stópki używamy na dole naszej strony
tez piszemy tam wszystko tak samo oprócz jednej rzeczy
nie piszemy wtedy w style float: left; bo jak byśmy tak napisali to byśmy mieli po lewej stronie stopke a my ją chcemy na dole
temu wtedy zamiast float wpisujemy tam clear: float; żeby usunąćw od tego diva żeby nie pojawiał się po lewo

po tym wszystkim zamykamy naszego wielkiego diva container i też html i body

# w tym tekście opowiedziałem ci na czyniki pierwsze każdy kod
mogą być błedy pisowni bo kończe to pisać o 4:30

Więc życze ci miłem przygody z językiem html

