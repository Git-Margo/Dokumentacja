<h2><b>Spis treści</b></h2><br>
<b><a href="#k1">1. System walki</a></b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k11">1.1. Moduł walk</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k12">1.2. Rozpoczynanie walk między graczami</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k13">1.3. Rozpoczynanie walk z NPC</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k14">1.4. Akcje gracza w walce</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k15">1.5. Stan nieprzytomności postaci</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k16">1.6. Doświadczenie</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k17">1.7. Punkty Honoru</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k18">1.8. Zdobycze</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k19">1.9. Przedmioty używane podczas walki</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k110">1.10. Wyczerpanie</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k111">1.11. Mechaniki światów specjalnych</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k112">1.12. Listy gończe</a><br>
<b><a href="#k2">2. System tur</a></b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k21">2.1. Kolejność wykonywania tur</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k22">2.2. Czas oczekiwania na akcję gracza</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k23">2.3. Umiejętności</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k24">2.4. Mistrzostwo walk</a><br>
<b><a href="#k3">3. Statystyki postaci w walce</a></b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k31">3.1. Statystyki gracza</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k32">3.2. Budowa ekwipunku</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k33">3.3. System ulepszania przedmiotów</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k34">3.4. System przekuwania przedmiotów</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k35">3.5. Statystyki NPC</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k36">3.6. Efekty umiejętności w walkach PvP</a><br>
<b><a href="#k4">4. Atrakcje oparte na walce</a></b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k41">4.1. Otchłań</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k42">4.2. Krwawa Łaźnia</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k43">4.3. Krwawa Kopalnia</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k44">4.4. Walki przeciw potworom</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#k45">4.5. Niuanse związane z elitami II</a><br>
<br><br>
<hr><a name="k1"></a><h2><b>1. System walki</b></h2><a name="k11"></a><b><h3>1.1. Moduł walk</h3></b><br>
Moduł walk jest elementem gry uruchamianym po wykonaniu akcji zaatakowania postaci. Składa się z ramki w pełni zajmującej przestrzeń całego modułu świata gry (obejmując mapę i jej obiekty). <br>
<br>
Poniżej zaprezentowano pozycję elementów modułu walki oraz elementów z nim związanych:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Pole walki, na którym znajdują się postaci graczy oraz NPC.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Okno logu walki, mieszczące się zawsze w centrum modułu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. Lista predykcji tur, umieszczona w prawej części okna logu walki. <b><a href="https://www.youtube.com/shorts/xdyX2LrOGr0">Krótki film</a></b> omawiający działanie okna predykcji tur oraz logu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. Licznik czasu trwania tury wraz z paskiem progresu, umieszczonym w górnej części okna logu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5. Licznik czasu wszystkich tur, umieszczony w lewej części okna logu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6. Przycisk poddania walki mieszczący się w lewym górnym rogu okna logu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7. Zestaw przycisków, mieszczących się w prawym górnym roku okna logu walki, służących do zmiany wielkości okna logu walki oraz otwarcua osobnych okien logu walki lub okna predykcji. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8. Przycisk zmiany celu, mieszczący się w lewym dolnym rogu okna logu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;9. Przycisk włączenia/wyłączenia szybkiej walki, mieszczący się w prawym dolnym rogu okna logu walki oraz pojawiający się w jego miejsce przycisk zamknięcia ramki walki po zakończeniu starcia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;10. Leżące w głównym interfejsie czerwone koło symbolizujące poziom życia postaci, którego wartość procentowa zmienia się w czasie przeprowadzania walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;11. Poboczny (górny) pasek umiejętności, mieszczącego się w dolnej części okna logu walki, który można odblokować poprzez wcześniejsze rozmieszczenie pozycji umiejętności aktywnych w module umiejętności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;12. Głównego (dolny) paska umiejętności, należący do głównego interfejsu, pojawiający się w miejscu paska szybkiego dostępu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;13. Umiejętności przypiętych do pasków umiejętności. Wyszarzonych umiejętności nie można użyć z faktu czasu odnowienia (symbolizowane cyfrą określającą pozostałą liczbę tur do odnowienia umiejętności), braku zasobów (energii lub many), braku spełnienia wymagań (nieprawidłowy typ obrażeń w broni) lub nieprawidłowa pozycja postaci w stosunku do pozycji celu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;14. Otwarte dodatkowe okno logu walki, którego pozycję oraz wielkość można personalizować.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;15. Animacja skrzyżowanych mieczy nad wizerunkiem postaci, informująca o tym, która postać w danym momencie wykonuje swoją akcję.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;16. Tooltip pojawiający się po najechaniu myszą na postać, wyświetlający najważniejsze informacje o jej stanie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;17. Nagrobki postaci, które zostały pokonane. Nagrobków nie można obrać za cel ataku oraz umiejętności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;18. Paski zdrowia (wszystkich postaci), paski energii oraz many (sojuszników), paski ładowania umiejętności specjalnej (potworów) oraz ikony działania efektów na postać (takich jak spowolnienie) nad wizerunkami postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;19. Ekwipunek postaci będący częścią głównego interfejsu. Zawiera wszystkie przedmioty, składające się na bieżące statystyki, z którymi postać rozpoczęła walkę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20. Numer wybranego zestawu do walk będący częścią głównego interfejsu. Zawiera informację o tym, z którym zestawem do walk postać rozpoczęła walkę (na zestaw do walk składa się ekwipunek oraz umiejętności).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21. Spis statystyk postaci będący częścią głównego interfejsu. Statystyki zawierają informacje o postaci, z którymi rozpoczynała ona walkę i nie zmieniają się wraz ze zmianą stanu postaci podczas przeprowadzania pojedynku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;22. Torba z przedmiotami mieszcząca się w głównym interfejsie. Podczas walki można korzystać z niektórych rzadkich przedmiotów, które zmieniają przebieg walki.<br>
<br>
<center><img src="https://mwc.garmory-cdn.cloud/documentation/dokumentacja_walk_01.png" width="1000"></center><br>
<br>
Niektóre elementy mogą w głównym interfejsie gry zostać odpięte, co pozwala na spersonalizowanie ułożenia okna walki. Operacji tej można dokonać poprzez kliknięcie w odpowiednią pineskę znajdującą się w prawym narożniku okna logu walki. Wśród obsługiwanych tą mechaniką elementów nich znajdują się:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Okno z listą predykcji tur.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Okno z logiem walki.<br>
<br>
Obsługiwane są dwa typy walk:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Walka graczy z potworami niezależnymi (NPC).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Walka graczy z graczami.<br>
<br>
Obsługiwane są następujące tryby walki:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Walka turowa, podczas której gracz sam wykonuje ruch. Uruchamiana jest poprzez kliknięcie lewym przyciskiem myszy na NPC lub poprzez akcję <i>Atakuj</i> wykonaną na graczu. Z walki turowej można przejść do walki szybkiej w dowolnym momencie. <b><a href="https://youtube.com/shorts/PpqNpBU4PDo">Krótki film</a></b> obrazujący działanie przełączania między szybką walką a turową.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Walka szybka, podczas której akcje postaci są wykonywane automatycznie (atak oraz Krok do przodu). Gracz ma możliwość wpływać na typ i kolejność wykonywanych akcji poprzez system <i>Mistrzostwa walki</i> mieszczący się w module umiejętności. Tryb ten uruchamiany jest w momencie włączenia opcji <i>Auto</i> podczas walki. Jeżeli w walce uczestniczy więcej niż jeden gracz, wybór przez jednego z nich opcji <i>Auto</i> nie wpłynie w żaden sposób na resztę graczy. Postacie niezależne zawsze dokonują akcji automatycznie. Z walki szybkiej można przejść do walki turowej w dowolnym momencie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Walka automatyczna, której działanie jest identyczne jak walki szybkiej, jednak jest ona obliczana sekwencyjnie przez silnik bez oczekiwania na akcję któregokolwiek gracza biorącego udział w walce. Włączenie tego trybu sprawia więc, że po chwili gracze są powiadamiani o jej wyniku. Walka automatyczna uruchamiana jest w momencie kliknięcia prawym przyciskiem myszy na NPC (przez samotnego gracza lub dowódcę drużyny) albo poprzez włączenie opcji <i>Auto dla drużyny</i> przez dowódcę drużyny tylko w walce z NPC. <br>
W przypadku pojedynku z grupą przeciwników, priorytet wybierania celu podczas walki automatycznej jest następujący:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• priorytet z perspektywy graczy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Przeciwnik, który został zaatakowany w momencie rozpoczynania walki nawet jeżeli jest potrzeba zmiany pozycji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Przeciwnik z najniższym poziomem, który może zostać zaatakowany przez atakującego bez konieczności zmiany jego pozycji. Jeżeli istnieje konieczność zmiany pozycji, by zaatakować któregokolwiek przeciwnika, wykonywany jest <i>Krok do przodu</i>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. Postać, której szablon został dodany najpóźniej do świata gry (z najwyższym ID).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. Postać, która została dodana najpóźniej do świata gry (z najwyższym ID).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• priorytet z perspektywy potwora:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0. Tworzona jest lista walczących graczy, zależna od kolejności dodania postaci do drużyny. Osoba, która pierwotnie utworzyła drużynę jest pierwsza na liście, a postać dodana jako ostatnia jest na ostatnim miejscu. Zmiana dowódcy nie powoduje zmiany kolejności listy. W momencie ataku potwora, postać atakująca go zamienia się miejscem na liście z dowódcą drużyny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Przeciwnik z najniższym poziomem, który może zostać zaatakowany przez atakującego bez konieczności zmiany jego pozycji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Przeciwnik, który rozpoczął walkę, jeżeli nie istnieje konieczność zmiany pozycji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. Postać, która jest najniżej na liście walczących graczy, którą można zaatakować bez zmiany pozycji. Jeżeli żadna postać nie może zostać zaatakowana bez zmiany pozycji, wykonywany jest <i>Krok do przodu</i>.<br>
<br>
Po stoczonej walce i zamknięciu logu, można raz jeszcze przejrzeć log walki poprzez użycie specjalnego skrótu klawiszowego (domyślnie <b>H</b>) lub wpisanie komendy <code>show battle</code> do konsoli (skrót klawiszowy <b>~</b>).<br>
<br>
<br><br>
<a name="k12"></a><b><h3>1.2. Rozpoczynanie walk między graczami</h3></b><br>
O możliwości podjęcia walk między graczami decyduje typ mapy oraz <i>Zgoda na PvP</i> ustawiona przez gracza. Walka rozpoczyna się w momencie, gdy jeden gracz wykona na drugim operację atakowania (poprzez przycisk w interfejsie lub skrót klawiszowy), zostanie spełniony warunek <i>Zgody na PvP</i> (w przypadku, gdy typ mapy pozwala na atakowanie graczy z pominięciem zgody, warunek nie jest sprawdzany), warunek odległości od gracza (promień o kształcie prostokąta wynosi 2 kratki) oraz warunek najkrótszej ścieżki (najkrótsza droga między postaciami, po uwzględnieniu kolizji, musi być odpowiednio krótko).<br>
<b><a href="https://youtube.com/shorts/2Wo37gtfJEg">Krótki film</a></b> obrazujący operację rozpoczynania walki.<br>
<br>
<i>Zgoda na PvP</i> jest specjalną opcją symbolizowaną przez tarczę (lub skrzyżowane miecze) mieszczącą się pod ekwipunkiem postaci gracza. Jest uwzględniana pod uwagę w przypadku wykonywania akcji <i>Ataku</i> na graczach znajdujących się na mapie <i>Żółtej</i> (PvP warunkowe) lub <i>Pomarańczowej</i> (arenie). Ustawienie tarczy oznacza brak zgody na walki między graczami, w konsekwencji żaden gracz nie będzie mógł zaatakować tej postaci. Ustawienie skrzyżowanych mieczy oznacza wyrażenie zgody na atak postaci.<br>
<br>
Typy mapy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zielona - gracze nie mogą na niej walczyć między sobą.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Żółta - gracze mogą rozpoczynać walkę z graczami wyrażającymi <i>Zgodę na PvP</i>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Czerwona - gracze mogą rozpoczynać walkę z każdym, <i>Zgoda na PvP</i> nie wpływa na możliwość rozpoczynania walk.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pomarańczowa - arena, gracze mogą rozpoczynać walkę z graczami wyrażającymi <i>Zgodę na PvP</i>, ponadto czas odrodzenia na arenie wynosi 10 sekund.<br>
<br>
Dodatkowe mechaniki mapy:<lu><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mapa żółta zamienia się na czerwoną w godzinach 0:00 - 5:59.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mapa czerwona zamienia się w żółtą w godzinach 8:00 - 10:59.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieją serwery, gdzie wszystkie domyślnie czerwone mapy, są zielone (Majuna).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieją serwery, gdzie wszystkie domyślnie żółte mapy są czerwone (Brutal, Perkun).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieje ustawienie mapy (bezwarunkowy tryb PvP), sprawiające, że jest ona czerwona niezależnie od serwera i pory dnia (wykorzystywane w Krwawej Łaźni i Krwawej Kopalni).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zapisanie się do kolejki systemu Otchłani sprawia, że do walki może dojść niezależnie od typu mapy, na jakiej obecna jest postać gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieje dodatkowa mechanika zdobycia mapy wykorzystywana na <a href="https://pomoc.margonem.pl/index/view,267">światach PvP</a>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieje opcja, która jest nałożona na niektóre mapy, wyłączająca przewagę poziomową między graczem a przeciwnikiem (innym graczem lub potworem niezależnym). Na takich mapach bonusy legendarne postaci z poziomem przewyższającym 300 działają tak, jakby miała ona poziom 300. Ponadto walki na niej nie powodują kumulowania punktów w ramach systemu listów gończych.<br>
<br>
Dodatkowa blokada rozpoczęcia walki:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Gracze nie mogą podejmować walki z postacią aktualnie uczestniczącą w walce.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Gracz nie może zaatakować członka swojej drużyny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pierwsze wejście postaci na czerwoną mapę uniemożliwia wszystkim graczom atakowanie jej przez 5 sekund lub do momentu wykonania akcji w grze. Ochrona odnawia się po 1 minucie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zalogowanie do gry uniemożliwia graczom atakowanie postaci przez 5 sekund  lub do momentu wykonania akcji w grze. Działa również na czerwonej mapie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Rozmowa postaci z NPC uniemożliwia chwilowe atakowanie jej przez graczy - czas ten zależny jest od długości dialogu. Istnieje specjalne ustawienie dla NPC, z którym rozmowa zupełnie uniemożliwia zaatakowanie postaci przez innych graczy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Skorzystanie przez postać z akcji <i>Ucieczki z walki</i>, uniemożliwia jej zaatakowanie innej postaci przez 5 sekund.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przejście gracza w tryb nieaktywności oraz rozwiązywanie zagadki nie wpływają na możliwość podjęcia walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Postacie z rangami MG, SMG i Admin mogą atakować inne postacie niezależnie od typu mapy.<br>
<b><a href="https://youtube.com/shorts/TrQMvpeuvUc">Krótki film</a></b> opisujący mechanikę blokady rozpoczęcia walki.<br>
<br>
<br><br>
<a name="k13"></a><b><h3>1.3. Rozpoczynanie walk z NPC</h3></b><br>
Moment rozpoczęcia walki:<br>
Walka rozpoczynana jest natychmiast, jeżeli przy atakowanym NPC znajduje się tylko jeden gracz bądź kilku graczy z tej samej drużyny. Gracze z drużyny uczestniczą w walce jeżeli znajdują się w mniejszej odległości niż promień 22 kratek (liczony również po przekątnych).<br>
Jeżeli, w odległości do 7 kratek od atakowanego NPC o randze powyżej Elita, znajduje się przynajmniej dwóch graczy z różnych drużyn, którzy nie uczestniczą w walce i nie tkwią w stanie nieaktywności, to moment rozpoczęcia walki opóźniony jest o około 4 sekundy na skutek losowania. Czas ten liczony jest od momentu kliknięcia w przycisk ataku przez pierwszego gracza. Przez ten okres inni gracze mają możliwość wzięcia udziału w losowaniu walki z NPC - nad graczami chcącymi rozpocząć walkę pojawia się wtedy ikona miecza ze znakiem zapytania.<br>
Szczegóły losowania:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Każdy gracz ma równe szanse na rozpoczęcie ataku, losowanie nikogo nie faworyzuje.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Szybkość kliknięcia oraz ilość kliknięć na przycisk rozpoczęcia ataku nie mają żadnego znaczenia podczas losowania.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli wielu graczy z tej samej drużyny wykona akcję ataku, to nie zwiększa to ich szans na rozpoczęcie walki - w losowaniu bierze udział cała drużyna jako jednostka.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli atakowana jest grupa NPC, to tryb losowania włącza się, jeżeli przy dowolnym członku grupy NPC znajduje się przynajmniej dwóch graczy z różnych drużyn.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tryb losowania włącza się tylko wtedy, gdy tuż przy atakowanym NPC lub grupie NPC znajdują się inni gracze z innej drużyny. Z tej zasady wyłączone są potwory rangi Elita, dla których promień, wewnątrzn którego musi być obecny inny gracz w celu rozpoczęcia losowania, wynosi 7 kratek.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tryb losowania został wprowadzony po to, by każdy gracz, niezależnie od szybkości łącza i klikania, miał taką samą szansę na rozpoczęcie ataku; system ten eliminuje także proste boty oraz rozszerzenia do gry wątpliwej legalności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Gracz rozpoczynający losowanie, nie może zostać dodany do grupy.<br>
<br>
<br><br>
<a name="k14"></a><b><h3>1.4. Akcje gracza w walce</h3></b><br>
W walce gracz jest przyporządkowany do jednej z dwóch drużyn, walczących przeciw sobie. Drużyna jest tworzona przed walką przez <b>dowódcę</b>, czyli gracza, który zaprasza wszystkich pozostałych graczy do swojej grupy. Dowódca ma możliwość rozwiązać drużynę (wyrzucić z niej wszystkich członków) oraz przekazać dowództwo innemu graczowi. Drużyna składa się z maksymalne 10 graczy. Finalnie w walce może zatem uczestniczyć do 20 graczy, po 10 graczy w każdej z drużyn.<br>
<br>
Walka jest podzielona na tury, czyli akcje graczy. Tura jest 15-sekundowym oczekiwaniem na akcję gracza. W przypadku, gdy gracz nie dokona żadnej akcji, zostaje wykonany automatyczny ruch.<br>
<br>
Gracz ma do dyspozycji wykonanie następujących akcji:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Akcja domyślna - podstawowy atak oraz krok do przodu<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Rzucenie umiejętności - akcje, których gracz musi się nauczyć poprzez moduł umiejętności<br>
<br>
Każda akcja wymaga dobrania odpowiedniego celu poprzez kliknięcie odpowiedniego obiektu myszą lub selekcję za pomocą przycisku TAB. Gracz może wybrać następujące cele:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Siebie samego - w celu poruszenia się (<i>Krok do przodu</i>) lub użycia umiejętności wyzwalającej efekt na postać lub wszystkich członków drużyny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Sojusznika - w celu wzmocnienia sojusznika lub wielu sojuszników.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przeciwnika - w celu zaatakowania przeciwnika lub użycia umiejętności ofensywnych nakładających efekt na przeciwnika lub wielu przeciwników.<br>
<br>
Akcje mogą posiadać warunki do spełnienia w celu ich wykonania. Dostępne są następujące wymagania:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pozycja - np: krok do przodu można wykonać wyłącznie będąc w pozycji pierwszej, natomiast umiejętności dystansowe wyłącznie jak jest się na pozycji drugiej lub trzeciej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Typ przedmiotu - np: niektóre umiejętności można wykonać posiadając tylko broń dwuręczną, umiejętności profesji dystansowych wymagają posiadania strzały.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Typ obrażeń - np: niektóre umiejętności można wykonać posiadając tylko broń zadającą obrażenia od głębokiej rany.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zasób - umiejętności mogą wymagać posiadania określonej puli punktów energii lub many.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Moment trwania walki - umiejętności mogą posiadać czas odnowienia pomiędzy kolejnymi użyciami wyrażony w turach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Cel - niektóre umiejętności posiadające efekt prowokacji (<code>shout</code>) zmuszają pozostałych graczy do atakowania określonego celu. Podczas tego efektu można brać za cel samego siebie.<br>
<br>
Na początku walki każdy gracz jest przyporządkowany do jednej z trzech dostępnych pozycji. Pozycja zależy od profesji gracza:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pozycja pierwsza - postacie posiadające broń do walki w zwarciu (zamiennie nazwane bronią białą) lub nieposiadające wyekwipowanej żadnej broni. W domyślnym ekwipunku są to profesje: wojownik, tancerz ostrzy, paladyn.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pozycja druga - postacie posiadające różdżkę. W Domyślnym ekwipunku jest to mag.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pozycja trzecia - postacie posiadające broń dystansową oraz wyekwipowany kołczan lub strzały (w przypadku, gdy strzały się skończą, postać musi podejść do przeciwnika w celu wykonania ataku). W Domyślnym ekwipunku są to profesje: tropiciel, łowca. <br>
<br>
Pozycje druga oraz trzecia należą do dystansowych. Postacie na tych pozycjach, w przypadku posiadania założonej broni, mogą wykonywać dowolne akcje bez konieczności spełnienia wymagań pozycji.<br>
Postacie z pozycji pierwszej muszą zmniejszyć odległość od obiektu w celu wykonania na nim akcji takich jak atak. Odległość zmniejsza się poprzez wykonanie kroku do przodu w liczbie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 1 krok do przodu w celu atakowania graczy na pozycji drugiej (podejście do pozycji drugiej)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 2 kroki do przodu w celu atakowania graczy na pozycji trzeciej (podejście do pozycji trzeciej)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 0 kroków do przodu w celu atakowania graczy na pozycji pierwszej, również tych którzy wykonali wcześniej krok do przodu<br>
<br>
Gracz może maksymalnie podejść do pozycji trzeciej. Nie ma jednak limitu wykonanych kroków w przód ze względu na mechanikę <code>pushback</code>, która odrzuca gracza od pozycji postaci wykonującej ten efekt (źródłem tego efektu są ciosy specjalne potworów).<br>
<br>
Walka kończy się w momencie kiedy wszyscy członkowie jednej z drużyn zostaną pokonani. Postać gracza umiera kiedy jej punkty zdrowia spadną poniżej 1. W przypadku zwycięstwa, gracz wraca do świata gry z pulą zdrowia, którą dysponował na końcu trwania walki. W przypadku, gdy gracz poległ, odradza się w miejscu zależnym od ustawień mapy, na której jego postać umarła (najbliższe miasto, przedsionek mapy z kolosem lub lokacja związana z zadaniem). Do momentu odrodzenia, postać pozostaje w stanie nieprzytomności.<br>
<br>
<br><br>
<a name="k15"></a><b><h3>1.5. Stan nieprzytomności</h3></b><br>
Postać jest w stanie nieprzytomności, do momentu odrodzenia, przez czas:<br>
<code>∀ lvl &lt;= 20 { T<sub>resp</sub> [s] = 10 + lvl }</code><br>
<code>∀ lvl &gt; 20 { T<sub>resp</sub> [s] = 30 + 10 * (lvl - 20) }</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom gracza (lub poziom operacyjny w przypadku postaci z poziomem wyższym niż 300).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>T<sub>resp</sub></code> - czas odrodzenia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja matematyczna minimum.<br>
<br>
Na czas trwania stanu nieprzytomności mają wpływ:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ustawienia mapy - mapa może mieć nadaną specjalną opcję <i>Krótki respawn gracza</i>, skracającą powrót do zdrowia postaci do 15 sekund.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Talizman - przedmioty o klasie <i>Talizman</i> mogą posiadać atrybut <code>respred</code>, który skraca czas trwania nieprzytomności o część zdefiniowaną w statystyce przedmiotu. Najwyższa wartość redukcji czasu nieprzytomności w talizmanie może wynosić 99%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwoje orzeźwienia - przedmioty konsumpcyjne z atrybutem <code>revive</code> są możliwe do użycia w czasie trwania stanu nieprzytomności i skracają czas powrotu do zdrowia o zdefiniowaną wartość. Czas powrotu do zdrowia nie może być jednak krótszy niż 10 sekund. Jeżeli postać jest nieprzytomna dłużej niż 60 minut lub krócej niż 30 sekund, nie może używać zwoju skracającego czas trwania stanu nieprzytomności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ustawienia serwera - na świecie zawodowym po śmierci postaci czas powrotu do zdrowia wynosi 10 minut.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zabicia postaci przez MG lub Zarządcę świata prywatnego - osoby z odpowiednimi uprawnieniami mogą zabić postać na czas nieokreślony.<br>
<br>
Występująca w talizmanach statystyka <i>Przyspieszenie wracania do zdrowia</i> (<code>respred</code>) skraca, o zadany procent, czas nieprzytomności o największą oferowaną spośród wszystkich aktywowanych z postacią talizmanów wartość tej statystyki.<br>
Wartość <code>respred</code> jest ustawiana manualnie zgodnie z poniższą funkcją:<br>
<code>respred [%] = round(1000 * (1 - (2 * (target_resp_time + 30) * arctan(lvl / 31 - 0.55) / PI) / (10 * lvl - 170))) / 10</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;respred - redukcja czasu powrotu do zdrowia (dozwolona jest wyłącznie liczba całkowita).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;target_resp_time - docelowy czas stanu nieprzytomności podawany w sekundach, zależny od jakości przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;arctan - funkcja arcus tangens.<br>
<br>
Czas odrodzenia można obliczyć z następującego wzoru:<br>
<code>T<sub>resp_final</sub>  [s] = T<sub>resp</sub> * (100% - respred[%])</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;T<sub>resp_final</sub> - finalny czas powrotu do zdrowia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;T<sub>resp</sub> - czas powrotu do zdrowia bez talizmanu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;respred - redukcja czasu powrotu do zdrowia (dozwolona jest wyłącznie liczba całkowita).<br>
<br>
Docelowy czas stanu nieprzytomności jest ustalony przez projektantów jako oczekiwany czas, jaki postać ma powracać do zdrowia w zależności od posiadanego przez nią talizmanu posiadającego poziom równy poziomowi tej postaci. Z faktu liniowości funkcji czasu powrotu do zdrowia, oczekiwany czas odrodzenia może znacznie przewyższać faktyczny czas spędzony w stanie nieprzytomności. Jest więc to granica wyznaczona dość ogólnie dla postaci z wyższym poziomem, dla którego przypada dłuższy czas odrodzenia niż ustalona wartość docelowa.<br>
Zakładając poziom talizmanu równy poziomowi postaci, docelowy czas stanu nieprzytomności wynosi:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 420 sekund - dla posiadaczy talizmanów pospolitych<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 340 sekund - dla posiadaczy talizmanów unikatowych<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 250 sekund - dla posiadaczy talizmanów heroicznych<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 210 sekund - dla posiadaczy talizmanów ulepszonych<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 170 sekund - dla posiadaczy talizmanów legendarnych<br>
<br>
<br><br>
<a name="k16"></a><b><h3>1.6. Doświadczenie</h3></b><br>
Pokonanie potwora lub grupy potworów i zakończenie walki nagradza każdą żywą postać punktami doświadczenia. Doświadczenie służy do <i>Awansu poziomowego</i> postaci. Nowo utworzona postać posiada poziom pierwszy i może osiągnąć maksymalnie poziom 500.<br>
<br>
<h3><span class="color-blue">Poziom postaci</span></h3>W celu awansu poziomowego, należy posiadać określoną pulę punktów doświadczenia. Liczba punktów doświadczenia, konieczna do skumulowania w celu awansu na określony poziom, obliczana jest ze wzoru:<br>
<code>exp_amount<sub>lvl</sub> = (lvl - 1)^4 + 10</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>exp_amount<sub>lvl</sub></code> - liczba punktów doświadczenia wymaganych do awansu na poziom <code>lvl</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom, na który postać ma awansować.<br>
<br>
<b>Poziom postaci wpływa na</b>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dostępność możliwych do wykonania zadań.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Możliwość przedostania się na niektóre zablokowane poziomowo mapy oraz przebywanie na nich.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Możliwość skorzystania z przedmiotów i założenia ekwipunku na postać.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Widoczność niektórych potworów (herosi).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziom przeciwników, którzy tkwią w trybie dostosowania swojego poziomu do poziomu gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziom przedmiotów, które tkwią w trybie dostosowania swojego poziomu do poziomu gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Możliwość zniszczenia przedmiotu wylosowanego z NPC.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Możliwość zmniejszenia liczby losowań po pokonaniu NPC.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Liczbę możliwych do rozdania punktów umiejętności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Niektóre statystyki postaci, takie jak atrybuty bazowe (zręczność, siła, intelekt), cios krytyczny i życie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowy przyrost niektórych atrybutów (cios krytyczny, siła ciosu krytycznego, unik, obniżanie uniku, blok) w walce z graczami i potworami, gdy przewaga poziomowa między przeciwnikami jest wysoka.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Otrzymywanie karnych punktów za zabijanie graczy z dużo niższym poziomem, mogących nałożyć na gracza <i>List gończy</i>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przyrost doświadczenia z mikstur i zadań z nagrodą zależną od poziomu gracza<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dostęp do niektórych modułów interfejsu (umiejętności, rzemiosło).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Możliwość wykonania niektórych akcji podczas rozgrywki (całowanie, wysyłanie wiadomości prywatnych, wykup depozytu).<br>
<br>
<a name="oplvl"></a><br>
<b>Poziom przewyższający 300</b><br>
Postacie z poziomem przewyższający 300 są traktowani tak samo jak postacie z poziomem 300 pod względem następujących mechanik:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wzrost statystyk i atrybutów podstawowych za poziom - siła, zręczność, intelekt, życie oraz cios krytyczny (nie mylić ze wzrostem szansy na cios krytyczny z faktu przewagi poziomowej) nie rosną powyżej poziomu 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Obliczanie statystyk zależnych od poziomu przeciwnika (blok, unik) - jeżeli przeciwnik ma poziom przewyższający 300, szansa na blok i unik postaci przyjmującej od niego cios, jest obliczana względem poziomu 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Możliwość znalezienia herosa - herosi powyżej poziomu 250 nie posiadają górnego limitu poziomowego postaci, do którego można ich znaleźć na mapie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Liczba dostępnych umiejętności - punkty umiejętności nie rosną powyżej poziomu 300, zatem maksymalna ich liczba wynosi 276.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Siła postaci podczas walk na Otchłani - postacie z poziomem wyższym od 300 są traktowane w kolejce wyszukiwania oraz podczas walki tak, jakby miały poziom 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększanie liczby losowań łupów po pokonaniu potwora - jeżeli w drużynie występują zarówno gracze z poziomem 300 jak i 500, nie następuje zredukowanie liczby losowań do jednego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zaliczanie progresów do wykonania zadań - gracz z poziomem 300 może zgrupować się z graczem z poziomem 500 w celu wspólnego zabicia potwora do zadania.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zaliczanie doświadczenia po pokonaniu potwora - w przypadku hipotetycznego istnienia potwora z poziomem 500, drużyna złożona z postaci z poziomem 300 oraz 499, otrzyma doświadczenie po jego zabiciu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ustalanie poziomu błogosławieństwa po jego założeniu - błogosławieństwo nie może przyjąć poziomu wyższego niż 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ustalanie poziomu przedmiotów ekwipowalnych ze statystyką <code>lvladjust</code> - przedmioty dostosowujące poziom na podstawie poziomu postaci, nie mogą przyjąć poziomu wyższego niż 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Otrzymywanie doświadczenia z przedmiotów ze statystyką <code>expadd</code> - przedmioty oferujące wielokrotność doświadczenia za pokonanie potwora o tym samym poziomie co postać, zawsze ustalają limit poziomu potwora, na podstawie którego obliczają doświadczenie, na poziom 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ustalanie poziomu potwora ze statystyką <code>autolvl</code> - potwory, których poziom dopasowuje się do poziomu postaci, nie mogą przyjąć poziomu wyższego niż 300.<br>
<br>
<b>Poziom operacyjny</b><br>
Na podstawie zmian związanych ze słabnięciem mechaniki przewagi poziomowej, każda postać z poziomem przewyższającym 300, otrzymała dodatkowy wskaźnik poziomowy - poziom operacyjny. Poziom postaci pełni jedynie funkcję wizualną, która odzwierciedla ilość doświadczenia, jaka zmagazynowana została na postaci, natomiast <b>poziom operacyjny jest parametrem wszystkich mechanik zależnych od poziomu postaci</b>. Oznacza to na przykład, że w celu obliczenia słabnięcia bonusu legendarnego, czasu trwania nieprzytomności lub przewagi poziomowej nad przeciwnikiem, należy wziąć pod uwagę poziom operacyjny, a nie poziom "standardowy" postaci.<br>
Poziom operacyjny widnieje w interfejsie gry jako druga liczba przy nazwie postaci, umiejscowiona po znaku pionowej linii: <code>|</code> .<br>
Poziom operacyjny postaci, która przekroczyła poziom 300, obliczany jest zgodnie z poniższym wzorem:<br>
<code>op_lvl = floor((0.88<sup>month</sup> * (exp_amount - 7992538811) + 7992538801)<sup>0.25</sup>) + 1</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>op_lvl</code> - poziom operacyjny postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>month</code> - liczba miesięcy, jaka upłynęła od daty 01.02.2025 r.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>exp_amounth</code> - liczba punktów doświadczenia zgromadzonych na postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja matematyczna podłoga.<br>
<br>
<a href="https://mwc.garmory-cdn.cloud/posts/tabela-poziomow-operacyjnych-pdf.pdf">Poziom operacyjny postaci może zmieniać się wraz z początkiem każdego miesiąca od dnia 03.03.2025 r. do dnia 01.03.2029 r. włącznie.</a><br>
Sposób czytania tabeli:<br>
1. Zlokalizuj dzień kalendarzowy, w którym zaszła ostatnia aktualizacja obliczania poziomu pozornego (kolumna).<br>
2. Zlokalizuj poziom operacyjny postaci jaki posiadasz (widoczny w interfejsie gry po znaku pionowej linii: <code>|</code> ).<br>
3. Możesz teraz sprawdzić, jaki poziom operacyjny będzie posiadała twoja postać w następnym miesiącu.<br>
<br>
<br>
<b>Przewaga poziomowa</b><br>
Gdy poziom postaci wykonującej cios (gracz lub NPC) jest wyższy od poziomu postaci odbierającej cios (gracz lub NPC) o 5, aktywuje się przewaga poziomowa, która wpływa na następujące statystyki:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększa lub zmniejsza szansę na cios krytyczny postaci wykonującej cios o:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>crit<sub>gain</sub> [%] = sign(lvl<sub>attack</sub> - lvl<sub>defence</sub>) * max(abs(lvl<sub>attack</sub> - lvl<sub>defence</sub>) - 5, 0) * 3</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>crit<sub>gain</sub></code> - przyrost szansy na cios krytyczny gracza (może być ujemny).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>attack</sub></code> - poziom postaci atakującej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>defence</sub></code> - poziom postaci atakowanej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sign</code> - funkcja znaku (wynikiem jest 1, 0 lub -1).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja maksimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>abs</code> - funkcja wartości bezwzględnej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększa lub zmniejsza siłę ciosu krytycznego fizycznego i magicznego postaci wykonującej cios o:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critval<sub>gain</sub> [%] = min(300 , sign(lvl<sub>attack</sub> - lvl<sub>defence</sub>) * max(abs(lvl<sub>attack</sub> - lvl<sub>defence</sub>) - 5, 0) * 10)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critval<sub>gain</sub></code> - przyrost siły ciosu krytycznego fizycznego oraz magicznego (może być ujemny).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>attack</sub></code> - poziom postaci atakującej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>defence</sub></code> - poziom postaci atakowanej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sign</code> - funkcja znaku (wynikiem jest 1, 0 lub -1).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja minimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja maksimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>abs</code> - funkcja wartości bezwzględnej.<br>
Mechanika przewagi poziomowej jest <b>wyłączona na światach posiadających blokadę przekroczenia trzysetnego poziomu postaci</b> przed wprowadzeniem poziomu operacyjnego do gry (dotyczy światów: Aether, Alcatraz, Aldous, Arkantes, Eternia, Fobos, Gordion, Hades, Lupus, Navis, Tempest, Valhalla oraz nowych światów powstałych po dniu 03.03.2025 r.).<br>
<br>
Istnieją mapy, które posiadają ustawiony parametr "wyłącz przewagę poziomową". Powoduje ona, że bonus za przewagę poziomową nie aktywuje się podczas walki.<br>
<br>
<br>
<br><br>
<h3><span class="color-blue">Pozyskiwanie doświadczenia</span></h3>Doświadczenie otrzymywać można jako nagrodę za wykonanie zadania (wartość predefiniowana) lub za pokonanie potwora.<br>
<br>
<b>Doświadczenie będące nagrodą za wykonanie zadania</b> ma zdefiniowaną przez projektanta wartość, ale może być zwiększane przez:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ustawienia świata (mnożnik od 1.0 do 5.0, świat <a href="https://pomoc.margonem.pl/index/view,268">Nerthus</a> posiada stały mnożnik 3.0).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Błogosławieństwa zwiększające doświadczenie z zadań (przedmiot z atrybutem <code>quest_expbon</code>).<br>
Doświadczenie może posiadać wartość:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Stałą.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zależną od poziomu gracza.<br>
<br>
<b>Doświadczenie pozyskiwane za zwycięstwo w walce</b> obliczane jest zgodnie z kolejnością:<br>
1. Pobranie wartości doświadczenia za zabicie każdego potwora z danym poziomem zgodnie ze wzorem:<br>
<code>experience = npc_lvl^1.80276 * (1 - 0.04 * max(0 , (player_lvl - npc_lvl))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>experience</code> - doświadczenie otrzymywane z potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>npc_lvl</code> - poziom potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>player_lvl</code> - poziom gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja matematyczna maksimum.<br>
2. Obliczenie bonusu za dużą utratę puli punktów zdrowia postaci:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-15% za utratę poniżej 5% puli zdrowia. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-10% za utratę poniżej 10% puli zdrowia. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-5% za utratę poniżej 15% puli zdrowia. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+0% za utratę poniżej 70% puli zdrowia. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+10% za utratę poniżej 80% puli zdrowia. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+20% za utratę poniżej 90% puli zdrowia. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+30% za utratę poniżej 99% puli zdrowia. <br>
3. Obliczenie bonusu za typ NPC:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 200% za walkę z elitą II lub elitą III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 1500% za walkę z herosem, kolosem lub tytanem.<br>
4. Obliczenie sumy doświadczenia za wszystkie pokonane potwory uwzględniając wszystkie powyższe bonusy.<br>
5. Uwzględnienie addytywnego bonusu do doświadczenia za walkę w grupie graczy.<br>
6. Uwzględnienie addytywnego bonusu do doświadczenia za walkę z grupą NPC.<br>
7. Uwzględnienie multiplikatywnego bonusu ustawień światów prywatnych lub wydarzeń okresowych.<br>
8. Uwzględnienie addytywnego bonusu za zdobycie mapy (tylko Perkun).<br>
9. Uwzględnienie multiplikatywnego bonusu współczynnika "fair", czyli redukcji doświadczenia, jeżeli w drużynie są poziomy graczy znacznie odbiegające od siebie.<br>
10. Uwzględnienie multiplikatywnego bonusu z rangi klanowej.<br>
11. Uwzględnienie addytywnego bonusu za zabicie gracza poszukiwanego listem gończym.<br>
12. Uwzględnienie multiplikatywnego bonusu do doświadczenia z przedmiotów ekwipowalnych i błogosławieństwa (bonusy są w tym kroku ze sobą sumowane).<br>
13. Podział doświadczenia przez liczbę członków w grupie.<br>
14. Sprawdzenie czy liczba punktów <b>Wyczerpania</b> gracza jest większa od zera, jeżeli nie, to postać nie otrzymuje doświadczenia.<br>
15. Przyznanie doświadczenia postaci.<br>
<br>
<b>Doświadczenie pozyskiwane za ukończenie zadania</b> obliczane jest zgodnie z kolejnością:<br>
1. Pobranie wartości doświadczenia za ukończenia zadania.<br>
2. Przemnożenie przez mnożnik serwerowy.<br>
3. Przemnożenie przez bonus klanowy.<br>
4. Przemnożenie przez bonus z błogosławieństwa.<br>
<br>
<br><br>
<b>Bonus do doświadczenia w grupie</b> graczy jest kompensacją podziału doświadczenia przyznawanego graczowi przez liczność grupy. Oblicza się go zgodnie ze wzorem:<br>
<code>experience_bonus [%] = 100% + <sup>G</sup>Σ<sub>n=1</sub>(9 + n)[%]</code><br>
gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>experience_bonus</code> - bonus do uzyskiwanego z walk doświadczenia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>G</code> - liczba członków grupy.<br>
<br>
<br><br>
<b>Kara do doświadczenia za przewagę poziomową</b> nad NPC:<br>
<code>experience_penalty [%] = max(0 , 4% * (lvl<sub>player</sub> - lvl<sub>NPC</sub>))</code><br>
gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>experience_penalty</code> - wartość procentowa, o którą zostaje obniżone pozyskiwane przez gracza doświadczenie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>player</sub></code> - poziom gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>NPC</sub></code> - poziom potwora.<br>
<br>
<br><br>
<b>Największy poziom gracza w grupie</b> umożliwiający pozyskiwanie doświadczenie z walk.<br>
Aby zdobywać doświadczenie z walk, między najniższym a najwyższym poziomowo graczem w grupie może być różnica wynosząca 40% poziomu gracza z najmniejszym poziomem powiększona o stałą wartość 4 (ale nie mniej niż 14 poziomów):<br>
<code>lvl<sub>ally_max</sub> = max( round( (1 + server_factor) * lvl<sub>ally_min</sub>) + 4, lvl<sub>ally_min</sub> + 14)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>ally_max</sub></code> - najwyższy poziom członka grupy. <b>Jeżeli wartość przekroczy 299, to maksymalny poziom członka drużyny zawsze wynosi 500</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>ally_min</sub></code> - najniższy poziom członka grupy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>min</sub></code> - najniższy poziom gracza w drużynie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>server_factor</code> - współczynnik serwerowy: 0.2 dla serwera publicznego, 0.4 dla serwera prywatnego oraz świata Nerthus.<br>
<br>
<br><br>
<b>Największy poziom gracza w grupie</b> zaliczający etapy w zadaniach.<br>
Aby zaliczać progresy zadań (na przykład zabicie potwora) będąc zgrupowany z innym graczem, między najsłabszą a najmocniejszą postacią w grupie może być różnica wynosząca 20% poziomu postaci z najmniejszym poziomem (ale nie mniej niż 10 poziomów). Aby drużynowe zabicie potwora zostało zaliczone, osoba wykonująca zadanie musi przeżyć walkę.<br>
<code>lvl<sub>ally_max</sub> = max( round( (1 + server_factor) * lvl<sub>ally_min</sub>) + 4, lvl<sub>ally_min</sub> + 14)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>ally_max</sub></code> - najwyższy poziom członka grupy. <b>Jeżeli wartość przekroczy 299, to maksymalny poziom członka drużyny zawsze wynosi 500</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>ally_min</sub></code> - najniższy poziom członka grupy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>min</sub></code> - najniższy poziom gracza w drużynie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>server_factor</code> - współczynnik serwerowy: 0.2 dla serwera publicznego, 0.4 dla serwera prywatnego oraz świata Nerthus.<br>
<br>
<br><br>
<b>Mikstury dodające doświadczenie</b> można pozyskać:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• ze skrzyń, które są dziennymi nagrodami za uczestnictwo w Otchłani.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• z Elit III na każdym poziomie trudności występujących podczas wydarzeń czasowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• z dodatkowych aktywności związanymi z wydarzeniami cyklicznymi.<br>
<br>
Typy mikstur dodających doświadczenie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowe doświadczenie równe zabitemu potworowi pomija dodatkowe mnożniki występujące podczas walki (liczba potworów w grupie, poziom zdrowia jaki pozostał po zakończonej walce).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty konsumpcyjne z atrybutem stałym <code>expadd=N</code>, dodające <code>N-</code>krotność doświadczenia za zabicie potwora na poziomie gracza używającego mikstury.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty konsumpcyjne z atrybutem zmiennym <code>expaddadjust=N</code>, który po zdobyciu przez postać mikstury, tworzy jej nową statystykę zmienną <code>expaddlvl=L,N</code>, dodającą po jej użyciu <code>N-</code>krotność doświadczenia za zabicie potwora na <code>L</code> poziomie.<br>
<br>
Właściwości mikstur dodających doświadczenie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mikstury dopasowują się do maksymalnie 300 poziomu. Gracz z poziomem przewyższającym 300, po użyciu mikstury, otrzymuje tyle doświadczenia jakby miał poziom 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Indywidualne ustawienia światów wpływają na zysk doświadczenia z mikstur (np: na świecie <a href="https://pomoc.margonem.pl/index/view,311">Brutal</a> postać otrzymuje 5 razy mniej doświadczenia).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Błogosławieństwa i przedmioty ekwipowalne z atrybutem <code>expbon</code> zwiększające doświadczenie za zabite potwory, nie wpływają na zysk doświadczenia z mikstur.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mikstur można używać tylko na mapach z wyłączonym trybem PvP (zielonych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mikstury zwiększają doświadczenie mimo braku posiadania punktów wyczerpania.<br>
<b><a href="https://www.youtube.com/shorts/ard0LGNaV8s">Krótki film</a></b> omawiający mechanikę mikstur przyznających doświadczenie.<br>
<br>
<h3><span class="color-blue">Cofanie doświadczenia</span></h3><b>Resetowanie doświadczenia</b> dla danego poziomu polega na ustawieniu postaci puli doświadczenia, która jest wymagana do awansu na poziom, który aktualnie posiada, bez żadnej nadwyżki. Po cofnięciu doświadczenia, pula doświadczenia wymaganego do awansu na następny poziom, wynosi 0%. <br>
Doświadczenie można zresetować poprzez wybranie odpowiedniej opcji dialogowej z postacią niezależną oferującą taką usługę - Sir Graunsheim w Przybytku Zakonu Białej Róży (Ratusz Karka-han). Zapłatę za cofnięcie doświadczenia można uiścić w złocie lub w Smoczych Łuskach.<br>
Koszt cofnięcia doświadczenia w Smoczych Łuskach wynosi 375 SŁ i rośnie o 75 SŁ za każdy kolejny reset doświadczenia (maksymalnie do 750 SŁ) oraz resetuje się do 375 SŁ, jeżeli postać awansuje na kolejny poziom podzielny przez 50.<br>
Koszt cofnięcia doświadczenia w złocie jest zależny od poziomu doświadczenia postaci i rośnie analogicznie jak koszt cofnięcia w Smoczych Łuskach.<br>
<b><a href="https://youtube.com/shorts/yyqNxdUhd5A">Krótki film</a></b> omawiający proces cofania doświadczenia.<br>
<br>
<br><br>
<a name="k17"></a><b><h3>1.7. Punkty Honoru</h3></b> <br>
W przeciwieństwie do walk z NPC, za zwycięstwo z graczem otrzymuje się Punkty Honoru. Stanowią one wskaźnik liczby stoczonych przez gracza pojedynków 1 vs 1 z pozytywnym wynikiem oraz są dodatkową walutą, którą można wymienić na przedmioty w specjalnych sklepach. Gracz pokonany traci Punkty Honoru ze swojej puli o równowartości liczby punktów, które zyskał zwycięzca (wartość skumulowanych Punktów Honoru nie może spaść poniżej zera). Źródła pozyskania Punktów Honoru są następujące:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zaatakowanie i pokonanie gracza maksymalnie 10 poziomów wyższego lub maksymalnie 2 poziomy niższego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zostanie zaatakowanym przez gracza maksymalnie 10 poziomów niższego lub maksymalnie 2 poziomy wyższego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wykonanie zadania lub części zadania, za którą przyznawane są w ramach nagrody Punkty Honoru - nie dotyczy świata <a href="https://pomoc.margonem.pl/index/view,311">Brutal</a>.<br>
<br>
Walka toczy się o Punkty Honoru gdy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• IP obu graczy jest różne.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Gracze nie należą do tego samego klanu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Obaj gracze mają powyżej 20 poziomu doświadczenia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przewaga poziomowa między graczami nie jest zbyt duża. Gracz atakujący może mieć maksymalnie 2 poziomy więcej i maksymalnie 10 poziomów mniej od gracza atakowanego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>player1</sub> - lvl<sub>player2</sub> &gt; 2</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>player2</sub> - lvl<sub>player1</sub> &gt; 10</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziom zdrowia graczy na początku walki jest większy bądź równy 85% bazowej puli zdrowia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp<sub>current</sub> / hp<sub>base</sub> &lt; 0.85</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Gracze nigdy nie walczyli ze sobą o Punkty Honoru.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Każdy z graczy od momentu ostatniej walki o Punkty Honoru stoczył więcej niż <code>N</code> pojedynków z innymi graczami.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie <code>N</code> to parametr wynoszący:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20, jeżeli poziom gracza jest niższy bądź równy 70<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;15, jeżeli poziom gracza jest niższy bądź równy 100<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;10, jeżeli poziom gracza jest wyższy niż 100<br>
<br>
Kolejność obliczania Punktów Honoru za walkę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Pobranie bazowych Punktów Honoru poprzez obliczenie średniej arytmetycznej z poziomów graczy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>PH<sub>base</sub> (lvl<sub>player1</sub>, lvl<sub>player2</sub>) = (lvl<sub>player1</sub> + lvl<sub>player2</sub>) / 2</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Uwzględnienie kary 33% za różną pozycję, jeżeli pozycje w walce profesji obu graczy nie należą do tego samej kategorii:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>PH = PH<sub>base</sub> * 0.66</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(wojownik/tancerz/paladyn - pozycja 1, mag - pozycja 2, tropiciel/łowca - pozycja 3)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. Uwzględnienie kary 50% za brak Punktów Honoru, jeżeli przegrany gracz ma mniej Punktów Honoru niż powinien utracić za przegraną walkę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>PH<sub>final</sub> = PH * 0.5</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. Przyznanie zwycięzcy <code>PH<sub>final</sub></code> oraz odebranie przegranemu <code>max(PH<sub>final</sub> , 0)</code>.<br>
<br>
<br><br>
<a name="k18"></a><b><h3>1.8. Zdobycze</h3></b><br>
Zakończenie walki z NPC może skutkować przyznaniem przedmiotu. Mechanizm ten dzieli się na moment losowania zdobyczy z puli przedmiotów danego potwora oraz na moment rozdzielania łupów między graczami.<br>
W przypadku, gdy co najmniej jedna zdobycz została wylosowana, wszystkim uczestnikom walki, którzy nie zamknęli okna walki przed jej zakończeniem, pojawia się okno łupów. Przyciskiem <code>ESC</code> można odrzucić wszystkie łupy zawarte w oknie.<br>
<b><a href="https://youtube.com/shorts/clXeA0GAfes">Krótki film</a></b> obalający zakorzenione mity związane z przydzielaniem łupów.<br>
<br>
<h3><span class="color-blue">Mechanizm losowania zdobyczy</span></h3><b>1. Sprawdzanie czy łup został zniszczony</b><br>
W przypadku, gdy żaden gracz nie przeżył walki, nie dochodzi do żadnego losowania.<br>
Dodatkowo wylosowany przedmiot jest niszczony w przypadku, gdy postać gracza przekroczy poziom:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 13 poziomów wyższy od poziomu potwora w przypadku gry na świecie publicznym<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• od 13 do 50 poziomów wyższy od poziomu potwora w zależności od ustawień świata prywatnego<br>
<br>
Przedmiot nie jest niszczony jeżeli szablon ma ustawiony parametr "Niezniszczalny", występujący u potworów eventowych, niektórych zwykłych potworów (głównie jeżeli posiadają przedmiot potrzebny do ukończenia zadania), herosów eventowych, kolosów eventowych oraz u postaci niezależnych z dialogiem.<br>
Potwory z poziomem wyższym bądź równym 250, mają zawsze niezniszczalny szablon zdobyczy.<br>
<br>
<b>2. Sprawdzanie typu potwora</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli losowanie przebiega dla łupu z szablonu, który ma ustawiony "Osobisty łup" (np: szablon zdobyczy Kolosów), każdy członek drużyny (niezależnie od tego czy przeżył walkę) uczestniczy w prywatnym gwarantowanym losowaniu. Łup trafia wyłącznie do gracza, któremu przysługuje losowanie. Nie można akceptować łupu z losowania należącego do innego gracza. Nie można odrzucić swojego łupu. Z puli przedmiotów odrzucane są te, które nie spełniają wymagań profesji gracza (stat <code>reqp</code>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli losowanie przebiega dla łupu z szablonu Elity II lub Herosa, następuje przejście do punktu trzeciego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli losowanie przebiega dla łupu z szablonu Tytana, następuje przejście do punktu czwartego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• W pozostałych przypadkach zachodzi tylko jedno losowanie.<br>
<br>
<b>3. Sprawdzanie czy różnica poziomów między graczami jest zbyt wysoka</b><br>
W przypadku, gdy poziomy dwóch dowolnych graczy zbytnio od siebie odbiegają, liczba losowań, niezależnie od liczności grupy, wynosi 1. W przeciwnym przypadku kolejnym krokiem jest punkt czwarty.<br>
<br>
Poziom najmniejszego gracza w drużynie:<br>
<code>lvl<sub>min</sub> = max( min( ceil( (min( lvl<sub>max</sub>, 300) - 4) / (1 + server_factor) ), lvl<sub>max</sub> - 14), 1 )</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>max</sub></code> - najwyższy poziom gracza w drużynie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>server_factor</code> - współczynnik serwerowy: 0.2 dla serwera publicznego, 0.4 dla serwera prywatnego oraz świata Nerthus.<br>
<br>
Poziom najwyższego gracza w drużynie:<br>
<code>lvl<sub>ally_max</sub> = max( round( (1 + server_factor) * lvl<sub>ally_min</sub>) + 4, lvl<sub>ally_min</sub> + 14)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>ally_max</sub></code> - najwyższy poziom członka grupy. <b>Jeżeli wartość przekroczy 299, to maksymalny poziom członka drużyny zawsze wynosi 500</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>ally_min</sub></code> - najniższy poziom członka grupy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>min</sub></code> - najniższy poziom gracza w drużynie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>server_factor</code> - współczynnik serwerowy: 0.2 dla serwera publicznego, 0.4 dla serwera prywatnego oraz świata Nerthus.<br>
<br>
<b>4. Obliczanie liczby losowań</b><br>
Liczba losowań jest zależna od liczby członków drużyny, która przeżyła do końca walki.<br>
<code>drops = min( 10, max( 1, 1 + floor((looters - 1) * 0.5 + rng)))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>drops</code> - liczba losowań.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>looters</code> - liczba członków drużyny, którzy przeżyli.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rng</code> - 50%, że wyniesie 0.5 oraz 50%, że wyniesie 0 (losowane tylko kiedy liczba członków drużyny jest parzysta).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja matematyczna minimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja matematyczna maksimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja matematyczna podłoga (zaokrąglenie w dół).<br>
<br>
<i>Przykłady</i>:<br>
W przypadku pełnej grupy graczy, liczba zdobyczy wynosi 5 oraz istnieje 50% szans na wylosowanie szóstego łupu.<br>
W przypadku, gdy gracz walczy w pojedynkę, liczba zdobyczy zawsze wynosi 1.<br>
W przypadku grupy dwóch graczy, liczba zdobyczy wynosi 1 i istnieje 50% szans na wylosowanie drugiego łupu.<br>
Mechanizm pozwala na wylosowanie do 10 łupów (jeżeli drużyna liczyłaby co najmniej 18 graczy).<br>
<br>
<b>5. Obliczanie szansy na pusty łup</b><br>
Dla każdego losowania obliczana jest szansa na pusty łup w zależności od mocy typu <b>NIC</b> ustalonej w szablonie zdobyczy.<br>
Szansa na pusty łup jest stosunkiem mocy <b>NIC</b> do sumy mocy wszystkich przedmiotów szablonu zdobyczy (przedmioty pospolite mają odpowiednio wyższą moc w zaprojektowanym szablonie niż przedmioty unikatowe, a przedmioty unikatowe wyższą niż przedmioty heroiczne itd.). Moc każdego przedmiotu jest zależna od rzadkości przedmiotu (niższa dla wyższej jakości) oraz od liczby przedmiotów danej rzadkości - wartość jest dopasowana w taki sposób, by finalna szansa na przedmiot danej rzadkości była równa ustandaryzowanej dla danego typu potwora.<br>
<br>
Kolejność mechanik wpływających na pusty łup:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. Zwiększenie szansy na pusty łup jeżeli liczba wystąpień tego samego szablonu zdobyczy jest wysoka (na przykład na ekspowisku).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Moc pustego łupu rośnie wówczas zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>new_power_empty = floor(0.5 + power_empty * (1.0 + 0.8 * ln(max(1, usage))))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<tabgdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>new_power_empty</code> - moc pustego łupu po uwzględnieniu wszystkich wystąpień szablonu w potworach<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>power_empty</code> - wstępna moc pustego łupu ustalona w szablonie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>usage</code> - liczba potworów z tym samym szablonem zdobyczy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ln</code> - funkcja matematyczna logarytm naturalny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja matematyczna podłoga.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b. Zmniejszenie szansy na pusty łup ze względu na ustawienia świata.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c. Zmniejszenie szansy na pusty łup z błogosławieństwa dla samotnie walczącego gracza (ze statystyką <code>lootbon</code>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;d. Modyfikacja łupu na serwerze <a href="https://pomoc.margonem.pl/index/view,311">Brutal</a>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• W przypadku, gdy w szablonie występuje szansa na pusty łup, moc pustego łupu oraz pospolitych przedmiotów jest mnożona 10-krotnie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli w szablonie szansa na pusty łup wynosi zero, moc przedmiotów unikatowych jest mnożona 10-krotnie.<br>
<br>
Prawdopodobienstwo na wylosowanie przedmiotu <code>X<sub>item</sub></code> w przypadku posiadania błogosławieństwa zmniejszającego szansę na pusty łup o <code>lootbon [%]</code> oblicza się zgodnie ze wzorem:<br>
<code>p<sub>X</sub> = 100% * p<sub>X,base</sub> / (1 - p<sub>empty</sub> * lootbon)</code><br>
gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>p<sub>X</sub></code> - szansa na zdobycie przedmiotu X.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>p<sub>X,base</sub></code> - szansa na zdobycie przedmiotu X bez posiadania błogosławieństwa ze statystyką <code>lootbon</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>p<sub>empty</sub></code> - szansa na pusty łup.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lootbon</code> - zmniejszenie szansy na pusty łup z błogosławieństwa.<br>
<br>
<i>Przykład:</i><br>
Z <a href="#t182">tabeli szans na przedmiot danej jakości</a> wyczytano, że prawdopodobieństwo na przedmiot legendarny z herosa eventowego wynosi 1%, a prawdopodobieństwo na pusty łup wynosi 29%. W przypadku założenia błogosławieństwa zmniejszającego szansę na pusty łup o 50% pod warunkiem zwycięstwa w samotnej walce, szansa na dowolny przedmiot legendarny wyniesie:<br>
<code>p<sub>legendary</sub> = 100% * 0.01 / (1 - 0.29 * 0.5) = 1.16%</code><br>
<br>
<b><a href="https://youtube.com/shorts/EXK7w9wyqQk">Krótki film</a></b> streszczający losowość systemu zdobyczy.<br>
<br>
Statystykę <code>lootbon</code> można również w tym wzorze zastąpić dowolną inną statystyką zmniejszającą szansę na pusty łup oferowaną z innych mechanik niż błogosławieństwa. Jeżeli ustawienia świata zmniejszają szansę na pusty łup trzykrotnie, jest to jednoznaczne ze zmniejszeniem szansy na pusty łup o 66% (<code>lootbon=0.66</code>).<br>
<br>
Poniżej zestawiono przykład wzrostu szansy na przedmiot legendarny z elity II, z szansą na ten przedmiot równą 0.06% oraz szansą na puty łup równą 50%, w przypadku posiadania błogosławieństwa ze statystyką obniżającą szansę na pusty łup.<br>
<br><table id="t183" style="width:500px">
<tbody><tr><th colspan="3" style="background-color:#546dd2"><center>Wpływ błogosławieństwa zmniejszającego prawopodobieństwo wystąpienia pustego łupu na szansę na przedmiot legendarny</center></th></tr><tr><th>Zmniejszenie szansy na pusty łup</th><th>Szansa na przedmiot legendarny</th><th>Ile razy się zwiększyła szansa</th></tr><tr><td>0%</td><td>0.060%</td><td>x1.00</td></tr><tr><td>5%</td><td>0.062%</td><td>x1.03</td></tr><tr><td>10%</td><td>0.063%</td><td>x1.05</td></tr><tr><td>20%</td><td>0.067%</td><td>x1.11</td></tr><tr><td>25%</td><td>0.069%</td><td>x1.14</td></tr><tr><td>50%</td><td>0.080%</td><td>x1.33</td></tr><tr><td>55%</td><td>0.083%</td><td>x1.38</td></tr><tr><td>60%</td><td>0.086%</td><td>x1.43</td></tr><tr><td>65%</td><td>0.089%</td><td>x1.48</td></tr><tr><td>70%</td><td>0.092%</td><td>x1.54</td></tr><tr><td>75%</td><td>0.096%</td><td>x1.60</td></tr><tr><td>80%</td><td>0.100%</td><td>x1.67</td></tr><tr><td>85%</td><td>0.104%</td><td>x1.74</td></tr><tr><td>90%</td><td>0.109%</td><td>x1.82</td></tr><tr><td>95%</td><td>0.114%</td><td>x1.90</td></tr><tr><td>100%</td><td>0.120%</td><td>x2.00</td></tr></tbody></table><br><br>
<h3><span class="color-blue">Mechanizm rozdzielania łupów</span></h3>Istnieją dwie metody przyznawania zdobyczy drużynie - zdobycz losowana oraz łup personalny.<br>
<br>
<b>Zdobycz losowana</b><br>
Zdobycz losowana następuje po pokonaniu potworów typu: Zwykły Potwór, Elita, Elita II, Elita III, Heros, Tytan, Heros Eventowy, Tytan Eventowy. Polega na współdzieleniu okna łupów między graczami i umożliwia wszystkim członkom drużyny wybór jednej z trzech decyzji dla każdego przedmiotu: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Nie chcę - gracz nie otrzyma przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Chcę - gracz weźmie udział w losowaniu przydziału przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Chcę bardzo - gracz weźmie udział w losowaniu przydziału przedmiotu z wyższym priorytetem względem osób zaznaczających "Chcę" (dostępne tylko, gdy profesja postaci spełnia wymagania przedmiotu).<br>
<br>
Opis mechaniki przydziału przedmiotu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. Każdy gracz wstępnie otrzymuje 20 <b>punktów szans</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b. Gracz po otrzymaniu jednego przedmiotu traci 15 <b>punktów szans</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c. Gracz nie może mieć mniej niż 1 <b>punktu szansy</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;d. Jeżeli rozdzielanie przedmiotu się nie powiedzie, przedmiot jest usuwany.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;e. Następuje losowanie względem posiadanych <b>punktów szans</b> graczy. Najpierw wśród graczy oznaczających "Bardzo potrzebuję", a następnie "Chcę", jeżeli do pierwszego losowania nie doszło.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;f. Niezależnie od wybranej decyzji, gracz po otrzymaniu przedmiotu ma obniżane <b>punkty szans</b>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;g. Najpierw losowane są przedmioty, które zostały utworzone w grze jako pierwsze (czyli najbardziej z lewej strony w oknie łupów).<br>
<br>
<b><a href="https://youtube.com/shorts/DvfwNmnKgt8">Krótki film</a></b> objaśniający zasady rozdzielania łupów.<br>
<br>
<b>Łup personalny</b><br>
Łup personalny następuje po pokonaniu potworów typu: Kolos, Kolos Eventowy, Elita III Eventowa. Każdy gracz ma losowaną zdobycz z puli przedmiotów, dla których postać gracza spełnia wymagania dotyczące profesji. Każdy gracz otrzymuje przedmiot dla siebie bez możliwości jego odrzucenia i bez możliwości decydowania o łupie innych członków drużyny.<br>
<br>
<br><br>
<h3><span class="color-blue">Rzadkość zdobyczy i ich liczba w szablonie potworów</span></h3>Dostępnych jest 6 różnych typów rzadkości przedmiotu, różniących się od siebie siłą oraz liczbą atrybutów (później nazywanych bonusami). Przedmioty mogą więc przyjmować rzadkość:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pospolity.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Unikatowy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Heroiczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ulepszony (dostępny wyłącznie z opcji Premium).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Legendarny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Artefakt (dostępny wyłącznie jako przedmioty nieekwipowane z zadań).<br>
<br>
Ustala się, że przedmioty heroiczne i ulepszone mają ten sam stopień jakości ze wględu na tą samą moc atrybutów natywnych.<br>
<br>
Każdy typ potwora ma z założeń określoną w przybliżeniu liczbę przedmiotów danej rzadkości, które występują u niego w szablonie zdobyczy. Zestawienie zostało zaprezentowane w tabeli poniżej.<br>
<br>
<br><table id="t181" style="width:500px">
<tbody><tr><th colspan="6" style="background-color:#546dd2"><center>Liczba przedmiotów danej rzadkości w szablonie</center></th></tr><tr><td style="background-color:lightgrey"><center>Typ potwora</center></td><td style="background-color:lightgrey"><center>Pusty łup</center></td><td style="background-color:grey"><center>Pospolity</center></td><td style="background-color:#f3f213"><center>Unikatowy</center></td><td style="background-color:#918fff"><center>Heroiczny</center></td><td style="background-color:#ff603b"><center>Legendarny</center></td></tr><tr><td><center>Zwykły Potwór</center></td><td><center>Tak</center></td><td><center>1-10</center></td><td><center>0-4</center></td><td><center>0</center></td><td><center>0</center></td></tr><tr><td><center>Elita</center></td><td><center>Tak</center></td><td><center>1-8</center></td><td><center>2-6</center></td><td><center>1-4</center></td><td><center>0</center></td></tr><tr><td><center>Elita II</center></td><td><center>Tak</center></td><td><center>1-8</center></td><td><center>6-12</center></td><td><center>6-12</center></td><td><center>3</center></td></tr><tr><td><center>Elita III</center></td><td><center>Nie</center></td><td><center>0</center></td><td><center>3-6</center></td><td><center>3-6</center></td><td><center>1-2</center></td></tr><tr><td><center>Heros</center></td><td><center>Nie</center></td><td><center>1</center></td><td><center>14-22</center></td><td><center>14-22</center></td><td><center>4</center></td></tr><tr><td><center>Kolos*</center></td><td><center>Nie</center></td><td><center>0</center></td><td><center>20-30</center></td><td><center>15-25</center></td><td><center>6-8</center></td></tr><tr><td><center>Tytan</center></td><td><center>Nie</center></td><td><center>0</center></td><td><center>18-24</center></td><td><center>18-24</center></td><td><center>7</center></td></tr><tr><td><center>Elita Wędrująca</center></td><td><center>Nie</center></td><td><center>0-2</center></td><td><center>1-6</center></td><td><center>1-6</center></td><td><center>0-3</center></td></tr><tr><td><center>Elita III Eventowa*</center></td><td><center>Nie</center></td><td><center>2-6</center></td><td><center>8-20</center></td><td><center>8-20</center></td><td><center>1-3</center></td></tr><tr><td><center>Heros Eventowy</center></td><td><center>Tak</center></td><td><center>0</center></td><td><center>6-8</center></td><td><center>6-8</center></td><td><center>2-4</center></td></tr><tr><td><center>Kolos Eventowy*</center></td><td><center>Nie</center></td><td><center>0</center></td><td><center>22</center></td><td><center>22</center></td><td><center>2-7</center></td></tr><tr><td><center>Tytan Eventowy</center></td><td><center>Nie</center></td><td><center>0</center></td><td><center>22</center></td><td><center>22</center></td><td><center>2-7</center></td></tr><tr><th colspan="6"><center>* Typ NPC z osobistym łupem</center></th></tr></tbody></table><br><br>
<br><table id="t182" style="width:500px">
<tbody><tr><th colspan="6" style="background-color:#546dd2"><center>Szanse na przedmiot danej rzadkości w szablonie</center></th></tr><tr><td style="background-color:lightgrey"><center>Typ potwora</center></td><td style="background-color:lightgrey"><center>Pusty łup</center></td><td style="background-color:grey"><center>Pospolity</center></td><td style="background-color:#f3f213"><center>Unikatowy</center></td><td style="background-color:#918fff"><center>Heroiczny</center></td><td style="background-color:#ff603b"><center>Legendarny</center></td></tr><tr><td><center>Zwykły Potwór</center></td><td><center>66.5%</center></td><td><center>33%</center></td><td><center>0.5%</center></td><td><center>0%</center></td><td><center>0%</center></td></tr><tr><td><center>Elita</center></td><td><center>50%</center></td><td><center>45%</center></td><td><center>4%</center></td><td><center>1%</center></td><td><center>0%</center></td></tr><tr><td><center>Elita II</center></td><td><center>50%</center></td><td><center>39.44%</center></td><td><center>8.5%</center></td><td><center>2%</center></td><td><center>0.06%</center></td></tr><tr><td><center>Elita II <a href="#k45">(specjalna)</a></center></td><td><center>50%</center></td><td><center>36.925%</center></td><td><center>10.5%</center></td><td><center>2.5%</center></td><td><center>0.075%</center></td></tr><tr><td><center>Elita III</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>70%</center></td><td><center>25%</center></td><td><center>5%</center></td></tr><tr><td><center>Heros***</center></td><td><center>0%</center></td><td><center>28.56%</center></td><td><center>50.32%</center></td><td><center>20.41%</center></td><td><center>0.71%</center></td></tr><tr><td><center>Kolos*</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>70%</center></td><td><center>29.7%</center></td><td><center>0.3%</center></td></tr><tr><td><center>Tytan</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>54.1%</center></td><td><center>45%</center></td><td><center>0.9%</center></td></tr><tr><td><center>Elita Wędrująca**</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>82.5%</center></td><td><center>17.36%</center></td><td><center>0.14%</center></td></tr><tr><td><center>Elita III Eventowa (normalny)*</center></td><td><center>0%</center></td><td><center>15%</center></td><td><center>65%</center></td><td><center>19.8%</center></td><td><center>0.2%</center></td></tr><tr><td><center>Elita III Eventowa (trudny)*</center></td><td><center>0%</center></td><td><center>5%</center></td><td><center>65%</center></td><td><center>29.7%</center></td><td><center>0.3%</center></td></tr><tr><td><center>Elita III Eventowa (mistrzowski)*</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>60%</center></td><td><center>39.6%</center></td><td><center>0.4%</center></td></tr><tr><td><center>Heros Eventowy</center></td><td><center>29%</center></td><td><center>0%</center></td><td><center>50%</center></td><td><center>20%</center></td><td><center>1%</center></td></tr><tr><td><center>Kolos Eventowy (normalny)*</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>65%</center></td><td><center>34.5%</center></td><td><center>0.5%</center></td></tr><tr><td><center>Kolos Eventowy (trudny)*</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>47.5%</center></td><td><center>51.75%</center></td><td><center>0.75%</center></td></tr><tr><td><center>Kolos Eventowy (mistrzowski)*</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>30%</center></td><td><center>69%</center></td><td><center>1%</center></td></tr><tr><td><center>Tytan Eventowy</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>54%</center></td><td><center>45%</center></td><td><center>1%</center></td></tr><tr><td><center>Kufer pospolity z Otchłani</center></td><td><center>0%</center></td><td><center>75%</center></td><td><center>25%</center></td><td><center>0%</center></td><td><center>0%</center></td></tr><tr><td><center>Kufer unikatowy z Otchłani</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>75%</center></td><td><center>24%</center></td><td><center>1%</center></td></tr><tr><td><center>Kufer heroiczny z Otchłani</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>96%</center></td><td><center>4%</center></td></tr><tr><td><center>Skrzynia Smoczych Kowali</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>89%</center></td><td><center>10%</center></td><td><center>1%</center></td></tr><tr><td><center>Doskonała skrzynia Smoczych Kowali</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>0%</center></td><td><center>98%</center></td><td><center>2%</center></td></tr><tr><th colspan="6"><center>* Typ NPC z osobistym łupem<br>** Dotyczy skrzyni reprezentującej szablon potwora<br>*** Dotyczy NPC po standaryzacji i reworku</center></th></tr></tbody></table><br><br>
Zostały określone następujące zasady projektowania szablonów zdobyczy:<br>
• Znacząca większosć przedmiotów tej samej rzadkości, ma tę samą szansę na zostanie wylosowanym. W celu obliczenia szansy na konkretny przedmiot należy więc podzielić szansę na zdobycie przedmiotu tej samej jakości przez liczbę przedmiotów tej samej jakości. Wyjątkiem są najczęściej Smoczne Runy, składniki do legendarnych zbroi lub inne nieekwipowalne przedmioty.<br>
• Elity II, Herosi, Kolosi, Tytani, Herosi Eventowi, Tytani Eventowi posiadają ustandaryzowany szablon zdobyczy - potwory tego samego typu posiadają taką samą szansę na wylosowanie przedmiotu określonej rzadkości (oraz szansę na pusty łup).<br>
• Kolosi Eventowi i Elity III Eventowe mają ustandaryzowany szablon zdobyczy w zakresie tego samego poziomu trudności.<br>
• Elity mają ustandaryzowany szablon zdobyczy, jeżeli ich liczba wystąpień nie przekracza 10 (skupiska potworów złożone z dużej liczby elit, posiadają znacznie zwiększoną szansę na pusty łup).<br>
• Szansa na pusty łup z szablonu elity oraz elity II wynosi 50%.<br>
• Wraz ze wzrostem liczby wystąpień tego samego szablonu zdobyczy przypisanego do potwora, rośnie szansa na pusty łup (dotyczy również elit II współdzielących szablon zdobyczy, takich jak Choukker).<br>
• Szansa na występujące w szablonach Elit II oraz Herosów kamienie do legendarnych zbroi jest zależna od liczby wymaganych składników do jej utworzenia. Im mniej wymaganych jest składników, tym szansa na ich pozyskanie jest mniejsza.<br>
• Elity II przebywające na mapach z wyłączoną możliwością grupowania się, mają 25% więcej szans na przedmiot unikatowy, heroiczny i legendarny bez zmiany szansy na pusty łup.<br>
<br>
Istnieją postacie, które losują łup pod warunkiem posiadania przez postać odpowiedniego klucza. W momencie użycia mechanizmu losującego łup, pobierana jest jedna sztuka klucza z ekwipunku postaci.<br>
Przykładami takich mechanizmów są:<br>
• <b>Smocza skrzynia</b> otwierana Pazurem młodego smoka.<br>
• <b>Shakkru</b> uruchamiany Rytualnym ostrzem orków.<br>
• <b>Rycerz z za małym mieczem</b> przeszukiwany Kolcem pajęczej matki.<br>
• <b>Ołtarz Pajęczej Bogini</b> uruchamiany Sercem pajęczego ołtarza.<br>
<br>
Odpowiednie szanse, na przedmiot dla tych mechanizmów, są ustawione w taki sposób, by prawdopodobieństwo zdobycia przedmiotu danej rzadkości przy jednoczesnym zdobyciu klucza, było identyczne jak w przypadku odpowiadającego typu potwora ze standardowym sposobem pozyskiwania przedmiotów. W ten sposób szanse na przedmiot unikatowy, heroiczny i legendarny z elity II - Władcy Rzek, są takie same jak z Ołtarza Pajęczej Bogini po uwzględnieniu zdobycia Serca pajęczego ołtarza.<br>
<br>
<br><br>
<a name="k19"></a><b><h3>1.9. Przedmioty używane podczas walki</h3></b><br>
Istnieją przedmioty konsumpcyjne, których efekt jest możliwy do wywołania w trakcie walki w dowolnym jej momencie bez utraty tury. Dzielą się one na trzy rodzaje:<br>
• Ucieczki.<br>
• Specjalne mikstury.<br>
• Zaśpiewy.<br>
<br><br>
<br>
<b>Ucieczki</b> powodują systemowe przerwanie walki u wszystkich graczy zachowując stan zdrowia oraz pozycji, który występował w momencie użycia przedmiotu. Są to przedmioty konsumpcyjne z atrybutem <code>action=flee</code>.<br>
<br><br>
<br>
<b>Specjalne mikstury</b> są to przedmioty konsumpcyjne posiadające atrybut <code>action=fightperheal,VALUE</code>, powodujący przywrócenie utraconych wcześniej punktów życia postaci o zadaną część bazowego zdrowia postaci określoną w parametrze <code>VALUE</code>. Przedmiot nie leczy o większą ilość punktów zdrowia niż pula, z którą gracz rozpoczął walkę.<br>
<br><br>
<br>
<b>Zaśpiewy</b> to przedmioty konsumpcyjne ze statystyką <code>battlestats</code>, które powodują wywołanie natychmiastowego efektu obsługiwanego przez system umiejętności. Główne cechy tych przedmiotów:<br>
• Statystyka może zostać wybrana z puli wszystkich aktywnych efektów umiejętności.<br>
• Przedmioty mogą zostać użyte wyłącznie podczas walk z NPC.<br>
• Dany efekt może zostać użyty przez jednego gracza tylko raz na walkę. Ten sam efekt może zostać wywołany tylko przez innego gracza. Gracz może aktywować jednocześnie wiele efektów przy użyciu zaśpiewów.<br>
• Czas trwania efektu w postaci liczby tur.<br>
<br>
<br><br>
<a name="k110"></a><b><h3>1.10. Wyczerpanie</h3></b><br>
Wyczerpanie jest atrybutem determinującym możliwość uzyskiwania doświadczenia za zabicie potworów. Codziennie o godzinie 5:25 postać otrzymuje wyczerpanie cykliczne, które uzupełnia liczbę punktów wyczerpania do 360 i z każdą minutą spada ono o 1 punkt. Gracz nie może przekroczyć 360 punktów wyczerpania czerpiąc je jedynie poprzez poranne uzupełnienie, natomiast może skumulować nadwyżkę jeżeli zwiększył swoje wyczerpanie z innych źródeł - w tym przypadku wyczerpanie jest sumą cyklicznego wyczerpania i wyczerpania pozyskanego w inny sposób. Wyczerpanie można zwiększać lub zmniejszać poprzez:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zakup zwiększenia lub zmniejszenia wyczerpania w module Premium.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Użycie specjalnego przedmiotu konsumpcyjnego zwiększającego lub zmniejszającego wyczerpanie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Skorzystanie z umiejętności klanowej, która zmniejsza lub zwiększa wyczerpanie postaci.<br>
<br>
Minimalna liczba punktów wyczerpania na postaci wynosi zero, natomiast maksymalna wartość nie jest ustalona.<br>
Wyczerpanie nie wpływa na pozyskiwanie doświadczenia z innych źródeł (mikstury, zadania).<br>
<br>
Przypadki wyjątkowe zależne od serwera:<br>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Na serwerach prywatnych, wyczerpanie nie jest odnawiane wraz z poranną przerwą. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Na serwerze Perkun gracze od poziomu 20 wzwyż, generują tylko 30 punktów wyczerpania wraz z poranną przerwą.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Na serwerze Perkun, gracze mogą otrzymać od 20 do 46 punktów wyczerpania za zwycięstwo w walce. Pierwiastek z sumy kwadratów poziomów graczy z każdej z drużyn musi być mniejszy lub równy 1.5-krotności tego samego wskaźnika obliczonego dla przeciwnej drużyny. Opisane jest to nierównością:<br>
<code>√(<sup>N</sup>Σ<sub>n</sub>player_lvl<sup>2</sup><sub>n</sub>) &lt;= 1.5 * √(<sup>M</sup>Σ<sub>m</sub>player_lvl<sup>2</sup><sub>m</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>N</code> - liczba graczy w pierwszej drużynie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>M</code> - liczba graczy w drugiej drużynie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>player_lvl</code> - poziom gracza.<br>
<br>
<a name="k111"></a><b><h3>1.11. Mechaniki światów specjalnych</h3></b><br>
Część mechaniki związanych z walkami różni się w zależności od serwera, na którym prowadzi rozgrywkę gracz. Serwery dzielą się na:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• <a href="https://pomoc.margonem.pl/index/view,268">Fabularne</a>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• <a href="https://pomoc.margonem.pl/index/view,267">PvP</a>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Non-PvP.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• <a href="https://pomoc.margonem.pl/index/view,311">Hard-PvP</a>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• <a href="https://pomoc.margonem.pl/index/view,312">Zawodowe</a>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• <a href="https://pomoc.margonem.pl/index/view,304">Prywatne</a>.<br>
<br>
<h3><span class="color-blue">Światy fabularne</span></h3>Do światów tych należy Nerthus.<br>
<br>
Na serwerze można posiadać tylko jedną postać, a wymagania założenia postaci są ściśle określone i zależą od posiadanych przez gracza Smoczych Łusek, reputacji, współczynnika ostrzeżeń, poziomu postaci na innych światach.<br>
Doświadczenie za zadania na światach fabularnych jest o 200% wyższe.<br>
<br>
Zmiany związane z walkami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Doświadczenie za potwory jest mniejsze o 50%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziomy potworów i graczy są zastąpione tytułami.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tytani oraz kolosi są osłabieni o 50%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Do zdobywania łupu konieczne jest posiadanie niezerowego wyczerpania.<br>
<br>
<h3><span class="color-blue">Światy PvP</span></h3>Do światów tych należy Perkun.<br>
<br>
Na serwerze występuje podział profesji na <b>frakcje</b>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Frakcja I: wojownik, paladyn, łowca.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Frakcja II: tancerz ostrzy, mag, tropiciel.<br>
<br>
Gracz tworząc postać, automatycznie jest przydzielany do frakcji w zależności od wybranej profesji.<br>
Różnice w mechanice zdeterminowane podziałem na frakcje:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zablokowanie niektórych akcji między postaciami z różnych frakcji (poczta, handel, zaproszenia do znajomych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Klany są frakcyjne i mogą w nich występować tylko postacie z profesją należącą do tej samej frakcji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zmiany wizualne w interfejsie wyróżniające graczy z przeciwnej frakcji od graczy z tej samej frakcji co postać.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieje ograniczenie wyboru profesji, jeżeli jedna frakcja ma 20% więcej postaci niż druga, gracze nie mogą zakładać postaci o profesji znajdującej się w pierwszej frakcji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Nazwy graczy z przeciwnej frakcji są ukryte.<br>
<br>
Zmiany związane z walkami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wygrana w walce z graczem w ramach nagrody zwiększa wyczerpanie postaci od 20 do 46 punktów w zależności od różnicy poziomów między postaciami.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Postać nie otrzymuje wyczerpania, gdy IP którychkolwiek graczy z przeciwnych drużyn jest takie samo.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Limit punktów wyczerpania wynosi 2000.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Postać nie otrzymuje wyczerpania, jeżeli walka odbywa się na mapie typu Arena.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wygrana w walce powoduje zabranie przegranym postaciom 1% posiadanego przez nich złota, które jest po równo rozdzielane między graczy ze zwycięskiej drużyny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wygrana w walce powoduje przyznanie postaci 20-krotności doświadczenia za zabicie potwora na tym samym poziomie co przeciwnik, o ile różnica poziomów między graczami jest mniejsza niż 5%. Bonus można odebrać maksymalnie 3 razy w ciągu doby (reset występuje podczas porannej synchronizacji o 5:25).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tytani oraz kolosi są osłabieni o 30%.<br>
<br>
Zmiany związane z mapami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Na wszystkich żółtych mapach można bezwarunkowo zaatakować postać z przeciwnej frakcji, ale postać z tej samej frakcji można zaatakować tylko z wyrażoną przez nią zgodą na walkę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Czerwone mapy mogą być zdobywane poprzez zabijanie graczy z przeciwnej frakcji. Zdobywanie map polega na kumulowaniu współczynnika zdobycia mapy wyrażanego w procentach:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zwiększenie współczynnika zdobycia mapy o 5% za każdego pokonanego gracza z przeciwnej frakcji przez frakcję postaci (maksymalnie o 100%).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zmniejszenie współczynnika zdobycia mapy o 5% za każdego pokonanego gracza z frakcji postaci przez frakcję przeciwną (maksymalnie o 100%).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wzrost współczynnika zdobycia mapy jednej frakcji powoduje analogiczny spadek u drugiej frakcji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Współczynnika zdobycia mapy zmienia się o 1% do 3 minuty dążąc do wartości wyjściowej - 0%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Współczynnik zdobycia mapy zwiększa lub zmniejsza zdobywane doświadczenie z potworów występujących na tej mapie o 3% za każdy 1% zgromadzonego lub brakującego współczynnika zdobycia.<br>
<br>
<h3><span class="color-blue">Światy Non-PvP</span></h3>Do światów tych należy Majuna.<br>
<br>
Zmiany związane z mapami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mapy czerwone są zamienione na żółte.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mapy z ustawieniem <i>Zawsze bezwarunkowe PvP</i> pozostają czerwone.<br>
<br>
<h3><span class="color-blue">Światy Hard-PvP</span></h3>Do światów tych należy Brutal.<br>
Na świecie Brutal nie można pozyskać Punktów Honoru w inny sposób niż walki z graczami, a doświadczenie za zadania powyżej poziomu 14 jest dwukrotnie mniejsze.<br>
<br>
Zmiany związane z walkami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• W walkach z graczami został wyłączony bonus do statystyk wynikający z przewagi poziomowej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Nie można atakować graczy z poziomem niższym od 21.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeżeli gracz, którego poziom jest niższy niż 95% poziomu przeciwnika, przegra walkę, odradza się dwukrotnie szybciej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mechanizm listów gończych jest wyłączony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Doświadczenie pozyskiwane w walkach z potworami jest zmniejszone:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ zmniejszenie o 0% między poziomem 1 a 14.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ zmniejszenie o 60% między poziomem 15 a 44.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ zmniejszenie o 80% powyżej poziomu 45.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieje możliwość pozyskania łupu w walce z graczami jeżeli różnica poziomów między graczami jest mniejsza niż 5% poziomu niższego gracza:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Za zwycięstwo gracz może otrzymać doświadczenie równe 30-krotności potwora zabitego na danym poziomie. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przeciwnik traci tyle samo doświadczenia, o ile nie przekracza to 1% posiadanego doświadczenia (w przeciwnym wypadku traci 1% doświadczenia). Nie istnieje jednak możliwość cofnięcia awansu poziomowego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ W walkach grupowych tylko gracze, którzy przeżyli otrzymują doświadczenie rozdzielane na nich po równo.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Można pozyskać maksymalnie 3 razy doświadczenie, za tego samego przeciwnika, w ciągu doby (reset następuje wraz z przerwą poranną o 5:25).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Za zwycięstwo w walce można wylosować przedmiot z ekwipunku poległego przeciwnika. Szansa na przedmiot zależy od rzadkości przedmiotu (2% na unikatowy, 1% na heroiczny, 0.2% na ulepszony, 0.1% na legendarny). <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ W przypadku walki grupowej, następuje rozdzielanie przedmiotów w oknie zdobyczy z możliwością zadecydowania o łupie (opcje "Chcę", "Nie chcę", "Bardzo potrzebuję").<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Można rozpocząć losowanie łupu od danego gracza maksymalnie 3 razy na dobę - każde kolejne losowanie zniszczy łup.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Za zwycięstwo gracz może odebrać przeciwnikowi 1% posiadanego przez niego złota.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Nie ma możliwości pozyskiwania doświadczenia, łupu ani złota za zwycięstwo na mapie typu Arena. <br>
<br>
Zmiany związane z mapami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wszystkie lokacje poza miastami, wnętrzami budynków oraz wioską startową są czerwone i obowiązuje na nich bezwarunkowa zgoda na PvP.<br>
<br>
<h3><span class="color-blue">Światy zawodowe</span></h3>Do światów tych należy Berufs.<br>
<br>
Śmierć postaci gracza powoduje:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Odrodzenie się jej w Grobowcu Śmiałków.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zmniejszenie jej poziomu do 1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przywrócenie atrybutów podstawowych do wartości z pierwszego poziomu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zresetowanie wszystkich zestawów umiejętności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zdjęcie przedmiotów z ekwipunku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Utratę złota do poziomu równego limitowi złota na danym poziomie.<br>
<br>
Zmiany związane z walkami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tytani oraz kolosi są osłabieni o 15%.<br>
<br>
Zmiany związane z mapami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieją mapy, na których śmierć nie powoduje utraty poziomu, a postać nie ponosi żadnych konsekwencji związanych z utratą poziomu.<br>
<br>
<h3><span class="color-blue">Światy prywatne</span></h3>Światy te są zakupione przez graczy i mogą mieć dostosowaną przez zarządcę konfigurację:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Niszczenie łupów od różnicy poziomów: 13-50.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Osłabienie tytanów: 0-50%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Osłabienie kolosów: 0-50%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mnożnik doświadczenia za potwory: 0.5-5.0.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mnożnik doświadczenia za zadania: 1.0-5.0.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mnożnik Punktów Honoru: 0.1-3.0.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mnożnik przyspieszenia czasu odradzania się potworów: 1.0-3.0.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Mnożnik zmniejszenia szansy na pusty łup: 1-4.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wyłączone automatyczne nakładanie blokady chatu na graczy: 0-1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wyłączenie przyrostu statystyk w walkach z przewagą poziomową: 0-1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Włączenie wymogu wyczerpania do zdobycia łupu: 0-1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ukrywanie poziomów graczy: 0-1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowa komenda czatu (<code>/me, /nar</code>): 0-1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Całodobowe czerwone mapy bez zmiany w żółte: 0-1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Całodobowe żółte mapy bez zmiany w czerwone: 0-1.<br>
<br>
<br><br>
<a name="k112"></a><b><h3>1.12. Listy gończe</h3></b><br>
Listy gończe są mechanizmem karania graczy, którzy zbyt często zabijają postacie posiadające wiele poziomów mniej. W przypadku, gdy postać zabije zbyt wielu graczy z wysoką przewagą:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jego postać trafia na listę poszukiwanych graczy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jego postać jest podświetlona czerwonym neonem.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jego postać może być zaatakowana, przez innych graczy, na żółtej i pomarańczowej mapie niezależnie od ustawionej zgody na PvP.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pod nazwą postaci występuje komunikat informujący o tym, że gracz jest poszukiwany.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jego postać odradza się trzy razy dłużej (nie dotyczy walk na mapach typu Arena).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jego postać, po przegranej walce, traci 1% posiadanego przez siebie złota, które jest dzielone po równo dla każdego zwycięzcy (nie dotyczy walk na mapach typu Arena). W przypadku, gdy gracz poszukiwany jest w grupie, po przegranej walce wszyscy członkowie jego grupy tracą 1% złota.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jego postać traci bonusy do statystyk wynikające z przewagi poziomowej.<br>
<br>
Lista poszukiwanych graczy dostępna jest w module listów gończych, dostępnym poprzez naciśnięcie na ikonkę symbolizującą kolor mapy lub poprzez zakładkę Poszukiwani w module Społeczności.<br>
W module wyświetlani są wszyscy aktywni w danej chwili gracze, którzy są poszukiwani listem gończym.<br>
<br>
Aby postać była poszukiwana listem gończym, musi posiadać 30 punktów karnych. Działanie mechanizmu punktów karnych jest następujące:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Postać otrzymuje punkt karny, jeżeli zaatakuje i wygra walkę z przeciwnikiem, którego poziom jest co najmniej mniejszy o:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min_lvl_difference = 16 + max(0 , (lvl_player - 100) / 5)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min_lvl_difference</code> - różnica poziomów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl_player</code> - poziom postaci gracza atakującego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja matematyczna maksimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wszyscy gracze drużyny otrzymują punkt karny, jeżeli wygrają z grupą przeciwników, których poziomy postaci spełniają nierówność:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="display: inline-block; line-height: 0.5"><code>0.5 * (max <sub>ω ∈ Ω1</sub> lvl(ω) + <sup>Ω1</sup>Σ<sub>ω</sub>lvl(ω) / |Ω1|) - <sup>Ω2</sup>Σ<sub>ω</sub>lvl(ω) / |Ω2| &gt; 15 + max( 0 , 0.1 * (max <sub>ω ∈Ω1</sub> lvl(ω) + <sup>Ω1</sup>Σ<sub>ω</sub>lvl(ω) / |Ω1|) - 20 )</code></span><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl(ω)</code> - funkcja obliczająca poziom postaci ω.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja najwyższej wartości.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>Ω1</code> - zbiór członków drużyny atakującej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>Ω2</code> - zbiór członków drużyny atakowanej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>|Ωn|</code> - liczność drużyny n.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pokonanie grupy graczy przydziela jeden punkt karny, niezależnie od liczności grupy przegranej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punkty karne są naliczane jedynie postaci atakującej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punkty karne nie są naliczane, jeżeli klany atakującego i atakowanego gracza prowadzą obustronną wojnę trwającą co najmniej 3 godziny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punkty karne nie są naliczane, jeżeli postać atakowana jest poszukiwana listem gończym.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punkty karne nie są naliczane, jeżeli walka odbywała się na mapie, na której wyłączony jest bonus wynikający z przewagi poziomowej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punkty karne nie są naliczane, jeżeli walka odbyła się na Otchłani.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Liczba punktów karnych maleje o 2 o 5:25 co dobę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Istnieją specjalne przedmioty konsumpcyjne ze statystyką <code>wanted_change</code>, których użycie może spowodować dodanie lub odjęcie punktów karnych do listu gończego.<br>
<br>
<br>
<hr><a name="k2"></a><h2><b>2. System tur</b></h2><a name="k21"></a><b><h3>2.1. Kolejność wykonywania tur</h3></b><br>
<b>Tura w systemie tur</b> to numerowana (od 1 wzwyż) akcja, którą postać może wykonać w sposób automatyczny (w przypadku postaci NPC lub graczy wybierających opcję automatycznej walki) lub manualny (wtedy gracz ma przyznawany czas na ruch). Tura jest akcją przyznawaną i tylko jedna postać w danym momencie może uzyskać możliwość wykonania tury. Po osiągnięciu maksymalnej liczby tur w walce, zostaje ona przerwana.<br>
Maksymalny liczba tur w walce jest sumą liczby tur wszystkich graczy uczestniczących w walce i wynosi:<br>
<code>max_moves = 75 * players_amount</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>players_amount</code> - liczba graczy<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max_moves</code> - maksymalna liczba tur<br>
Przykład:<br>
Walka, w której uczestniczył łowca, tropiciel oraz wojownik, nie wyłoniła zwycięzcy. Łowca i tropiciel walczyli przeciw wojownikowi. Łowca wykonał 90 tur, wojownik wykonał 55 tur, zatem wiemy, że tropiciel musiał wykonać liczbę tur:<br>
<code>output = 75 * 3 - (90 + 55) = 80</code><br>
<br>
Istnieje również osobne zliczanie tur w walce dla danego gracza, które służy obliczaniu efektów rozłożonych w czasie.<br>
Na liczbę tur nie wpływają dodatkowe tury wynikające z efektu <code>add_attacks</code>, występującego na przykład w umiejętności <i>Podwójny strzał</i>.<br>
<br>
<br><br>
Każdy gracz posiada swój <b>licznik czasu trwania</b> wszystkich wykonanych przez niego ataków oznaczanym jako <b>v</b>. Każda tura posiada swój czas wykonania <code>(AT - Attack Time)</code>, którego wartość służy do powiększania licznika gracza. Rozpoczynając walkę (tura zerowa), licznik jest ustawiany na wartość AT równą przewidywanemu czasowi trwania jego następnej tury. Po <code>N</code> turach licznik osiągnie wartość:<br>
<code>v<sub>N</sub> = <sup>N</sup>Σ<sub>n</sub> AT<sub>n</sub></code><br>
Przykłady:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Gracz rozpoczyna walkę i obliczany jest przewidywany czas wykonania przez niego pierwszej tury:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>v<sub>0</sub> = <sup>0</sup>Σ<sub>n</sub> AT<sub>n</sub> = 0.2</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Gracz wykonuje swoją pierwszą turę, która trwa 0.2:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>v<sub>1</sub> = <sup>1</sup>Σ<sub>n</sub> AT<sub>n</sub> = 0.4</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Gracz wykonuje swoją piątą turę, która trwa 0.1:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>v<sub>5</sub> = <sup>5</sup>Σ<sub>n</sub> AT<sub>n</sub> = <sup>4</sup>Σ<sub>n</sub> AT<sub>n</sub> + 0.1</code><br>
Czas, po jakim gracz dokonał akcji (czas oczekiwania przez serwer na ruch), nie wpływa na licznik czasu trwania tur. <br>
<br>
<br><br>
<b>Czas trwania tury a czas trwania ataku</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Czas trwania tury to czas oczekiwania na akcję gracza - jeśli system przyzna postaci możliwość wykonania tury, włącza się licznik, który po osiągnięciu wartości zero, automatycznie wykonuje akcję za gracza. Termin "Czas trwania wszystkich tur" odnosi się do czasu liczonego w sekundach, jaki gracz ma na wykonanie wszystkich akcji, zanim system uruchomi tryb specjalny, polegający na ustawieniu czasu trwania tury na wartość minimalną (zwykle 0 lub 1 sekundę). Mechanika ta została opisana w sekcji <a href="#k22">2.2. Czas oczekiwania na akcję gracza</a>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Czas trwania ataku (<code>attack time</code>) to parametr, który określa jak szybka jest postać. Zależy on od szybkości ataku postaci, spowolnienia jakie zostały na nią nałożone oraz wszelkich umiejętności, które modyfikują szybkość ataku postaci. Termin "Czas trwania wszystkich ataków" odnosi się do sumy czasu trwania ataku obliczonego dla każdej tury postaci, która służy do wyłaniania pierwszeństwa wykonania tury w danej chwili walki.<br>
<br>
<br><br>
<b>Pierwszeństwo w wykonaniu tury</b> ma gracz, którego przewidywany licznik czasu trwania ataków po zakończeniu następnej jego tury będzie najniższy. Silnik oblicza więc przewidywany czas trwania ataku dla każdego gracza i sumuje z jego licznikiem czasu trwania ataków. Tura zostanie przyznana graczowi, którego predykcyjna wartość licznika będzie najniższa. <br>
Przewidywany czas trwania następnego ataku obliczany jest w oparciu o działające na gracza efekty modyfikujące jego szybkość ruchu. Przewidywany czas trwania ataku obliczany jest jednocześnie dla wszystkich graczy oraz dla wielu następnych (przyszłych) tur po każdej wykonanej już turze, względem czego tworzy się kolejka poruszających się po sobie graczy umieszczana wewnątrz <i>Listy predykcji tur</i>.<br>
<code>v<sub>predicted</sub>(N) = v<sub>N - 1</sub> + AT<sub>N</sub> = <sup>N</sup>Σ<sub>n</sub> AT<sub>n</sub></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>v<sub>predicted</sub>(N)</code> - przewidywany skumulowany czas trwania N ataków gracza z uwzględnieniem następnej tury.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>v<sub>N - 1</sub></code> - wartość skumulowanego czasu trwania wszystkich dotychczasowych ataków gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>AT<sub>N</sub></code> - przewidywany czas trwania następnego ataku gracza.<br>
Po przyznaniu tury graczowi, wartość jego skumulowanego czasu trwania ataków (ani licznika każdego innego gracza) się nie zmienia. Inkrementacja zachodzi dopiero po wykonaniu przez niego tury, ponieważ przewidywany czas trwania ataku nie musi być równy faktycznemu czasowi ataku po jej wykonaniu (ze względu na występujące modyfikatory szybkości ataku):<br>
<code>v<sub>predicted</sub>(N) ≠ v<sub>N</sub></code><br>
<br>
Jeżeli więcej niż jeden gracz osiąga najniższy skumulowany przewidywany czas trwania następnego ataku, remis rozstrzygany jest poprzez przyznanie tury graczowi z najwyższym priorytetem, zgodnie z kolejnością (od najwyższego do najniższego priorytetu):<br>
1. Postać gracza, który rozpoczął walkę.<br>
2. Członek drużyny gracza, który rozpoczął walkę.<br>
3. Postać z najniższym ID.<br>
<br>
<br><br>
<b>Zasada obliczania czasu ataku:</b><br>
1. Uwględnienie wzmocnień addytywnych względem SA postaci powiększonego o 1:<br>
<code><span style="color: #a59148">SA_additive_modified</span> = (SA + 1) * (1 + additive_modifiers_sum<sup>[1]</sup>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>SA_additive_modified</code> - suma addytywnych modyfikatorów SA<br>
<br>
2. Uwzględnienie modyfikatorów stałych wraz ze wzmocnieniami oraz osłabieniami:<br>
<code><span style="color: blue">SA_constant_modifiers</span> = <span style="color: #a59148">SA_additive_modified</span> - <br>
[weapon_modifier * (1 + modifier_boost - slow_reduction) + eq_constant_modifiers_sum * (1 - slow_reduction)]<sup>[2]</sup></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>weapon_modifier</code> - największa wartość spowolnienia SA spośród posiadanych przez przeciwnika broni od zimna i trucizny <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>modifier_boost</code> - efekt umiejętności wzmocnienia spowalniania SA z broni przez przeciwnika<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>eq_constant_modifiers_sum</code> - suma wartości bonusów w obniżanie SA przeciwnika z ekwipunku przeciwnika<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>slow_reduction</code> - redukcja nałożonego na postać spowolnienia<br>
<br>
3. Obliczanie czasu ataku wraz ze sprawdzeniem limitu spowolnienia wynoszącego 33% SA spowalnianego gracza:<br>
<code><span style="color: red">AT</span> = min(1 / <span style="color: blue">SA_constant_modifiers</span>  ,   3 / (SA + 1))</code><br>
<br>
4. Uwzględnienie modyfikatorów multiplikatywnych:<br>
<code><span style="color: #7c88d6">AT_final</span> = multiplied_modifiers_product<sup>[3]</sup> * <span style="color: red">AT</span></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>multiplied_modifiers_product</code> - iloczyn multiplikatywnych modyfikatorów AT<br>
<br>
5. Sumowanie czasu ataku z wypadkowym licznikiem czasu trwania wszystkich ataków:<br>
<code>v<sub>N</sub> = <sup>N</sup>Σ<sub>n</sub> AT<sub>n</sub> = <sup>N-1</sup>Σ<sub>n</sub> AT<sub>n</sub> + <span style="color: #7c88d6">AT_final</span> = v<sub>N-1</sub> + <span style="color: #7c88d6">AT_final</span></code> <br>
<br>
________________________<br>
<sup>[1]</sup> Na przykład: <span style="color: #2e83f3"><b>Krytyczne spowolnienie</b></span> (-10%) wraz z <span style="color: #718e27">Szadzią</span> (-14%) wraz z <span style="color: #22f398"><b>Szybkim atakiem</b></span> (+40%) doprowadzi do osiągnięcia wartości:	<br>
<b>SA_additive_modified = (-<span style="color: #2e83f3">0.1</span> - <span style="color: #718e27">0.14</span> + <span style="color: #22f398">0.4</span>) = +0.16</b> <br>
<sup>[2]</sup> Uwzględniana jest tylko wyższa wartość spowolnienia z broni, obniżanie SA z ekwipunku nie posiada ograniczeń kumulacji. Wszystkie te modyfikatory są spowolnieniami, zatem w tym wzorze podajemy ich wartość bezwzględną. Na przykład: <span style="color: teal"><b>Spowolnienie z broni od zimna</b></span> (0.75) wraz z umiejętnością <span style="color: #718e27"><b>Pchnięcie mrozu</b></span> (100%) oraz <span style="color: #fd7b24"><b>obniżaniem SA z ekwipunku</b></span> (0.5) przeciwko <span style="color: #b41dfc"><b>redukcji spowolnienia</b></span> (25%) doprowadzi do osiągnięcia wartości:	<br>
<b>SA_constant_modifiers = [(<span style="color: teal">0.75</span> * ( 1 + <span style="color: #718e27">1</span> - <span style="color: #b41dfc">0.25</span>) + <span style="color: #fd7b24">0.5</span> * (1 - <span style="color: #b41dfc">0.25</span>)] = 1.6875</b><br>
<sup>[3]</sup> Na przykład: <span style="color: red"><b>Błyskawiczna strzała</b></span> (26%) wraz z <span style="color: #949100"><b>Szybką strzałą</b></span> (75%) doprowadzi do osiągnięcia wartości:	<br>
<b>multiplied_modifiers_product = [(1 - <span style="color: red">0.26</span>) * (1 - <span style="color: #949100">0.75</span>)] = 0.185</b><br>
<br>
<br><br>
<b>Przykład obliczania czasu trwania ataku:</b><br>
Walka trwa między tancerzem a magiem. <br>
Liczniki przed wykonaniem ataku:<br>
AT<sub>tancerz</sub> = 0.2000<br>
AT<sub>mag</sub> = 0.2200<br>
<br>
Przyjmijmy, że przewidywane AT Tancerza jest niższe niż przewidywane AT Maga po następnym ruchu, zatem Tancerz otrzymuje możliwość wykonania tury.<br>
Tancerz o SA 30.0 atakuje maga korzystając z umiejętności <i>Błyskawiczny cios</i> (40%), podczas którego zachodzi zdarzenie <i>Ciosu krytycznego</i>, które z kolei wyzwala efekty <i>Krytycznego przyspieszenia</i> (20%). Ponadto z umiejętności <i>Płynność ruchów</i> (80%) redukuje nałożone na niego spowolnienia.<br>
Mag o SA 22.0 wcześniej użył umiejętności spowalniającej szybkość ataku agresora - <i>Magiczna bariera</i> (15%) oraz Lodowy Pocisk (+65%). Ponadto jego broń od zimna spowalnia przeciwnika o 6.0 SA na 2 tury, a z ekwipunku posiada dodatkowe obniżanie SA przeciwnika o 3.5.<br>
<br>
Obliczanie AT tancerza po jego turze:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. <code><span style="color: #a59148">SA_additive_modified</span> = (30.0 + 1) * (1 + 0.4 + 0.2) = 49.6</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. <code><span style="color: blue">SA_constant_modified</span> = <span style="color: #a59148">49.6</span> - [6.0 * (1 + 0.65 - 0.8) + 3.5 * (1 - 0.8)] = 43.8</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. <code><span style="color: red">AT</span> = min(1 / <span style="color: blue">43.8</span>  ,   3 / (30.0 + 1)) = 0.02283</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. <code><span style="color: #7c88d6">AT_final</span> = (1 - 0) * <span style="color: red">0.02283</span> = 0.02283</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5. <code>v<sub>N</sub> = 0.2000 + <span style="color: #7c88d6">0.02283</span> = 0.2228</code><br>
<br>
Liczniki po wykonaniu tury tancerza:<br>
AT<sub>tancerz</sub> = 0.2228<br>
AT<sub>mag</sub> = 0.2200<br>
Następnie obliczane jest przewidywane AT (w sposób analogiczny z pominięciem punktu piątego oraz rzucanych w trakcie tury umiejętności) i na podstawie wyniku wyłaniana jest postać, która otrzyma możliwość wykonania tury.<br>
<br>
<br><br>
<a name="k22"></a><b><h3>2.2. Czas oczekiwania na akcję gracza</h3></b><br>
Serwer oczekuje określony czas na akcję gracza, po przekroczeniu którego dokonuje akcji w sposób automatyczny przekazuje możliwość wykonania tury następnemu graczowi z kolejki.<br>
Czas, podczas którego gracz może wykonać akcję, jest określony dwoma licznikami:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Czas trwania tury - licznik, który jest resetowany po otrzymaniu przez postać tury (możliwości wykonania akcji). Maleje o 1 co każdą sekundę. Wartość początkowa jest zależna od ustawień mapy, trybu przeprowadzania walki (świat lub Otchłań), typu przeciwnika (PvE lub PvP) oraz kary (ilość zaniechań wykonania tury przez gracza):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 16 sekund, jeżeli jest to pierwsza tura gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 16 sekund, jeżeli gracz dokonał działania w poprzedniej turze przed zakończeniem czasu oczekiwania.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 11 sekund, jeżeli gracz nie dokonał działania w poprzedniej turze i czas oczekiwania na ruch skończył się po 15 sekundach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 6 sekund, jeżeli gracz po raz drugi z kolei nie dokonał działania w poprzedniej turze i czas oczekiwania na ruch skończył się po 10 sekundach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 4 sekundy (zawsze), jeżeli gracz walczy na <i>Otchłani</i>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Każda mapa może mieć manualnie ustawiany czas oczekiwania na turę gracza (3 poziomy oczekiwania w zależności od tego, czy gracz zaniechał wykonania akcji przed upływem przyznanego mu czasu). Dotyczy to przede wszystkim map określonych jako <i>Krwawe Kopalnie</i>, na których gracz ma zawsze 4 sekundy na wykonanie tury.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Czas trwania wszystkich tur - licznik, który jest zatrzymywany po wykonaniu akcji przez gracza oraz wznawiany, gdy otrzyma turę. Jeżeli licznik spada do zera, to czas trwania tury (pojedynczej) zostaje ustawiony na czas minimalny. Zaniechanie czasu wykonania akcji może dodatkowo zmniejszyć licznik czasu trwania wszystkich tur. Każda lokalizacja może mieć ustawione parametry inne niż globalne, co można prześledzić w oknie "Świat" w zakładce "Parametry lokacji". Licznik ten ma następujące parametry:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Czas początkowy - czas, jaki otrzymuje każdy gracz uczestniczący w walce, podczas którego występuje tryb swobodny. Przyznawany czas na wykonanie tury wynika z ustawień licznika tury. Po przekroczeniu tego czasu, następuje przejście w tryb przyspieszony, podczas którego czas na wykonanie tury zawsze jest równy czasowi minimalnemu. Globalnie wartość czasu początkowego wynosi 120 sekund, ale istnieją lokacje z ustawionym czasem równym 60s.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Czas minimalny - określa wartość wyrażoną w sekundach, poniżej której nie może spaść czas wykonania tury. Jeżeli licznik trwania wszystkich tur osiągnie zero, obowiązuje tryb przyspieszony, podczas którego gracz otrzymuje zawsze czas minimalny na wykonania tury (zamiast standardowo 15 sekund). Globalnie wartość ta wynosi 2 sekundy, natomiast dla Krwawych Kopalni obowiązuje 0 sekund (tury postaci są wykonywane automatycznie).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Kara za brak ruchu - określa czas w sekundach o jaki zostaje pomniejszony licznik czasu trwania wszystkich tur w przypadku, gdy gracz zaniecha wykonania akcji. Globalnie wartość ta wynosi 5.<br>
<br>
<br><br>
<a name="k23"></a><b><h3>2.3. Umiejętności</h3></b><br>
Każdy gracz ma na początku do dyspozycji dwie bazowe akcje domyślne:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Atak - wyzwala losowanie wartości ataku oraz zadanie obrażeń przeciwnikowi z uwzględnieniem wszystkich zdarzeń i atrybutów, które aplikowane są wraz z atakiem.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Krok do przodu - akcja zmiany pozycji o jeden, która po spełnieniu warunków jest wykonywana niezależnie od ciążących na postaci efektów.<br>
<br>
<h3><span class="color-blue">Moduł umiejętności</span></h3>Korzystając z modułu umiejętności, gracz z poziomem większym bądź równym 25 może nauczyć postać określonych umiejętności. Umiejętności składają się z wielu efektów, które są odczytywane przez silnik i odpowiednio zmieniają postać gracza w trakcie rozgrywki lub w trakcie walki.<br>
<b><a href="https://youtube.com/shorts/PWMlHvvjZ5c">Krótki film</a></b> omawiający proces uczenia się umiejętności.<br>
<b>Podział umiejętności ze względu na posiadane efekty</b>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pasywna - umiejętność posiada wyłącznie efekty pasywne, czyli zwiększające atrybuty postaci oraz nadające parametry wyzwalające zdarzenia podczas walki lub po zakończeniu walki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Aktywna - umiejętność posiada co najmniej jeden efekt aktywny (wymagający aktywacji i trwający określoną liczbę tur) oraz dowolną liczbę efektów pasywnych. Każda umiejętność aktywna dodaje graczowi jedną nową akcję możliwą do wykonania podczas walki.<br>
<br>
Niektóre umiejętności aktywne pozbawiają gracza możliwości wykonania wraz z nią ataku (wyzwalany jest sam efekt umiejętności). Umiejętności można użyć zarówno na sobie jak i na innych graczach i potworach uczestniczących w walce.<br>
<b>Podział umiejętności aktywnych ze względu na rodzaj użycia</b>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Umiejętność parowana z atakiem (<code>Sum with attack</code>) - efekt następuje przed wykonaniem ataku po użyciu umiejętności na przeciwniku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Umiejętność nakładana na przeciwnika (<code>Spell</code>) - efekty umiejętności nakładane są  tylko po użyciu umiejętności na przeciwniku. Gracz zostaje pozbawiony ataku w tej turze.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Umiejętność nakładana na gracza rzucającego (<code>Only self</code>) - efekty umiejętności nakładane są tylko po użyciu umiejętności na sobie. Gracz zostaje pozbawiony ataku w tej turze.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Umiejętność nakładana na sojusznika (<code>Only friends</code>) - efekty umiejętności nakładane są po użyciu umiejętności na sojuszniku. Gracz zostaje pozbawiony ataku w tej turze. Typ umiejętności nie koliduje z typem <code>Only self</code>, zatem umiejętność może dziedziczyć po obu typach.<br>
Niektóre efekty aktywne kolidują ze sobą, przez co umieszczenie jednego z nich może wymusić rodzaj użycia umiejętności (na przykład użycie na sojusznika) lub sprawić, że efekt nie jest wyzwalany.<br>
<br>
<br><br>
Umiejętności mogą posiadać dodatkowe wymagania odnośnie pozycji gracza (zwarcie lub dystans).<br>
<b>Podział umiejętności aktywnych ze względu na wymagania pozycji</b>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwarcie (<code>Melee</code>) - umiejętność wykonywana wyłącznie jeśli różnica pozycji między graczami jest mniejsza bądź równa 1.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dystans (<code>Only distance</code>) - umiejętność wykonywana wyłącznie jeśli różnica pozycji między graczami jest większa niż 1.<br>
<br>
<br><br>
Prezentacja w oknie gry przebiega w formie tablicy poukładanych w odpowiedniej kolejności umiejętności. Każda umiejętność posiada swój wymagany poziom, ID oraz pozycję w tej tablicy. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• ID umiejętności służy dobraniu grafiki, efektów audiowizualnych oraz tooltipów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziom umiejętności służy umiejscowieniu jej w odpowiednim rzędzie tablicy w Module umiejętności. Gracz może nauczyć się umiejętności tylko jeśli spełnia jej wymagania poziomowe.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pozycja tablicy to kolumna, na której umiejętność występuje. Kolumna różni się w zależności od klienta (stary i nowy klient).<br>
<br>
Mechanika umiejętności składa się z porównywania obliczonej liczby punktów umiejętności jakie gracz wydał oraz przypisanej do każdej belki poziomowej (rzędu) liczby punktów umiejętności, którą gracz musi przekroczyć w celu nauki umiejętności z tej konkretnej belki.<br>
<b>Belki umiejętności oraz odpowiadające im wymagania punktowe</b>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Poziom: 25, Wydanych punktów: 0<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Poziom: 35, Wydanych punktów: 10<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. Poziom: 50, Wydanych punktów: 25<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. Poziom: 80, Wydanych punktów: 55<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5. Poziom: 120, Wydanych punktów: 95<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6. Poziom: 170, Wydanych punktów: 145<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7. Poziom: 230, Wydanych punktów: 205<br>
<br>
W celu wydania punktów nauki, od gracza pobierane jest złoto w wysokości:<br>
<code>gold_cost<sub>lvl</sub> = floor(lvl^1.9)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>gold_cost<sub>lvl</sub></code> - koszt rozdania punktu umiejętności dla postaci o poziomie <code>lvl</code> liczony w złocie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja matematyczna podłoga.<br>
Bez wymaganych sztuk złota, nauka umiejętności kończy się niepowodzeniem.<br>
Istnieją specjalne przedmioty konsumpcyjne z atrybutem <code>freeskills</code>, który sprawia, że przez określony czas nauka umiejętności jest darmowa.<br>
<br>
<br><br>
<h3><span class="color-blue">Zestawy umiejętności</span></h3>Każdy zestaw ekwipunku ma przypisany do siebie zestaw umiejętności. Przełączenie zestawu ekwipunku zawsze wiąże ze sobą przełączenie również zestawu umiejętności, który jest do niego przypisany. Każdy zestaw umiejętności można spersonalizować poprzez rozdanie punktów umiejętności. Zestaw można zresetować korzystając ze specjalnego przycisku znajdującego się w module umiejętności (koszt: 75 SŁ) lub wybierając odpowiedni dialog w rozmowie z NPC resetującym zestawy umiejętności (może wymagać opłaty w złocie).<br>
<br>
<br><br>
<a name="k24"></a><b><h3>2.4. Mistrzostwo walk</h3></b><br>
Mistrzostwo walk to opcja dostępna w module umiejętności, która pozwala zakolejkować używanie umiejętności podczas walki toczonej automatycznie. Lista składa się z dwudziestu ponumerowanych pozycji, które gracz musi odblokować z osobna przy użyciu złota lub Smoczych Łusek. <br>
Do danej pozycji można przypisać umiejętność lub akcję domyślną (Atak, Krok do Przodu). <br>
Algorytm działania Mistrzostwa walk podczas walki automatycznej jest następujący:<br>
1. Pobranie pierwszej pozycji z listy i próba wykonania akcji.<br>
2. Jeżeli działanie nie może być wykonane, pobierana jest kolejna pozycja.<br>
3. Algorytm zatrzymuje się na pierwszej pozycji, która może zostać wykonana.<br>
4. Jeżeli algorytm dotrze do końca listy, przechodzi na jej początek.<br>
5. Jeżeli żadne działanie z listy nie może zostać wykonane i algorytm dotrze do akcji, którą sprawdzał jaką pierwszą, podejmowana jest próba wykonania domyślnego Ataku. Jeżeli atak również nie może zostać wykonany, postać wykonuje Krok do Przodu.<br>
6. Celem umiejętności nakładanej na przeciwnika jest zawsze postać z najniższym poziomem, którą można zaatakować bez konieczności zmiany pozycji postaci (wyjątkiem jest konieczność zaatakowania przeciwnika, który rzucił na postać efekt <code>shout</code>). Jeżeli istnieje konieczność zmiany pozycji, postać wykonuje Krok do przodu.<br>
7. Jeżeli umiejętność, której używa gracz, może być nałożona na postać gracza lub sojusznika, to postać zawsze używa jej na sobie samej.<br>
<br>
<br>
<hr><a name="k3"></a><h2><b>3. Statystyki postaci w walce</b></h2><b>Informacja ogólna</b><br>
Wiele funkcji na wszelkie dostępne w grze atrybuty, może zawierać zbiór swoich wartości w dziedzinie liczb rzeczywistych. Ze względu na skończoną reprezentację wszystkich parametrów zarówno w momencie przekazywania informacji z serwera do klienta, jak i podczas wizualizowania tych parametrów graczom, dochodzi do zaokrągleń wartości. W przypadku, gdy nie została jasno zasygnalizowana metoda zaokrąglenia, przyjmuje się, że przed wysłaniem jej do klienta, nastąpiło zaokrąglenie matematyczne.<br>
W przypadku występowania rozrzutów jakichkolwiek wartości, losowanie jest zawsze podyktowane rozkładem jednostajnym dyskretnym (każda wartość ma takie same szanse na zostanie wylosowaną).<br>
<br>
<a name="k31"></a><b><h3>3.1. Statystyki gracza</h3></b><br>
Statystyki postaci gracza składają się z atrybutów, które mogą się zmieniać w wyniku:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• zmiany elementów ekwipunku<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• awansu poziomowego<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• zmiany umiejętności<br>
<br>
Podczas walki, atrybuty gracza są mapowane, w konsekwencji mogą zmieniać one swoje wartości chwilowo w zakresie danego pojedynku. Ulegają one wtedy zmianie w wyniku:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Użycia umiejętności postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Użycia umiejętności przez przeciwnika.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Użycia umiejętności przez sojusznika.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przyjęcia obrażeń od przeciwnika.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Skorzystania z Zaśpiewów typu <code>battlestat</code> lub Mikstur typu <code>fightperheal</code>.<br>
<br>
Poniżej został zamieszczony spis posiadanych przez postać atrybutów wraz z ich nazwami skrótowymi, używanymi przez klienta gry.<br>
<br>
<a name="damages"></a><br>
<h3><span class="color-blue">Typy obrażeń</span></h3><b>Obrażenia fizyczne</b> (<code>a1, a2</code>)<br>
• W logu walki kolorowane na szaro.<br>
• Obecne tylko jako atrybut broni do walki w zwarciu (jednoręczne, dwuręczne, półtoraręczne).<br>
• Wartość obrażeń losowana jest między wartością minimalną oraz maksymalną broni, a następnie sumowana efektem umiejętności, zwiększającym obrażenia za każdy posiadany punkt siły. Rozrzut w broniach wynosi 10% względem wartości średniej.<br>
• Są redukowane przez pancerz zgodnie ze wzorem:<br>
<code>dmg<sub>out</sub> = dmg<sub>in</sub> - ac * (1.13 - 0.31 * ac / dmg<sub>in</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>out</sub></code> - obrażenia zredukowane przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>in</sub></code> - obrażenia przed redukcją przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ac</code> - pancerz postaci atakowanej.<br>
• Absorpcja redukuje do 75% wartości obrażeń fizycznych po wstępnej redukcji przez pancerz.<br>
• Obrażenia te są redukowane przez <i>Fizyczną Osłonę</i>.<br>
• Mogą być zwiększane przez siłę po nauczeniu specjalnego efektu. Siła zwiększa wówczas minimalne i maksymalne obrażenia o stałą wartość.<br>
<br>
<b>Obrażenia dystansowe</b> (<code>a1, a2</code>)<br>
• W logu walki kolorowane na zielono.<br>
• Obecne tylko jako atrybut broni dystansowej.<br>
• Wartość obrażeń losowana jest między wartością minimalną oraz maksymalną broni, a następnie sumowana efektem umiejętności, zwiększającym obrażenia za każdy posiadany punkt zręczności. Rozrzut w broniach wynosi 10% względem wartości średniej.<br>
• Są redukowane przez pancerz zgodnie ze wzorem:<br>
<code>dmg<sub>out</sub> = dmg<sub>in</sub> - ac * (1.13 - 0.31 * ac / dmg<sub>in</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>out</sub></code> - obrażenia zredukowane przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>in</sub></code> - obrażenia przed redukcją przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ac</code> - pancerz postaci atakowanej.<br>
• Absorpcja nie redukuje obrażeń dystansowych, jednak jej skuteczność może zostać zwiększona poprzez efekt <code>absorbd</code>.<br>
• Obrażenia te są redukowane przez <i>Fizyczną Osłonę</i>.<br>
• Występują również w efekcie umiejętności <i>Deszcz Strzał</i> (efekty <code>arrowrain, arrowrain_all-perw</code>).<br>
• <b><a href="https://youtube.com/shorts/cGIIDCF-ryg">Krótki film</a></b> streszczający mechanikę obrażeń dystansowych.<br>
• Mogą być zwiększane przez zręczność po nauczeniu specjalnego efektu. Zręczność zwiększa wówczas minimalne i maksymalne obrażenia o stałą wartość.<br>
<br>
<b>Obrażenia broni pomocniczej</b> (<code>of_a1, of_a2</code>)<br>
• W logu walki kolorowane na brązowo.<br>
• Obecne tylko jako atrybut broni pomocniczych.<br>
• Wartość obrażeń losowana jest między wartością minimalną oraz maksymalną broni, a następnie sumowana efektem umiejętności, zwiększającym obrażenia za każdy posiadany punkt siły. Rozrzut w broniach wynosi 10% względem wartości średniej.<br>
• Są redukowane przez pancerz zgodnie ze wzorem:<br>
<code>dmg<sub>out</sub> = dmg<sub>in</sub> - ac * (1.13 - 0.31 * ac / dmg<sub>in</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>out</sub></code> - obrażenia zredukowane przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>in</sub></code> - obrażenia przed redukcją przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ac</code> - pancerz postaci atakowanej.<br>
• Absorpcja nie redukuje obrażeń pomocniczych.<br>
• Obrażenia te są redukowane przez <i>Fizyczną Osłonę</i>.<br>
• Mogą być zwiększane przez siłę po nauczeniu specjalnego efektu. Siła zwiększa wówczas minimalne i maksymalne obrażenia o stałą wartość.<br>
<br>
<b>Obrażenia od ognia</b> (<code>fire</code>)<br>
• W logu walki kolorowane na czerwono.<br>
• Obecne tylko jako atrybut broni jednoręcznych, dwuręcznych, półtoraręcznych, dystansowych, różdżek, orbów magicznych, strzał oraz kołczanów.<br>
• Rozrzut obrażeń wynosi 20% względem wartości średniej.<br>
• Są redukowane przez pancerz zgodnie ze wzorem:<br>
<code>dmg<sub>out</sub> = dmg<sub>in</sub> - 0.5 * ac * (1.13 - 0.31 * 0.5 * ac / dmg<sub>in</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>out</sub></code> - obrażenia zredukowane przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>in</sub></code> - obrażenia przed redukcją przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ac</code> - pancerz postaci atakowanej.<br>
• Absorpcja magiczna redukuje do 90% wartości obrażeń od ognia po wstępnej redukcji przez pancerz.<br>
• Obrażenia te są redukowane przez odporność na ogień.<br>
• Obrażenia mogą być również rozłożone w czasie na skutek niektórych efektów umiejętności.<br>
• <b><a href="https://youtube.com/shorts/EMlG2z0ftUE">Krótki film</a></b> streszczający mechanikę obrażeń od ognia.<br>
• Mogą być zwiększane przez intelekt po nauczeniu specjalnego efektu. Intelekt zwiększa wówczas średnie obrażenia od ognia, czyli jest uwzględniany podczas liczenia rozrzutu obrażeń.<br>
<br>
<b>Obrażenia od zimna</b> (<code>frost1</code>)<br>
• W logu walki kolorowane na niebiesko.<br>
• Obecne tylko jako atrybut broni jednoręcznych, dwuręcznych, półtoraręcznych, dystansowych, różdżek, orbów magicznych, strzał oraz kołczanów.<br>
• Rozrzut obrażeń wynosi 0% względem wartości średniej.<br>
• Zawsze powodują efekt spowolnienia przeciwnika na 3 tury o wartości zależnej od typu broni oraz poziomu przedmiotu.<br>
• Są redukowane przez pancerz zgodnie ze wzorem:<br>
<code>dmg<sub>out</sub> = dmg<sub>in</sub> - 0.5 * ac * (1.13 - 0.31 * 0.5 * ac / dmg<sub>in</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>out</sub></code> - obrażenia zredukowane przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>in</sub></code> - obrażenia przed redukcją przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ac</code> - pancerz postaci atakowanej.<br>
• Absorpcja magiczna redukuje do 90% wartości obrażeń od zimna po wstępnej redukcji przez pancerz.<br>
• Obrażenia te są redukowane przez odporność na zimno.<br>
• Mogą być zwiększane przez intelekt po nauczeniu specjalnego efektu. Intelekt zwiększa wówczas średnie obrażenia od zimna.<br>
<br>
<b>Obrażenia od błyskawic</b> (<code>light</code>)<br>
• W logu walki kolorowane na żółto.<br>
• Obecne tylko jako atrybut broni jednoręcznych, dwuręcznych, półtoraręcznych, dystansowych, różdżek, orbów magicznych, strzał oraz kołczanów.<br>
• Obrażenia rosną o 2.5% względem obrażeń początkowych aż do 50%, wraz z każdym wykonanym w przeciwnika atakiem. Rozrzut obrażeń w broni wynosi 20%.<br>
• Są redukowane przez pancerz zgodnie ze wzorem:<br>
<code>dmg<sub>out</sub> = dmg<sub>in</sub> - 0.5 * ac * (1.13 - 0.31 * 0.5 * ac / dmg<sub>in</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>out</sub></code> - obrażenia zredukowane przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dmg<sub>in</sub></code> - obrażenia przed redukcją przez pancerz.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ac</code> - pancerz postaci atakowanej.<br>
• Absorpcja magiczna redukuje do 90% wartości obrażeń od błyskawic po wstępnej redukcji przez pancerz.<br>
• Obrażenia te są redukowane przez odporność na błyskawice.<br>
• Obrażenia mogą być również rozłożone w czasie na skutek niektórych efektów umiejętności.<br>
• Mogą być zwiększane przez intelekt po nauczeniu specjalnego efektu. Intelekt zwiększa wówczas maksymalne obrażenia od błyskawic.<br>
<br>
<b>Obrażenia od trucizny</b> (<code>poison1, of_poison1</code>)<br>
• W logu walki występują zawsze w sekcji obrażeń rozłożonych w czasie.<br>
• Obecne tylko jako atrybut broni jednoręcznych, dwuręcznych, półtoraręcznych, dystansowych, pomocniczych, strzał oraz kołczanów.<br>
• Są aplikowane na 5 tur po trafieniu przeciwnika obrażeniami o niezerowej wartości.<br>
• Wyzwalają się przed turą przeciwnika, na którego zostały zaaplikowane.<br>
• Obrażenia od broni głównej oraz broni pomocniczej (również w przypadku broni dystansowej i strzał) sumują się. Broń pomocnicza z obrażeniami od trucizny aplikuje efekt osobno względem broni głównej z obrażeniami od trucizny - trucizna od danej broni nie zostanie zaaplikowana, jeżeli obrażenia nią zadane będą zerowe.<br>
• Obrażenia nie są kumulowane - podczas walki grupowej, na przeciwnika aplikowane są zawsze obrażenia od trucizny o największej wartości.<br>
• Zawsze powodują efekt spowolnienia przeciwnika o wartości zależnej od typu broni oraz poziomu przedmiotu, utrzymujący się do momentu wygaśnięcia obrażeń.<br>
• Obrażenia te są redukowane przez odporność na truciznę.<br>
• <b><a href="https://youtube.com/shorts/gEsj3AgPmQ4">Krótki film</a></b> streszczający mechanikę trucizny.<br>
<br>
<b>Obrażenia od głębokiej rany</b> (<code>wound1, of_wound1</code>)<br>
• W logu walki występują zawsze w sekcji obrażeń rozłożonych w czasie.<br>
• Obecne tylko jako atrybut broni jednoręcznych, dwuręcznych, półtoraręcznych, dystansowych oraz pomocniczych.<br>
• Są aplikowane na 5 tur po trafieniu przeciwnika obrażeniami o niezerowej wartości w przypadku zajścia zdarzenia <i>Głęboka rana</i>.<br>
• Wyzwalają się przed turą przeciwnika, na którego zostały zaaplikowane.<br>
• W przypadku, gdy zostały zaaplikowane, każdorazowe zajście zdarzenia <i>Głęboka rana</i> w przypadku trafionego ciosu, przedłuża efekt obrażeń od głębokich ran o 2 tury (maksymalnie do 5 tur) oraz zwiększa jej obrażenia o 50% względem aplikowanej wartości obrażeń (maksymalnie do 100%).<br>
• Obrażenia od broni głównej oraz broni pomocniczej sumują się, jednak podlegają osobnym zdarzeniom (<i>Głęboka rana</i> oraz <i>Głęboka rana pomocnicza</i>).<br>
• Obrażenia są kumulowane - wartość obrażeń od głębokiej rany rośnie do maksymalnej obliczonej wartości. Maksymalna wartość obrażeń od głębokiej rany ustalana jest w momencie zajścia zdarzenia:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ <i>Głęboka rana</i>: ustala maksymalną wartość na dwukrotność obrażeń od głębokiej rany w broni głównej gracza wykonującego cios.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ <i>Głęboka rana pomocnicza</i>: ustala maksymalną wartość na dwukrotność obrażeń od głębokiej rany w broni pomocniczej gracza wykonującego cios.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ <i>Głęboka rana</i> oraz <i>Głęboka rana pomocnicza</i> (jednocześnie): ustala maksymalną wartość na dwukrotność sumy obrażeń od głębokiej rany w broni głównej oraz broni pomocniczej gracza wykonującego cios.<br>
W przypadku, gdy głęboka rana została już zaaplikowana, maksymalna wartość głębokiej rany jest nadpisywana tylko wtedy, kiedy jest większa od trwającej najwyższej wartości tego efektu. Każdy gracz nakładając efekt głębokiej rany, zwiększa wartość obrażeń tylko względem posiadanej przez siebie broni, jednak maksymalna wartość obrażeń jest wspólna dla wszystkich graczy w drużynie.<br>
• Jeżeli w ramach jednego ataku zaaplikowana zostanie jednocześnie trucizna oraz głęboka rana, przyrost obrażeń od głębokiej rany w ramach tej aplikacji jest dzielony przez 2. Obniżenie obrażeń nie następuje podczas nakładania głębokiej rany na cel, który już wcześniej został zatruty, o ile podczas ataku nie jest nakładana trucizna.<br>
• Obrażenia te są redukowane przez odporność na głęboką ranę.<br>
• Występują również w efektach <i>Ciężka rana</i> (<code>critwound</code>) oraz <i>Zranienie</i> (<code>injure</code>), których źródłem są umiejętności lub ciosy specjalne potworów, jednak podlegają innym zasadom obliczania obrażeń, czasu trwania oraz kumulacji.<br>
• <b><a href="https://youtube.com/shorts/89z2KUvvFjY">Krótki film</a></b> streszczający mechanikę głębokiej rany.<br>
<br>
<b>Obrażenia umiejętności</b><br>
• W logu walki występują zawsze w sekcji obrażeń od umiejętności.<br>
• Są wyzwalane w momencie użycia umiejętności posiadającej efekt <code>combo_dmg_hpp-target</code> lub <code>dmg-target_physical</code>.<br>
• Wyzwalane są przed turą postaci, która używa umiejętności i obliczane są niezależnie od ataku, który po nich występuje (tak jakby podczas ciosu występowały dwa osobne ataki obniżające punkty zdrowia przeciwnika).<br>
• Są redukowane wyłącznie przez efekty osłabiające wszelkie źródła obrażeń, takich jak efekt umiejętności <i>Strach</i> (<code>dmg_from_player_per</code>) czy <i>Toksyczny Wstrząs/Toksyczne Opary</i> (<code>poison_lowdmg_per-enemies</code>).<br>
<br>
<h3><span class="color-blue">Typy obrażeń rozłożonych w czasie</span></h3><br><table id="t31" style="width:500px">
<tbody><tr><th colspan="6" style="background-color:#546dd2"><center>Zachowanie obrażeń rozłożonych w czasie</center></th></tr><tr><th><center>Typ obrażeń</center></th><th><center>Nadpisywanie</center></th><th><center>Kumulacja</center></th><th><center>Wzmocnienie</center></th><th><center>Źródło</center></th><th><center>Redukcja</center></th></tr><tr><th><center>Ogień</center></th><td><center><span style="color:green">Tak</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center>Umiejętność wymagająca obrażeń od ognia</center></td><td><center>Odporność na ogień</center></td></tr><tr><th><center>Błyskawice</center></th><td><center><span style="color:green">Tak</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center>Umiejętność wymagająca obrażeń od błyskawic</center></td><td><center>Odporność na błyskawice</center></td></tr><tr><th><center>Trucizna</center></th><td><center><span style="color:red">NIE</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center><span style="color:green">TAK</span></center></td><td><center>Bronie i umiejętności aplikujące truciznę</center></td><td><center>Odporność na truciznę</center></td></tr><tr><th><center>Głęboka rana</center></th><td><center><span style="color:red">NIE</span></center></td><td><center><span style="color:green">TAK</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center>Zdarzenie <i>głębokiej rany</i> i <i>głębokiej rany pomocniczej</i></center></td><td><center>Odporność na głęboką ranę</center></td></tr><tr><th><center>Zranienie</center></th><td><center><span style="color:green">TAK</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center><span style="color:red">NIE</span></center></td><td><center>Zdarzenie <i>zranienia</i> i <i>ciężkiej rany</i></center></td><td><center>Odporność na głęboką ranę</center></td></tr></tbody></table><br><br>
<b>Nadpisywanie</b><br>
W przypadku, gdy obrażenia rozłożone w czasie, tego samego typu, zostały już zaaplikowane, ich obrażenia zostają nadpisane. Brak tej mechaniki oznacza, że liczą się tylko obrażenia najwyższe, a kolejne zaaplikowanie obrażeń tylko przedłuża ich czas trwania.<br>
<br>
<b>Kumulacja</b><br>
Po nastąpieniu zdarzenia ustalana jest <b>maksymalna wartość</b> obrażeń jakie dany efekt może osiągnąć, która jest dwukrotnością obrażeń silnikowych. Maksymalna wartość jest nadpisywana wyłącznie wtedy, gdy nowa dwukrotność wartości silnikowej, ze zdarzeń występujących w danym ciosie, jest wyższa. W przypadku, gdy podczas jednego ciosu występują zarówno zdarzenia głębokiej rany i głębokiej rany pomocniczej, maksymalną wartością jest dwukrotność sumy silnikowych obrażeń od głębokiej rany i głębokiej rany pomocniczej. W innym wypadku wartość maksymalnych obrażeń ustalana jest tylko od tych obrażeń, do których zdarzenia doszło.<br>
Czas trwania obrażeń tej klasy po ich zaaplikowaniu nie jest równy czasowi jej przedłużania. W przypadku głębokiej rany czas trwania po aplikacji wynosi 5 tur, zaś każde zdarzenie przedłuża czas trwania o 2 tury.<br>
<br>
<b>Wzmocnienie</b><br>
Obrażenia opisane tą mechaniką wyłączają <b>mechanikę wyższej wartości</b>. Po zaaplikowaniu wzmocnionych obrażeń (jak wzmocniona trucizna), kolejne udane ciosy, które aplikowałyby truciznę, nie przedłużają czasu jej trwania. Oznacza to, że wzmocnione obrażenia są zadawane do momentu zakończenia czasu ich trwania, a następnie wygasają, o ile nie została do tego czasu zaaplikowana kolejna umiejętność zwiększająca jej obrażenia. <br>
<br>
<b>Zdarzenie ciężkiej rany i zranienia</b><br>
Obrażenia obu zdarzeń ustalane są w chwili redukcji obrażeń wykonanych przez wszystkie modyfikatory defensywne. Wymagają niezerowych obrażeń zadanych w przeciwnika, by mogły zostać zaaplikowane.<br>
<br>
<br><br>
<h3><span class="color-blue">Atrybuty podstawowe</span></h3><b>Profesja postaci</b><br>
• Jest to nazwa oraz jednoliterowy skrót profesji postaci. Postać gracza może mieć jedną z następujących profesji:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o Tancerz ostrzy (<code>b</code>)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o Wojownik (<code>w</code>)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o Paladyn (<code>p</code>)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o Mag (<code>m</code>)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o Tropiciel (<code>t</code>)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o Łowca (<code>h</code>)<br>
• Jest widoczna zaraz obok poziomu w każdym dymku lub sekcji informacji o postaci gracza.<br>
• Odpowiada za listę umiejętności, jakiej nauczyć może się postać.<br>
• Umożliwia noszenie przedmiotów, których wymagania odnoszące się do profesji zostały określone przez projektanta.<br>
• Wpływa na liczbe <i>punktów honoru</i>, jaką można uzyskać (lub stracić) za wygraną (bądź przegraną) walkę.<br>
• Wpływa na niektóre dialogi postaci niezależnych. Część dialogów, zadań lub zdarzeń losowych może się różnić w zależności od profesji postaci gracza.<br>
• Może zostać zmieniona u <i>Dalhara</i> w <i>Ratuszu Karka-han</i> za Smocze Łuski pod warunkiem, że poziom postaci jest wyższy niż 19. <b><a href="https://youtube.com/shorts/Y3JqM_8LyZ4">Krótki film</a></b> opisujący proces zmiany profesji.<br>
<br>
<b>Poziom postaci</b> (<code>lvl</code>)<br>
• Jest to atrybut jawny, wyświetlany przy postaci w grze oraz na profilu gracza. Wyjątkiem są <a href="https://pomoc.margonem.pl/index/view,268">światy fabularne</a>, gdzie poziom postaci w grze zostaje zamieniony na tytuł.<br>
• Ulega zmianie wyłącznie na skutek <i>Awansu poziomowego</i>, czyli przekroczenia wymaganej puli punktów doświadczenia. Wyjątkiem są światy zawodowe, na których poziom gracza może zostać cofnięty do pierwszego w wyniku śmierci postaci.<br>
• Wpływa na liczbę punktów <i>Zdrowia</i> postaci zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp (lvl) = 20 * min(lvl , 300)^1.375</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp</code> - podstawowa pula punktów zdrowia postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom postaci gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja minimum.<br>
• Wpływa w sposób stały na szansę na <i>Cios krytyczny</i> postaci zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>crit (lvl) [%] = 1 + 0.02 * lvl</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>crit</code> - podstawowa szansa na cios krytyczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom postaci gracza (postacie z poziomem przekraczającym 300 są traktowane tak, jakby miały poziom 300).<br>
• Wpływa na szansę na <i>Cios krytyczny</i> postaci gracza podczas walki, zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>crit<sub>gain</sub> [%] = sign(lvl<sub>player</sub> - lvl<sub>enemy</sub>) * max(abs(lvl<sub>player</sub> - lvl<sub>enemy</sub>) - 5, 0) * 3</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>crit<sub>gain</sub></code> - przyrost szansy na cios krytyczny gracza (może być ujemny).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>player</sub></code> - poziom postaci gracza (postacie z poziomem przekraczającym 300 są traktowane tak, jakby miały poziom 300).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>enemy</sub></code> - poziom postaci przeciwnika (postacie z poziomem przekraczającym 300 są traktowane tak, jakby miały poziom 300).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sign</code> - funkcja znaku (wynikiem jest 1, 0 lub -1).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja minimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>abs</code> - funkcja wartości bezwzględnej.<br>
• Wpływa na <i>Siłę ciosu krytycznego</i> (zarówno fizycznego jak i magicznego) postaci gracza podczas walki, zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critval<sub>gain</sub> [%] = min(300 , sign(lvl<sub>player</sub> - lvl<sub>enemy</sub>) * max(abs(lvl<sub>player</sub> - lvl<sub>enemy</sub>) - 5, 0) * 10)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critval<sub>gain</sub></code> - przyrost siły ciosu krytycznego fizycznego oraz magicznego (może być ujemny).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>player</sub></code> - poziom postaci gracza (postacie z poziomem przekraczającym 300 są traktowane tak, jakby miały poziom 300).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>enemy</sub></code> - poziom postaci przeciwnika (postacie z poziomem przekraczającym 300 są traktowane tak, jakby miały poziom 300).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sign</code> - funkcja znaku (wynikiem jest 1, 0 lub -1).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja minimum.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>abs</code> - funkcja wartości bezwzględnej.<br>
• Wpływa na siłę, zręczność oraz intelekt postaci w zależności od jej profesji. Każdy awans poziomowy (poniżej poziomu 301) zwiększa następujące atrybuty podstawowe:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;wojownikowi:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 4 punkty siły i 1 punkt zręczności - przed awansem na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 5 punktów siły - po awansie na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;paladynowi:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 2 punkty siły, 2 punkty intelektu i 1 punkt zręczności - w trakcie awansu na parzysty poziom, przed awansem na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 3 punkty siły, 2 punkty intelektu - w trakcie awansu na nieparzysty poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 2 punkty siły, 3 punkty intelektu - w trakcie awansu na parzysty poziom, po awansie na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;magowi:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 3 punkty intelektu, 1 punkt siły, 1 punkt zręczności - przed awansem na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 5 punktów zręczności - po awansie na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tropicielowi:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 1 punkt siły, 2 punkty intelektu i 2 punkty zręczności - przed awansem na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 2 punkty intelektu i 3 punkty zręczności - w trakcie awansu na nieparzysty poziom, po awansie na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 3 punkty intelektu i 2 punkty zręczności - w trakcie awansu na parzysty poziom, po awansie na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;łowcy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 1 punkty siły i 4 punkty zręczności - przed awansem na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 5 punktów zręczności - po awansie na 21 poziom<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tancerzowi:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 3 punkty siły i 2 punkty zręczności - w trakcie awansu na nieparzysty poziom lub przed awansem na 21 poziom <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;o 2 punkty siły i 3 punkty zręczności - w trakcie awansu na parzysty poziom oraz po awansie na 21 poziom <br>
<br>
<b>Siła</b> (<code>st</code>)<br>
• Ulega zmianie na skutek zmiany poziomu i zmiany ekwipunku.<br>
• Każda postać otrzymuje bazowo 4 punkty siły.<br>
• Wpływa w sposób stały na pulę punktów <i>Zdrowia</i> zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp<sub>gain</sub> = ds * 5</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp<sub>gain</sub></code> - przyrost punktów zdrowia postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ds</code> - liczba punktów siły postaci.<br>
• Wpływa dodatkowo na pulę punktów <i>Zdrowia</i>, jeżeli gracz wyekwipuje zbroję dostępną tylko dla profesji wojownika oraz paladyna, która posiada natywny atrybut, oferujący dodatkowe punkty życia za każdy zgromadzony punkt siły. Wartość dodatkowych punktów zdrowia wyraża się wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp<sub>gain</sub> = ds * lvl<sub>item</sub> * 0.1</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp<sub>gain</sub></code> - przyrost punktów zdrowia postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ds</code> - liczba punktów siły postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>item</sub></code> - poziom zbroi (dostępnej dla wojownika, paladyna lub łączonej dla paladyna i wojownika).<br>
• Wpływa dodatkowo na pulę punktów <i>Zdrowia</i>, jeżeli gracz nauczy się umiejętności z efektem <code>hpbon</code>, który oferuje dodatkowe punkty życia za każdy zgromadzony punkt siły.<br>
• Wpływa w sposób stały na <i>Siłę ciosu krytycznego fizycznego</i> powyżej 20 poziomu postaci zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critval<sub>gain</sub> = ds / (0.5 * min( lvl , 300))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critval<sub>gain</sub></code> - przyrost siły ciosu krytycznego fizycznego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ds</code> - liczba punktów siły postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja matematyczna minimum.<br>
• Wpływa w sposób stały na obrażenia, jeżeli gracz nauczy się umiejętności z efektami <code>str1h, str2h, of-str</code>, które oferują dodatkowe punkty obrażeń do określonego typu ataku za każdy punkt siły. Siła zwiększa obrażenia minimalne i maksymalne o tę samą stałą, w konsekwencji rozrzut obrażeń po uwzględnieniu dodatkowych punktów ataku z siły, jest taki sam co do wartości.<br>
<br>
<b>Intelekt</b> (<code>it</code>)<br>
• Ulega zmianie na skutek zmiany poziomu i zmiany ekwipunku.<br>
• Każda postać otrzymuje bazowo 3 punkty intelektu.<br>
• Wpływa w sposób stały na granicę możliwych do pozyskania punktów <i>Absorpcji</i> oraz <i>Absorpcji magicznej</i> zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>absorb<sub>limit</sub> = di * 7</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>hp<sub>gain</sub></code> - granica puli punktów absorpcji oraz absorpcji magicznej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>di</code> - liczba punktów intelektu postaci.<br>
• Wpływa w sposób stały na <i>Siłę ciosu krytycznego magicznego</i> powyżej 20 poziomu postaci zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critmval<sub>gain</sub> = di / (0.5 * min( lvl , 300))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>critmval<sub>gain</sub></code> - przyrost siły ciosu krytycznego magicznego.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>di</code> - liczba punktów intelektu postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja matematyczna minimum.<br>
• Wpływa w sposób stały na pulę punktów <i>Many</i>, jeżeli gracz nauczy się umiejętności z efektem <code>manastr</code>, która oferuje dodatkowe punkty many za każdy zgromadzony punkt intelektu.<br>
• Wpływa w sposób stały na obrażenia, jeżeli gracz nauczy się umiejętności z efektami <code>firebon, frostbon, lightbon</code>, które oferują dodatkowe punkty obrażeń do określonego typu ataku za każdy punkt intelektu. Intelekt zwiększa obrażenia średnie przypadające dla każdego posiadanego typu obrażeń od żywiołów (ogień, zimno, błyskawice), w konsekwencji rozrzut obrażeń po uwzględnieniu dodatkowych punktów ataku z intelektu, jest procentowo taki sam dla danego typu ataku.<br>
<br>
<b>Zręczność</b> (<code>ag</code>)<br>
• Ulega zmianie na skutek zmiany poziomu i zmiany ekwipunku.<br>
• Każda postać otrzymuje bazowo 3 punkty zręczności.<br>
• Wpływa w sposób stały na <i>Szybkość ataku</i> zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sa = min(2, 0.02 * dz) + max(0, 0.002 * (dz - 100))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sa</code> - szybkość ataku postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dz</code> - liczba punktów zręczności postaci.<br>
• Wpływa w sposób stały na <i>Unik</i> postaci zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>evade<sub>gain</sub> = dz / 30</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>evade<sub>gain</sub></code> - przyrost punktów uniku postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>dz</code> - liczba punktów zręczności postaci.<br>
• Wpływa w sposób stały na obrażenia, jeżeli gracz nauczy się umiejętności z efektem <code>agi</code>, która oferuje dodatkowe punkty obrażeń do określonego typu ataku za każdy punkt zręczności. Zręczność zwiększa obrażenia minimalne i maksymalne o tę samą stałą, w konsekwencji rozrzut obrażeń po uwzględnieniu dodatkowych punktów ataku ze zręczności, jest taki sam co do wartości.<br>
<br>
<b>Życie</b> (<code>hp</code>)<br>
• Ulega zmianie na skutek zmiany poziomu, zmiany ekwipunku, umiejętności pasywnych, umiejętności aktywnych oraz pośrednio zmiany poziomu.<br>
• Określa poziom zdrowia postaci. Gdy życie podczas walki spada poniżej 1 punktu, postać umiera.<br>
• Każda postać otrzymuje bazowo 20 punktów życia.<br>
• Liczba punktów życia po rozpoczęciu walki jest nie mniejsza niż bieżący poziom zdrowia, jaki posiada postać w czasie wolnej rozgrywki, natomiast punkty życia po powrocie z walki do rozgrywki są co do wartości równe punktom życia z jakimi postać zakończyła walkę (nie mniej niż 1). Za wszelką manipulację punktami zdrowia po zakończeniu walki odpowiadają talizmany leczące.<br>
• Podczas walki używana jest zarówno wartość bieżąca poziomu punktów życia, jak i wartość maksymalna puli punktów zdrowia do obliczania siły efektów umiejętności.<br>
• Wszelkie źródła leczenia w czasie walki nie mogą podnieść puli zdrowia postaci ponad poziom, z którym rozpoczynała ona walkę.<br>
<i>Przykład:</i> Posiadając w czasie wolnej rozgrywki 800/1000 punktów zdrowia, po rozpoczęciu walki postać ma 80% paska zdrowia. Po użyciu w pierwszej turze umiejętności <i>Leczenie ran</i>, która przywraca 300 punktów zdrowia wciąż poziom paska zdrowia postaci będzie wynosił 80%.<br>
• Życie w trakcie walki może zostać przywrócone poprzez atrybut leczący przed każdą turą postaci, efekty umiejętności oraz specjalne mikstury używane podczas pojedynków.<br>
<br>
<b>Szybkość ataku</b> (<code>sa</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności pasywnych, umiejętności aktywnych oraz pośrednio zmiany poziomu.<br>
• Odpowiada za pierwszeństwo wykonania ruchu oraz przewagę w liczbie tur nad przeciwnikiem. Oblicza się za jej pomocą czas trwania ataku postaci - im krótszy jest czas trwania ataku, tym więcej akcji wykona postać przed akcją pozostałych graczy. Działanie szybkości ataku zostało dokładnie opisane w sekcji dotyczącej <a href="#k21">kolejności wykonywania tur</a>. Czas trwania ataku można wyrazić przy użyciu uproszczonego wzoru:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>at = 1 / (sa + 1)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>at</code> - czas trwania ataku postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sa</code> - szybkość ataku postaci.<br>
• Atrybut przedstawiany zwykle w postaci liczby rzeczywistej zaokrąglonej do 2 miejsc dziesiętnych.<br>
• Każda postać otrzymuje bazowo 1.0 szybkości ataku.<br>
• Na szybkość ataku wpływają:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przyspieszenia o wartości procentowej (np: <i>Szybki atak, Błyskawiczny cios</i>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Spowolnienia o wartości procentowej (np: <i>Szadź, Krytyczne spowolnienie</i>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Spowolnienia o wartości stałej (np: spowolnienie od trucizny i magii zimna).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Obniżanie szybkości ataku z ekwipunku przeciwnika o wartości stałej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Redukcja spowolnień o wartościach stałych z efektu <code>redslow</code> (np: <i>Twarda głowa</i>).<br>
• Na podstawie szybkości ataku ulega również skrócenie czasu trwania ataku z efektu <code>red-sa</code> (np: <i>Błyskawiczny strzał</i>).<br>
• W przypadku, gdy wszystkie postacie uczestniczące w walce mają tę samą wartość szybkości ataku, turę rozpoczyna gracz inicjujący walkę.<br>
<br>
<b>Obniżanie szybkości ataku przeciwnika</b> (<code>slow</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Odpowiada za zmniejszanie szybkości ataku przeciwnika. Bieżąca szybkość ataku postaci podczas walki nie może spaść poniżej 33% jej wartości bazowej.<br>
• Atrybut kumuluje się z dowolnej liczby przedmiotów.<br>
• W trakcie walki grupowej, postać objęta jest działaniem efektu obniżenia szybkości ataku jedynie ze źródeł przedmiotów należących do gracza, który nałożył na cel największą wartość obniżenia.<br>
• Efekt działa przez całą walkę od momentu trafienia przeciwnika do momentu nadpisania wartości przez atak innego gracza (w przypadku, gdy wartość obniżania szybkości ataku jest wyższa) lub oczyszczenia spowolnień na skutek <i>Płomiennego oczyszczenia</i>, umiejętności z efektem <code>removeslow-allies</code> lub umiejętności NPC oczyszczających ze spowolnień.<br>
• Jest redukowane przez efekt <code>redslow</code> zmniejszający spowolnienia z umiejętności.<br>
• <b><a href="https://youtube.com/shorts/j7MctZ1ISoU">Krótki film</a></b> omawiający różnicę między spowolnieniem, a obniżaniem szybkości ataku.<br>
<br>
<b>Spowolnienie</b> (<code>poison0, of_poison0, frost0</code>)<br>
• Występuje wyłącznie i zawsze w parze z obrażeniami od trucizny lub zimna.<br>
• Ulega zmianie na skutek zmiany ekwipunku oraz umiejętności aktywnych.<br>
• Odpowiada za zmniejszanie szybkości ataku przeciwnika. Bieżąca szybkość ataku postaci podczas walki nie może spaść poniżej 33% jej wartości bazowej.<br>
• Źródłem atrybutu jest przedmiot o najwyższej wartości spowolnienia.<br>
• Efekt spowolnienia, którego źródłem jest magia zimna, trwa przez trzy tury od momentu trafienia przeciwnika. Zostaje on nałożony na przeciwnika podczas celnego ciosu nawet w przypadku, gdy obrażenia wynoszą zero.<br>
• Efekt spowolnienia, którego źródłem jest trucizna, trwa przez cały czas trwania trucizny i wymaga, by trucizna została nałożona na postać. Istnieją efekty zdejmujące jedynie spowolnienie z postaci - trucizna będzie wówczas wciąż zadawała obrażenia, ale straci zdolność do spowalniania.<br>
• Efekt kumuluje się do 2 wystąpień z 2 różnych źródeł i trwa do momentu nadpisania wartości przez atak trzeciej postaci (w przypadku, gdy wartość spowolnienia jest wyższa) lub oczyszczenia spowolnień na skutek <i>Płomiennego oczyszczenia</i>, umiejętności z efektem <code>removeslow-allies</code> lub umiejętności NPC oczyszczających ze spowolnień.<br>
• Może być wzmocnione przez efekty umiejętności. <br>
• Jest redukowane przez efekt <code>redslow</code> zmniejszający spowolnienia z umiejętności. Spowolnienie wynikające z samego wzmocnienia nie jest redukowane.<br>
• Oczyszczenie samego spowolnienia od trucizny powoduje, że obrażenia od trucizny wciąż są wyzwalane, jednak spowolnienie zostaje trwale usunięte do momentu kolejnego zaaplikowania go na postać.<br>
• <b><a href="https://youtube.com/shorts/j7MctZ1ISoU">Krótki film</a></b> omawiający różnicę między spowolnieniem, a obniżaniem szybkości ataku.<br>
<br>
<b>Leczenie</b> (<code>heal</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku oraz umiejętności.<br>
• Polega na nałożeniu na postać efektu rozłożonego w czasie, który trwa przez całą walkę lub do momentu obniżenia wartości efektu do zera.<br>
• Efekt przywraca punkty zdrowia postaci o wartość równą bieżącej wartości leczenia. <br>
• Warunkiem wyzwolenia efektu jest posiadanie w bieżącej turze mniej życia niż poziom zdrowia z jakim postać rozpoczynała walkę.<br>
• Wartość efektu maleje o 5% względem początkowej wartości leczenia po każdym wyzwoleniu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>heal<sub>n+1</sub> = heal<sub>n</sub> - 0.05 * heal<sub>init</sub> = heal<sub>init</sub> * (1 - 0.05 * n)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>heal<sub>n+1</sub></code> - wartość leczenia wyzwalana w następnej turze.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>heal<sub>n</sub></code> - bieżąca wartość leczenia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>heal<sub>init</sub></code> - wartość leczenia, z którym postać rozpoczynała walkę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;n - liczba wykonanych tur.<br>
• Efekt nie może przywrócić więcej życia niż poziom, z którym postać rozpoczynała walkę - wartość leczenia jest odpowiednio pomniejszana, jednak osłabienie leczenia po wyzwoleniu wciąż wynosi 5%. <br>
• Efekt leczenia wyzwala się tylko przed wykonaniem akcji przez gracza, do którego jest przypisany i tylko w przypadku, gdy spełniony jest warunek wyzwolenia.<br>
• Wartość leczenia może być osłabiona przez stałe modyfikatory (pochodzące z ekwipunku przeciwnika jak atrybut <code>lowhealenemy</code>) lub procentowe modyfikatory (pochodzące z umiejętności przeciwnika jak efekty <code>heal_per-enemies, critpoison_per</code>).<br>
• Wartość leczenia może być wzmocniona przez procentowe modyfikatory, których źródłem są umiejętności gracza lub sojusznika (efekt <code>heal_per-allies</code>).<br>
<b><a href="https://youtube.com/shorts/U2-FShNIGF4">Krótki film</a></b> streszczający mechanikę leczenia.<br>
• Istnieje bonus w przedmiocie (<code>adest</code>), który zmniejsza początkowe leczenie posiadacza. Skumulowana wartość leczenia nie może jednak spaść poniżej zera.<br>
<br>
<b>Energia</b> (<code>energy</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku oraz umiejętności.<br>
• Jest zasobem wykorzystywanym przez część umiejętności zawierających efekt <code>energy</code>.<br>
• Podczas walki bieżąca ilość punktów energii może się zmieniać od wartości początkowej, z którą postać rozpoczynała walkę, do zera.<br>
• Każda postać otrzymuje bazowo 50 punktów energii.<br>
• Może być generowana wraz z każdą turą gracza przez efekt <code>energygain</code>.<br>
• Może być przywracana o stałą wartość przez efekt <code>en-regen</code>.<br>
• Może być przywracana o pewną część przez niektóre efekty umiejętności (efekty <code>energyrestore_per</code>, <code>engback</code>).<br>
• Może być redukowana przez efekty niszczenia energii z ekwipunku przeciwnika (atrybut <code>enfatig, endest</code>) lub umiejętności przeciwnika (efekt <code>manaendest</code>).<br>
<br>
<b>Mana</b> (<code>mana</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku oraz umiejętności.<br>
• Jest zasobem wykorzystywanym przez część umiejętności zawierajacych efekt <code>mana</code>.<br>
• Podczas walki bieżąca ilość punktów many może się zmieniać od wartości początkowej, z którą postać rozpoczynała walkę, do zera.<br>
• Może być generowana wraz z każdą turą gracza przez efekt <code>managain</code>.<br>
• Może być zwiększana za każdy posiadany przez postać punkt intelektu przez umiejętność z efektem <code>manastr</code>.<br>
• Może być przywracana o pewną część przez umiejętność z efektem <code>manarestore_per</code>.<br>
• Może być redukowana przez efekty niszczenia many z ekwipunku przeciwnika (atrybut <code>manafatig, manadest</code>) lub umiejętności przeciwnika (efekty <code>manaendest</code>, <code>stealmana_per</code>).<br>
<br>
<b>Siła ciosu krytycznego fizycznego/magicznego/pomocniczego</b> (<code>critval, critmval, critmval2, of-critval</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności, poziomu oraz różnicy poziomowej między postaciami toczącymi ze sobą walkę.<br>
• Atrybut przedstawiany zwykle w postaci liczby rzeczywistej zaokrąglonej do 2 miejsc dziesiętnych.<br>
• Każda postać otrzymuje bazowo 1.20 siły ciosu krytycznego zarówno fizycznego jak i magicznego.<br>
• Atrybut zwiększa siłę ciosu w przypadku zajścia zdarzenia <i>cios krytyczny</i> podczas walki. Siła ciosu krytycznego fizycznego zwiększa siłę obrażeń fizycznych oraz dystansowych, natomiast siła ciosu krytycznego magicznego wzmacnia odpowiadające jej obrażenia od żywiołu (ogień, zimno, błyskawice).<br>
• Istnieją efekty, które zwiększają siłę ciosu krytycznego tylko określonego żywiołu, dlatego ich mocy ciosu krytycznego jest podzielona w zależności od typu ataku (<code>critmval2</code>).<br>
• Siła ciosu krytycznego, któa jest bonusem w broni pomocniczej, zwiększa siłę ciosu krytycznego tylko dla zdarzenia <i>Cios krytyczny pomocniczy</i>.<br>
<br>
<br><br>
<h3><span class="color-blue">Typy redukcji obrażeń</span></h3><b>Pancerz</b> (<code>ac</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Redukuje obrażenia od broni przeciwnika (fizyczne, pomocnicze, dystansowe, od ognia, zimna, błyskawic). Obrażenia magiczne (ogień, zimno, błyskawice) są redukowane w mniejszym stopniu.<br>
• Podczas walki może być zwiększany na skutek efektów umiejętności (na przykład: <i>Osłona tarczą</i>).<br>
• Podczas walki może być zmniejszany w wyniku posiadanego przez przeciwnika niszczenia pancerza, jednak maksymalnie do połowy swojej wartości początkowej.<br>
• Redukcja obrażeń następuje po obliczeniu zniszczenia pancerza w obrębie przyjmowanego ataku.<br>
• <b><a href="https://youtube.com/shorts/MKp1byWbRqE">Krótki film</a></b> streszczający mechanikę pancerza.<br>
<br>
<b>Odporności na żywioły: ogień, zimno, błyskawice</b> (<code>resfire, resfrost, reslight</code>)<br>
• Ulegają zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Redukują obrażenia od odpowiedniej magii - ognia, zimna lub błyskawic.<br>
• Podczas walki mogą być zwiększane na skutek efektów umiejętności (na przykład: <i>Aura ochrony</i>).<br>
• Podczas walki mogą być zmniejszane w wyniku posiadanego przez przeciwnika niszczenia odporności, jednak maksymalnie do zera. W przypadku posiadania większych odporności niż 90%, odporność obniża się bez ucięcia wartości (zniszczenie odporności o 1% ze 101% wynosi 100%).<br>
• Minimalna wartość odporności wynosi 0%.<br>
• Maksymalna wartość redukcji obrażeń magicznych wynosi 90%, jednak istnieje możliwość posiadania dowolnie wysokiej kumulacji tej statystyki.<br>
• Redukcja obrażeń następuje po obliczeniu zniszczenia odporności w obrębie przyjmowanego ataku.<br>
<br>
<b>Odporności na truciznę</b> (<code>act</code>)<br>
• Ulegają zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Redukują obrażenia od trucizny.<br>
• Podczas walki mogą być zwiększane na skutek efektów umiejętności.<br>
• Podczas walki mogą być zmniejszane w wyniku posiadanego przez przeciwnika niszczenia odporności na truciznę z efektu umiejętności (<code>actdmg</code>), jednak maksymalnie do zera. W przypadku posiadania większych odporności niż 90%, odporność obniża się bez ucięcia wartości (zniszczenie odporności o 1% ze 101% wynosi 100%).<br>
• Minimalna wartość odporności wynosi 0%.<br>
• Maksymalna wartość redukcji obrażeń wynosi 90%, jednak istnieje możliwość posiadania dowolnie wysokiej kumulacji tej statystyki.<br>
<br>
<b>Odporności na głęboką ranę</b> (<code>woundred</code>)<br>
• Ulegają zmianie na skutek zmiany umiejętności.<br>
• Redukują obrażenia od głębokiej rany oraz obrażeń rozłożonych w czasie zaaplikowanych w wyniku zdarzeń <i>Zranienie</i> i <i>Ciężka rana</i>.<br>
• Odporności nie można obniżyć w trakcie walki.<br>
• Minimalna wartość odporności wynosi 0%.<br>
• Maksymalna wartość redukcji obrażeń wynosi 90%, jednak istnieje możliwość posiadania dowolnie wysokiej kumulacji tej statystyki.<br>
<br>
<b>Absorpcja</b> (<code>absorb</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności i pośrednio poziomu.<br>
• Redukuje maksymalnie 75% obrażeń fizycznych, które w danym momencie redukcji przyjął na siebie gracz. W przypadku nieposiadania wystarczającej ilości absorpcji, by zredukować 75% obrażeń fizycznych, obrażenia są redukowane o pozostałą posiadaną przez postać absorpcję. Następnie o wartość zredukowanych obrażeń jest zmniejszana pula absorpcji użytecznej podczas walki.<br>
• Maksymalna wartość możliwej do skumulowania absorpcji wynosi siedmiokrotność posiadanego intelektu.<br>
• Absorpcja może być obniżania przez przeciwnika posiadającego przedmiot z atrybutem niszczenie absorpcji (<code>absdest</code>), jednak nie może być obniżona poniżej wartości 0.<br>
• Absorpcja może być generowana z każdym wykonanym ciosem o pewną część posiadanej puli absorpcji na skutek efektu umiejętności (<code>absagain_per</code>), jednak nie może przekroczyć wartości początkowej. Niszczenie absorpcji następuje przed redukcją obrażeń na skutek absorpcji.<br>
• Absorpcja może być również użyta do redukcji obrażeń dystansowych, jeżeli gracz nauczy się umiejętności posiadającej efekt wzrostu skuteczności absorpcji przeciw broni dystansowej (<code>absorbd</code>).<br>
<br>
<b>Absorpcja magiczna</b> (<code>absorbm</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności i pośrednio poziomu.<br>
• Redukuje maksymalnie 90% obrażeń od magii ognia, zimna oraz błyskawic, które w danym momencie redukcji przyjął na siebie gracz. W przypadku nieposiadania dość absorpcji by zredukować 90% obrażeń, są  one redukowane o pozostałą absorpcję magiczną. Następnie o wartość zredukowanych obrażeń jest zmniejszana pula absorpcji magicznej użytecznej podczas walki.<br>
• Maksymalna wartość możliwej do skumulowania absorpcji magicznej wynosi siedmiokrotność posiadanego intelektu.<br>
• Absorpcja magiczna może być obniżania przez przeciwnika posiadającego przedmiot z atrybutem niszczenie absorpcji (<code>absdest</code>), jednak nie może być obniżona poniżej wartości 0.<br>
• Absorpcja magiczna może być generowana z każdym wykonanym ciosem o pewną część posiadanej puli absorpcji na skutek efektu umiejętności (<code>absagain_per</code>), jednak nie może przekroczyć wartości początkowej. Niszczenie absorpcji następuje przed redukcją obrażeń na skutek absorpcji magicznej.<br>
<br>
<a name="kkrd"></a><br>
<b>Kolejność redukcji obrażeń w ramach ciosu</b><br>
1. Efekty umiejętności osłabiające źródła obrażeń (np. umiejętności <i>Strach</i> lub <i>Toksyczne opary</i>) - wynik tych obliczeń jest w logu walki widoczny jako obrażenia wylosowane przez atakującego.<br>
2. Zdarzenia regularne niwelujące obrażenia (Unik, Parowanie, Blok strzały).<br>
3. Blok.<br>
4. Pancerz.<br>
5. Absorpcja i absorpcja magiczna.<br>
6. Odporności na żywioły.<br>
7. Odporności bonusów legendarnych (<i>Fasada opieki</i>, <i>Krytyczna osłona</i>).<br>
8. Pozostałe efekty zerujące obrażenia (na przykład efekt <code>immunity_to_dmg</code> umiejętności <i>Wewnętrzny spokój</i>) - wynik tych obliczeń jest w logu walki widoczny jako obrażenia zadane w przeciwnika.<br>
<br>
<a name="kkrdot"></a><br>
<b>Kolejność redukcji obrażeń efektów rozłożonych w czasie</b><br>
1. Efekty umiejętności osłabiające źródła obrażeń (np. umiejętności <i>Strach</i> lub <i>Toksyczne opary</i>) - kumulują się ze sobą addytywnie.<br>
2. Odporności na żywioły, truciznę i głęboką ranę.<br>
<br>
<br><br>
<h3><span class="color-blue">Obniżanie statystyk przeciwnika</span></h3><b>Niszczenie pancerza</b> (<code>acdmg</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Obniża pancerz atakowanego przeciwnika o stałą liczbę punktów.<br>
• Podczas ciosu pancerz ulega zmniejszeniu przed rozpoczęciem redukcji obrażeń.<br>
• Pancerz przeciwnika nie może spaść poniżej 50% wartości skumulowanego przez niego pancerza.<br>
• Niszczenie pancerza jest obniżane na skutek statystyki przeklętej (<code>resacdmg</code>) oraz efektu umiejętności (<code>redacdmg_per</code>).<br>
<br>
<b>Niszczenie odporności</b> (<code>acmdmg</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Obniża odporność na ogień, zimno oraz błyskawice u atakowanego przeciwnika o stałą liczbę punktów procentowych. Wszystkie odporności redukowane są jednocześnie.<br>
• Podczas ciosu odporności ulegają zmniejszeniu przed rozpoczęciem redukcji obrażeń.<br>
• W przypadku gdy przeciwnik posiada nadwyżkę, najpierw redukowana jest nadwyżka odporności na magię.<br>
• Odporność na magię u przeciwnika nie może zostać zmniejszona poniżej 0%.<br>
<br>
<b>Niszczenie absorpcji</b> (<code>absdest</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Obniża absorpcję oraz absorpcję magiczną atakowanego przeciwnika o stałą wartość przed obliczeniem redukcji obrażeń od absorpcji. Oba typy absorpcji są obniżane w tym samym czasie.<br>
• Przywracanie absorpcji z efektu umiejętności <code>absagain_per</code> następuje przed zniszczeniem absorpcji.<br>
• Absorpcja przeciwnika nie może zostać zredukowana poniżej wartość 0.<br>
• Niszczenie absorpcji może zostać zredukowane na skutek działania efektu umiejętności (<code>redabdest_per</code>).<br>
<br>
<b>Obniżanie uniku</b> (<code>lowevade</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Obniża unik atakowanego przeciwnika o stałą liczbę punktów.<br>
• Unik przeciwnika nie może zostać obniżony poniżej wartość 0.<br>
<br>
<b>Obniżanie szansy na cios krytyczny przeciwnika</b> (<code>lowcrit</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Obniża szansę na cios krytyczny oraz cios krytyczny pomocniczy u przeciwnika atakującego posiadacza statystyki o stałą liczbę punktów procentowych.<br>
• Nie wpływa na szansę zajścia zdarzenia Ciosu bardzo krytycznego.<br>
• Szansa na cios krytyczny przeciwnika nie może zostać obniżona poniżej wartość 1%.<br>
<br>
<b>Szansa na zniszczenie energii przeciwnikowi</b> (<code>enfatig</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Wraz z turą przeciwnika, losuje zdarzenie odebrania mu stałej liczby punktów energii.<br>
• Wartość niszczonej energii nie maleje wraz z kolejnymi zajściami zdarzenia.<br>
• Szansa na zajście zdarzenia nie może przekroczyć 100%.<br>
• Wartość niszczonej energii jest pobierana zawsze z przedmiotu, który posiada największą wartość tej statystyki.<br>
• W przypadku chybionego ataku, nie nastepuje wyzwolenie efektu tej statystyki.<br>
• Liczba punktów energii przeciwnika nie może spaść poniżej wartość 0.<br>
• Wartość niszczonej energii może zostać zredukowana przez statystykę przeklętą (<code>resmanaendest</code>) oraz efekt umiejętności (<code>reddest_per</code>).<br>
<br>
<b>Szansa na zniszczenie energii przeciwnikowi</b> (<code>manafatig</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Wraz z turą przeciwnika, losuje zdarzenie odebrania mu stałej liczby punktów many.<br>
• Wartość niszczonej many nie maleje wraz z kolejnymi zajściami zdarzenia.<br>
• Szansa na zajście zdarzenia nie może przekroczyć 100%.<br>
• Wartość niszczonej many jest pobierana zawsze z przedmiotu, który posiada największą wartość tej statystyki.<br>
• W przypadku chybionego ataku, nie nastepuje wyzwolenie efektu tej statystyki.<br>
• Liczba punktów many przeciwnika nie może spaść poniżej wartość 0.<br>
• Wartość niszczonej many może zostać zredukowana przez statystykę przeklętą (<code>resmanaendest</code>) oraz efekt umiejętności (<code>reddest_per</code>).<br>
<br>
<b>Słabnące niszczenie energii przeciwnika</b> (<code>endest</code>)<br>
• Jest to bonus wycofany z gry.<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Wraz z turą przeciwnika, odbiera mu stałą liczbę punktów energii.<br>
• Wartość niszczonej energii maleje z każdą turą o 5% względem skumulowanej wartości początkowej. Następuje zaokrąglenie matematyczne, także efekt może zaniknąć wcześniej niż po 20 turach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>endest<sub>n+1</sub> = endest<sub>n</sub> - 0.05 * endest<sub>init</sub> = endest<sub>init</sub> * (1 - 0.05 * n)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>endest<sub>n+1</sub></code> - wartość niszczenia energii wyzwalana w następnej turze.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>endest<sub>n</sub></code> - bieżąca wartość niszczenia energii.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>endest<sub>init</sub></code> - wartość niszczenia energii, z którym postać rozpoczynała walkę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;n - liczba wykonanych tur.<br>
• W przypadku chybionego ataku, nie nastepuje wyzwolenie efektu tej statystyki, jednak jest ona wciąż osłabiana na skutek zakończonej tury.<br>
• Liczba punktów energii przeciwnika nie może spaść poniżej wartość 0.<br>
• Wartość niszczonej energii może zostać zredukowana przez statystykę przeklętą (<code>resmanaendest</code>) oraz efekt umiejętności (<code>reddest_per</code>).<br>
<br>
<b>Słabnące niszczenie many przeciwnika</b> (<code>manadest</code>)<br>
• Jest to bonus wycofany z gry.<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Wraz z turą przeciwnika, odbiera mu stałą liczbę punktów many.<br>
• Wartość niszczonej many maleje z każdą turą o 5% względem skumulowanej wartości początkowej.  Następuje zaokrąglenie matematyczne, także efekt może zaniknąć wcześniej niż po 20 turach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>manadest<sub>n+1</sub> = manadest<sub>n</sub> - 0.05 * manadest<sub>init</sub> = manadest<sub>init</sub> * (1 - 0.05 * n)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>manadest<sub>n+1</sub></code> - wartość niszczenia many wyzwalana w następnej turze.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>manadest<sub>n</sub></code> - bieżąca wartość niszczenia many.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>manadest<sub>init</sub></code> - wartość niszczenia many, z którym postać rozpoczynała walkę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;n - liczba wykonanych tur.<br>
• W przypadku chybionego ataku, nie nastepuje wyzwolenie efektu tej statystyki, jednak jest ona wciąż osłabiana na skutek zakończonej tury.<br>
• Liczba punktów many przeciwnika nie może spaść poniżej wartość 0.<br>
• Wartość niszczonej many może zostać zredukowana przez statystykę przeklętą (<code>resmanaendest</code>) oraz efekt umiejętności (<code>reddest_per</code>).<br>
<br>
<br><br>
<h3><span class="color-blue">Regularne zdarzenia losowe</span></h3><b>Cios krytyczny</b> (<code>crit, of-crit</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności, poziomu oraz różnicy poziomów podczas walki.<br>
• Zdarzenie zachodzi podczas ataku.<br>
• Określa szansę na wyzwolenie wzmocnionego ataku broni, którego wartość jest przemnażana przez odpowiednio siłę ciosu krytycznego fizycznego (dla obrażeń fizycznych i dystansowych) oraz siłę ciosu krytycznego magicznego (dla obrażeń od ognia, zimna lub błyskawic).<br>
• Broń pomocnicza posiada własne zdarzenie - cios krytyczny broni pomocniczej, który odpowiednio wzmacnia obrażenia pomocnicze w zależności od posiadanej siły ciosu krytycznego fizycznego dla broni pomocniczych (obliczaną osobno względem siły ciosu krytycznego fizycznego).<br>
• Zawsze jest przedstawiany w postaci szansy na zajście zdarzenia, a każdy modyfikator jest przedstawiany jako wzrost/spadek punktów procentowych tej statystyki.<br>
• Szansa może być zwiększona w wyniku skorzystania z umiejętności posiadającej efekt aktywnego lub pasywnego warunkowego zwiększania szansy na cios krytyczny (<code>active_crit</code>, <code>lastcrit</code>).<br>
• Szansa może być zmniejszona na skutek statystyki obniżającej szansę na cios krytyczny z atrybutu <code>lowcrit</code>, będącego w ekwipunku przeciwnika, oraz na skutek umiejętności z efektami zmniejszającymi szansę na cios krytyczny (<code>disturb</code>, <code>stinkbomb</code>).<br>
• Minimalna szansa na cios krytyczny wynosi 1% i nie może zostać obniżona poniżej tej wartości. W przypadku posiadania szansy przewyższającej 100%, obniżenia szansy na cios krytyczny przez przeciwnika redukują również nadwyżkę.<br>
<br>
<b>Przebicie pancerza</b> (<code>pierce</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Zdarzenie zachodzi podczas ataku.<br>
• Zdarzenie sprawia, że w obrębie ciosu pancerz nie redukuje wartości obrażeń.<br>
• Broń pomocnicza jest liczona jako osobna instancja obrażeń, przez co obrażenia od niej nie ignorują pancerza mimo zajścia zdarzenia przebicia.<br>
• Szansa może być zwiększona w wyniku skorzystania z umiejętności posiadającej efekt aktywnego zwiększania szansy na przebicie pancerza.<br>
• Zawsze jest przedstawiane w postaci szansy na zajście zdarzenia, a każdy modyfikator jest przedstawiany jako wzrost/spadek punktów procentowych tej statystyki.<br>
• Szansa może być zmniejszona na skutek umiejętności z efektami zmniejszającymi szansę na przebicie pancerza (<code>disturb</code>).<br>
• Efekt zdarzenia może zostać wyłączony, jeżeli jednocześnie zajdzie zdarzenie <i>Bloku przebicia</i>, <i>Bloku</i> lub cios <b>Chybi</b> (zdarzenie <i>Uniku, Parowania, Bloku strzały</i>).<br>
<br>
<b>Głęboka rana</b> (<code>wound0, of_wound0</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku i umiejętności.<br>
• Zdarzenie zachodzi podczas ataku.<br>
• Zdarzenie powoduje próbę aplikacji obrażeń od głębokiej rany na 5 tur.<br>
• W przypadku, gdy głęboka rana została zaaplikowana przed zdarzeniem, kolejne wystąpienie zdarzenia powoduje próbę przedłużenia poprzedniego efektu o 2 tury oraz zwiększenia obrażeń, jeżeli nie osiągnęły jeszcze maksymalnej wartości.<br>
• Zawsze jest przedstawiana w postaci szansy na zajście zdarzenia, a każdy modyfikator jest przedstawiany jako wzrost/spadek punktów procentowych tej statystyki.<br>
• Efekt zdarzenia może zostać wyłączony w przypadku <b>chybienia</b> (zdarzenie <i>Uniku, Parowania, Bloku strzały</i>) lub zadania obrażeń zerowych - obrażenia nie zostaną zaaplikowane, a efekt nie zostanie przedłużony.<br>
• <b><a href="https://youtube.com/shorts/89z2KUvvFjY">Krótki film</a></b> streszczający mechanikę głębokiej rany.<br>
<br>
<b>Unik</b> (<code>evade</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności, pośrednio poziomu oraz różnicy poziomów podczas walki.<br>
• Zdarzenie zachodzi podczas obrony.<br>
• Przedstawiany jest w formie punktowej, który wpływa na szansę na zdarzenie w następujący sposób:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>evade [%] = evade<sub>points</sub> * 20 / min(lvl<sub>enemy</sub>, 300)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>evade</code> - szansa na zajście zdarzenia uniku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>evade<sub>points</sub> </code> - liczba punktów uniku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>enemy</sub></code> - poziom przeciwnika.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja matematyczna minimum.<br>
• Unik przedstawiany w postaci procentowej (na przykład w ramach efektów umiejętności) zawsze informuje o przyroście/spadku punktów procentowych atrybutu.<br>
• Zdarzenie powoduje zniwelowanie obrażeń od broni głównej przeciwnika, w obrębie ataku, do zera.<br>
• Zdarzenie prowadzi do efektu <i>chybienia</i>, który nie dopuszcza do zajścia następujących zdarzeń: <i>Ogłuszenie, Wytrącenie z równowagi, Klątwa, Oślepienie, Blok, Blok przebicia, Parowanie, Zranienie, Ciężka rana</i> oraz niektórych efektów umiejętności.<br>
• Zdarzenie wyłącza efekty następujących zdarzeń: <i>Głęboka rana, Przebicie pancerza</i>.<br>
• Obrażenia od broni pomocniczej nie mogą zostać uniknięte - atak nigdy nie chybi. Oznacza to, że zdarzenia <i>Głęboka rana pomocnicza, Cios krytyczny pomocniczy</i> nie mogą być zniwelowane poprzez zajście zdarzenia uniku.<br>
• Obrażenia od ciosów profesji mag nie mogą zostać uniknięte - atak nigdy nie chybi.<br>
• Maksymalna szansa na unik podczas walki wynosi 50%, jednak istnieje możliwość gromadzenia punktów w unik powyżej tej wartości. Efekty zmniejszające szansę na unik wpływają w pierwszej kolejności na nadwyżkę punktów.<br>
• Szansa może być zwiększona z faktu posiadania przez gracza umiejętności z efektami oferującymi dodatkowe punkty procentowe uniku po spełnieniu określonych warunków (efekt <code>adrenalin_evade_per</code>).<br>
• Szansa może być zmniejszona na skutek atrybutu <code>lowevade</code>, którego źródłem jest ekwipunek atakującej postaci oraz umiejętności z efektami zmniejszającymi w sposób aktywny oraz pasywny szansę na unik przeciwnika (<code>active_decevade_per</code>, <code>decevade_per</code>).<br>
<br>
<b>Blok</b> (<code>blok</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku, umiejętności oraz różnicy poziomów podczas walki.<br>
• Zdarzenie zachodzi podczas obrony.<br>
• Blok nigdy nie zajdzie, jeżeli postać nie jest wyposażona w tarczę.<br>
• Przedstawiany jest w formie punktowej, który wpływa na szansę na zdarzenie w następujący sposób:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>block [%] = block<sub>points</sub> * 20 / min(lvl<sub>enemy</sub>, 300)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>block</code> - szansa na zajście zdarzenia bloku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>block<sub>points</sub> </code> - liczba punktów bloku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>enemy</sub></code> - poziom przeciwnika.<br>
• Blok przedstawiany w postaci procentowej (na przykład w ramach efektów umiejętności) zawsze informuje o przyroście/spadku punktów procentowych atrybutu.<br>
• Zdarzenie powoduje zredukowanie obrażeń od broni głównej przeciwnika (zarówno obrażeń magicznych, fizycznych jak i pomocniczych) podczas przyjętego ataku o 30%.<br>
• Redukcja obrażeń podczas bloku następuje przed redukcją przez absorpcję, pancerz oraz odporności.<br>
• Zdarzenie nie dopuszcza do zajścia następujących zdarzeń: <i>Ogłuszenie, Parowanie</i>.<br>
• Zdarzenie wyłącza efekty następujących zdarzeń: <i>Przebicie pancerza</i>.<br>
• Maksymalna szansa na blok podczas walki wynosi 50%, jednak istnieje możliwość gromadzenia punktów w blok powyżej tej wartości.<br>
• Istnieją efekty umiejętności zmniejszające szansę na blok (<code>decblock_per, active_decblock_per, active_decblock_per-enemies</code>).<br>
<b><a href="https://youtube.com/shorts/uLYnivGDQOk">Krótki film</a></b> omawiający działanie bloku.<br>
<br>
<b>Blok przebicia</b> (<code>pierceb</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku (tarczy).<br>
• Zdarzenie zachodzi podczas obrony.<br>
• Zawsze jest przedstawiana w formie prawdopodobieństwa na zajście zdarzenia.<br>
• Zdarzenie zachodzi wyłącznie po zajściu zdarzenia <i>Przebicie pancerza</i> i powoduje wyłączenie wyzwalanych przez nie efektów.<br>
• Szansa na blok przebicia nie może być zmniejszona poprzez żadne umiejętności ani atrybuty.<br>
<br>
<b>Kontra</b> (<code>contra</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku oraz umiejętności.<br>
• Zdarzenie zachodzi podczas obrony.<br>
• Zawsze jest przedstawiana w formie prawdopodobieństwa na zajście zdarzenia, a każdy modyfikator jest przedstawiany jako wzrost/spadek punktów procentowych tej statystyki.<br>
• Zdarzenie zachodzi wyłącznie po zajściu zdarzenia <i>Cios krytyczny</i> lub <i>Cios krytyczny pomocniczy</i> i powoduje wymuszenie wykonania następnej tury w sposób automatyczny przez atakowaną postać. Podczas wymuszonej tury nie może zostać użyta żadna umiejętność.<br>
• Szansa na kontrę nie może być bezpośrednio zmniejszona poprzez żadne umiejętności ani atrybuty.<br>
<br>
<b>Ogłuszenie</b> (<code>stun</code>)<br>
• Zdarzenie wymagające posiadania odpowiedniej umiejętności.<br>
• Występuje również pod nazwami: Zamrożenie, Potężne ogłuszenie, Potężne przeszycie, Potężne porażenie, Potężne zamrożenie, Potężne poparzenie.<br>
• Nakłada na przeciwnika stan obezwładnienia, który automatycznie uniemożliwia wykonanie następnej tury przez postać. Czas trwania zablokowanej tury jest zależny od bieżącej szybkości ataku gracza.<br>
• Czas trwania ogłuszenia może zostać skrócony maksymalnie o 90% na skutek efektu umiejętności zmniejszającego czas trwania stanu obezwładnienia (<code>redstun</code>).<br>
• Efekty z przedrostkiem "Potężne", których źródłem są ciosy potworów, ogłuszają graczy na 2 tury.<br>
• Ogłuszenie nie może nastąpić jeśli cios przeciwnika <b>chybił</b> lub zaszło zdarzenie <i>Bloku</i>. Zdarzenia te zmniejszają więc szansę na ogłuszenie.<br>
• Ogłuszony przeciwnik przed zakończeniem stanu obezwładnienia (poprzez wykonanie najbliższej prawidłowej tury, która nie została przerwana) nie może wylosować zdarzenia <i>Kontry</i>, <i>Bloku</i>, <i>Uniku</i>, <i>Parowania</i> oraz <i>Bloku strzały</i>.<br>
<br>
<br><br>
<h3><span class="color-blue">Statystyki przeklęte</span></h3><b>Obniżanie niszczenia energii i many przeciwnika</b> (<code>resmanaendest</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Zmniejsza wartość niszczenia energii oraz niszczenia many z ekwipunku oraz umiejętności przeciwnika atakującego posiadacza statystyki o stałą wartość.<br>
• Redukcja następuje przed redukcją z efektu umiejętności (<code>reddest_per</code>).<br>
<br>
<b>Obniżanie niszczenia pancerza przeciwnika</b> (<code>resacdmg</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Zmniejsza wartość niszczenia pancerza z ekwipunku oraz umiejętności przeciwnika atakującego posiadacza statystyki o stałą wartość.<br>
• Redukcja następuje przed redukcją z efektu umiejętności (<code>redacdmg_per</code>).<br>
<br>
<b>Obniżanie siły ciosu krytycznego przeciwnika</b> (<code>lowcritallval</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Zmniejsza wartość siły ciosu krytycznego fizycznego, pomocniczego oraz magicznego przeciwnika atakującego posiadacza statystyki o stałą wartość.<br>
<br>
<b>Obniżanie leczenia przeciwnika</b> (<code>lowheal2turns</code>)<br>
• Ulega zmianie na skutek zmiany ekwipunku.<br>
• Zmniejsza wartość leczenia atakowanego przeciwnika o stałą wartość na 2 tury.<br>
• Działa wraz z każdym wyzwoleniem leczenia przeciwnika.<br>
<br>
<br><br>
<a name="k32"></a><b><h3>3.2. Budowa ekwipunku</h3></b><br>
<br>
Ekwipunek postaci składa się z dwóch głównych typów przedmiotów:<br>
• Przedmioty ekwipowalne umieszczane w odpowiednie gniazda, które oferują statystyki służące postaci w walce. Postać dysponuje 9 gniazdami na przedmioty ekwipowalne:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Broń główna (Jednoręczne, Dwuręczne, Półtoraręczne, Dystansowe, Różdżki),<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Broń pomocnicza (Pomocnicze, Tarcze, Orby magiczne, Kołczany, Strzały),<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Hełm,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Buty,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Rękawice,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Pierścień,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Naszyjnik,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Błogosławieństwo (wygasające z czasem).<br>
• Przedmioty nieekwipowalne, używane podczas rozgrywki swobodnej poprzez konsumpcję (teleporty lub mikstury), służące jako talizmany aktywowane tuż po walce (leczące lub przyspieszające powrót do zdrowia) oraz przedmioty neutralne. Postać ma do dyspozycji 3 gniazda na torby liczące do 42 miejsc oraz jedno gniazdo na specjalną torbę, liczącą do 42 miejsc, którą może być: torba na klucze, torba na walutę oraz torba na teleporty. <br>
<b><a href="https://youtube.com/shorts/8pxX7gwuxac">Krótki film</a></b> opisujący zastosowanie specjalnego miejsca na torbę.<br>
Można wymienić następujące klasy przedmiotów nieekwipowalnych:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Konsumpcyjne,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Neutralne,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Waluty,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Złoto,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Talizmany,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ulepszenia,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Questowe,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Książki,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Klucze,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Recepty,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Stroje,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Maskotki,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Teleporty,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Torby.<br>
<br>
<br>
<h3><span class="color-blue">Klasy przedmiotów ekwipowalnych</span></h3>Przedmioty ekwipowalne dzielą się na klasy. Każda klasa ma inne właściwości - różnią się typem oraz wartościami atrybutów natywnych oraz liczbą bonusów nadanych, które projektant może im rozdać. Niektóre atrybuty mogą być natywne dla części klas przedmiotów, ale można jednocześnie je nadać w ramach bonusów.<br>
Atrybuty w przedmiotach dzielą się na:<br>
• Atrybuty natywne - statystyki, które zawsze występują w przedmiocie o danej klasie, wymogach profesji oraz rzadkości. Możemy do nich zaliczyć: obrażenia fizyczne, obrażenia dystansowe, obrażenia pomocnicze, obrażenia od magii, obrażenia od trucizny, obrażenia od głębokiej rany, szansa na zajście zdarzenia głębokiej rany, odporności, absorpcja, absorpcja magiczna, pancerz, spowolnienie, niszczenie pancerza, niszczenie odporności, głęboka rana, trucizna, blok.<br>
• Bonusy nadane - statystyki, które zostały dobrane manualnie do przedmiotu. Możemy do nich zaliczyć: dodatkowe obrażenia, dodatkowa obrona, dodatkowy pancerz, dodatkowe odporności (ogień, zimno, błyskawice, trucizna), dodatkowa absorpcja, dodatkowa absorpcja magiczna, niszczenie absorpcji, cios krytyczny, siła ciosu krytycznego fizycznego, siła ciosu krytycznego magicznego, szybkość ataku, wszystkie cechy, intelekt, siła, zręczność, życie, leczenie, ranienie posiadacza, unik, blok, blok przebicia, kontra, przebicie pancerza, niszczenie pancerza, niszczenie odporności, obniżanie uniku, niszczenie energii, niszczenie many, obniżanie szansy na cios krytyczny przeciwnika.<br>
• Bonusy przeklęte - statystyki występujące tylko w przedmiotach przeklętych, posiadających określoną ilość i zużywające się o jedną sztukę wraz z zakończeniem walki. Możemy do nich zaliczyć: obniżanie leczenia przeciwnika, obniżanie niszczenia pancerza przeciwnika, obniżanie niszczenia energii oraz many przeciwnika, obniżanie siły ciosu krytycznego przeciwnika.<br>
<br>
Każdy przedmiot posiada określoną liczbę bonusów, które mogą mu zostać manualnie nadane. Część statystyk może przyjmować ujemne wartości (np: życie, unik), wobec czego mogą występować pod postacią <i>bonusów ujemnych</i>. Na każdy bonus ujemny przypada dodatkowy bonus zwyczajny w przedmiocie. Zestawienie liczby bonusów dla określonej klasy przedmiotów oraz dla danej rzadkości zostało przedstawione w poniższej tabeli. <br>
<b><a href="https://youtube.com/shorts/Sm9VX93eMc4">Krótki film</a></b> omawiający kwestię bonusów ujemnych.<br>
<br>
<br><table id="t321" style="width:500px">
<tbody><tr><th colspan="6" style="background-color:#546dd2"><center>Liczba bonusów w przedmiotach</center></th></tr><tr><th rowspan="2"><center>Klasa przedmiotu</center></th><th colspan="5"><center>Rzadkość</center></th></tr><tr><td style="background-color:grey">Pospolita</td><td style="background-color:#f3f213">Unikatowa</td><td style="background-color:#918fff">Heroiczna</td><td style="background-color:#fc4ab4">Ulepszona</td><td style="background-color:#ff603b">Legendarna</td></tr><tr><th><center>Jednoręczne</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Dwuręczne</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Półtoraręczne</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Dystansowe</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Pomocnicze</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Różdżki</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Orby magiczne</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Zbroje</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Hełmy</center></th><td><center>1</center></td><td><center>4</center></td><td><center>8</center></td><td><center>8</center></td><td><center>12</center></td></tr><tr><th><center>Buty</center></th><td><center>1</center></td><td><center>4</center></td><td><center>8</center></td><td><center>8</center></td><td><center>12</center></td></tr><tr><th><center>Rękawice</center></th><td><center>1</center></td><td><center>4</center></td><td><center>8</center></td><td><center>8</center></td><td><center>12</center></td></tr><tr><th><center>Pierścienie</center></th><td><center>5</center></td><td><center>9</center></td><td><center>13</center></td><td><center>13</center></td><td><center>17</center></td></tr><tr><th><center>Naszyjniki</center></th><td><center>6</center></td><td><center>10</center></td><td><center>14</center></td><td><center>14</center></td><td><center>18</center></td></tr><tr><th><center>Tarcze</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Kołczany</center></th><td><center>1</center></td><td><center>3</center></td><td><center>6</center></td><td><center>7</center></td><td><center>9</center></td></tr><tr><th><center>Błogosławieństwa</center></th><td><center>2</center></td><td><center>3</center></td><td><center>4</center></td><td><center>4</center></td><td><center>4</center></td></tr></tbody></table><br><br>
<br>
Przedmiotowi można nadać <b>dodatkowy bonus typu nagroda</b> w przypadku, gdy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• jest nagrodą za wykonanie zadania, jeżeli nagrodą jest dostęp do sklepu, wszystkie przedmioty otrzymują dodatkowy bonus.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• jest wynikiem stworzenia przedmiotu ze składników przy użyciu barteru lub rzemiosła.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• pochodzi z tytana.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• pochodzi z limitowanych aukcji i licytacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• jest błogosławieństwem dostępnym do pozyskania w trakcie wydarzenia czasowego.<br>
<br>
<br><br>
<a name="f1"></a><br>
<h3><span class="color-blue">Funkcje główne opisujące wartości atrybutów</span></h3><b>Moc poziomu przedmiotu</b><br>
Wzrost części atrybutów w przedmiotach ma charakter wielomianowy. Wraz ze wzrostem poziomu ich wartość zmienia się zgodnie z funkcją:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>level_power = 0.02 * lvl ^ 2 + 2.6 * lvl</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>level_power</code> - moc przedmiotu zależna od jego poziomu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom przedmiotu.<br>
<br>
<br><br>
<b>Moc klasy przedmiotu</b><br>
Istnieją bonusy, których moc zależna od jest klasy przedmiotu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Życie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Leczenie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Absorpcja i absorpcja magiczna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Pancerz.<br>
Na wartość tych bonusów wpływa moc klasy przedmiotu <code>class_power</code>, której zestawienie zostało zaprezentowane w poniższej tabeli.<br>
<br>
<br><table id="t322" style="width:500px">
<tbody><tr><th colspan="2" style="background-color:#546dd2"><center>Moc klasy przedmiotu (class_power)</center></th></tr><tr><th><center>Klasa przedmiotu</center></th><th><center>Moc klasy przedmiotu<br>(class_power)</center></th></tr><tr><th><center>Jednoręczne</center></th><td><center>1.00</center></td></tr><tr><th><center>Dwuręczne</center></th><td><center>1.00</center></td></tr><tr><th><center>Półtoraręczne</center></th><td><center>1.00</center></td></tr><tr><th><center>Dystansowe</center></th><td><center>1.00</center></td></tr><tr><th><center>Pomocnicze</center></th><td><center>1.00</center></td></tr><tr><th><center>Różdżki</center></th><td><center>1.00</center></td></tr><tr><th><center>Orby magiczne</center></th><td><center>1.00</center></td></tr><tr><th><center>Zbroje</center></th><td><center>1.00</center></td></tr><tr><th><center>Hełmy</center></th><td><center>0.33</center></td></tr><tr><th><center>Buty</center></th><td><center>0.30</center></td></tr><tr><th><center>Rękawice</center></th><td><center>0.25</center></td></tr><tr><th><center>Pierścienie</center></th><td><center>1.00</center></td></tr><tr><th><center>Naszyjniki</center></th><td><center>1.00</center></td></tr><tr><th><center>Tarcze</center></th><td><center>0.75</center></td></tr><tr><th><center>Kołczany</center></th><td><center>1.00</center></td></tr><tr></tr><tr><th><center>Błogosławieństwa</center></th><td><center>1.00</center></td></tr></tbody></table><br><br>
<br>
<b>Moc rzadkości przedmiotu</b><br>
Wzrost rzadkości przedmiotu wpływa na natywne atrybuty, takie jak:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• obrażenia<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• pancerz<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• absorpcja<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• absorpcja magiczna<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• odporność na magię<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• odporność na truciznę<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• niszczenie absorpcji.<br>
Moc rzadkości przedmiotu określa się wzorem:<br>
<code>rarity_power = 0.02 * lvl * ceil(10 * rarity_factor / 3) + sign(rarity_factor) * (7.8 * rarity_factor + 2.6)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rarity_power</code> - moc rzadkości przedmiotu potrzebna do ustalania wartości atrybutów przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>sign</code> - funkcja matematyczna znak.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>ceil</code> - funkcja matematyczna sufit.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rarity_factor</code> - współczynnik zależny od rzadkości przedmiotu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 0 - pospolite<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 - unikatowe<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 - heroiczne i ulepszone<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 3 - legendarne<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 4 - artefakty<br>
<br>
<br><br>
<h3><span class="color-blue">Obrażenia broni</span></h3>Wartość obrażeń w broni głównej, broni pomocniczej, orbie oraz kołczanach jest zależna od:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Klasy przedmiotu<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziomu przedmiotu<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Rzadkości przedmiotu<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Typu obrażeń<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wymagań profesji<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowych bonusów w obrażenia<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowego ulepszenia przedmiotu<br>
<br>
<b>Wartość obrażeń</b> danego typu obliczana jest zgodnie z następującą formułą:<br>
<code>damage<sub>item</sub> = 8 * weapon_factor<sub>item</sub> * (rariry_power<sub>item</sub> + level_power<sub>item</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>damage</code> - wartość obrażeń dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>weapon_factor<sub>item</sub></code> - współczynnik mocy obrażeń dla przedmiotu <code>item</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rariry_power<sub>item</sub></code> - moc rzadkości dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>level_power<sub>item</sub></code> - moc poziomu dla przedmiotu <code>item</code>. <br>
<br>
<br><table id="t323" style="width:500px">
<tbody><tr><th colspan="4" style="background-color:#546dd2"><center>Współczynnik ataku (weapon_factor) w broniach dla<br>wybranych typów ataku</center></th></tr><tr><th><center>Klasa przedmiotu</center></th><th><center>Typ obrażeń</center></th><th><center>Współczynniki obrażeń<br>(weapon_factor)</center></th><th><center>Rozrzuty obrażeń</center></th></tr><tr><td rowspan="6"><center>Jednoręczne</center></td><td><center>Zwyczajny</center></td><td><center>0.3378</center></td><td><center>10%</center></td></tr><tr><td><center>Zwyczajny<br>Głęboka rana</center></td><td><center>0.2646<br>0.0876</center></td><td><center>10%<br>100%</center></td></tr><tr><td><center>Zwyczajny<br>Trucizna</center></td><td><center>0.2646<br>0.0797</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Ogień</center></td><td><center>0.2869<br>0.1594</center></td><td><center>10%<br>20%</center></td></tr><tr><td><center>Zwyczajny<br>Zimno</center></td><td><center>0.2869<br>0.1435</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Błyskawice</center></td><td><center>0.2869<br>0.1594</center></td><td><center>10%<br>20%</center></td></tr><tr><td rowspan="6"><center>Dwuręczne</center></td><td><center>Zwyczajny</center></td><td><center>0.5578</center></td><td><center>10%</center></td></tr><tr><td><center>Zwyczajny<br>Głęboka rana</center></td><td><center>0.4606<br>0.1530</center></td><td><center>10%<br>100%</center></td></tr><tr><td><center>Zwyczajny<br>Trucizna</center></td><td><center>0.4606<br>0.0797</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Ogień</center></td><td><center>0.4876<br>0.2390</center></td><td><center>10%<br>20%</center></td></tr><tr><td><center>Zwyczajny<br>Zimno</center></td><td><center>0.4876<br>0.2152</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Błyskawice</center></td><td><center>0.4876<br>0.2391</center></td><td><center>10%<br>20%</center></td></tr><tr><td rowspan="6"><center>Półtoraręczne</center></td><td><center>Zwyczajny</center></td><td><center>0.3984</center></td><td><center>10%</center></td></tr><tr><td><center>Zwyczajny<br>Głęboka rana</center></td><td><center>0.3267<br>0.1084</center></td><td><center>10%<br>100%</center></td></tr><tr><td><center>Zwyczajny<br>Trucizna</center></td><td><center>0.3267<br>0.0797</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Ogień</center></td><td><center>0.4016<br>0.2072</center></td><td><center>10%<br>20%</center></td></tr><tr><td><center>Zwyczajny<br>Zimno</center></td><td><center>0.4016<br>0.1865</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Błyskawice</center></td><td><center>0.4016<br>0.2072</center></td><td><center>10%<br>20%</center></td></tr><tr><td rowspan="6"><center>Dystansowe</center></td><td><center>Zwyczajny</center></td><td><center>0.4303</center></td><td><center>10%</center></td></tr><tr><td><center>Zwyczajny<br>Głęboka rana</center></td><td><center>0.2901<br>0.1036</center></td><td><center>10%<br>100%</center></td></tr><tr><td><center>Zwyczajny<br>Trucizna</center></td><td><center>0.2901<br>0.1116</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Ogień</center></td><td><center>0.2231<br>0.2263</center></td><td><center>10%<br>20%</center></td></tr><tr><td><center>Zwyczajny<br>Zimno</center></td><td><center>0.2231<br>0.2040</center></td><td><center>10%<br>0%</center></td></tr><tr><td><center>Zwyczajny<br>Błyskawice</center></td><td><center>0.2231<br>0.2258</center></td><td><center>10%<br>20%</center></td></tr><tr><td rowspan="3"><center>Pomocnicze</center></td><td><center>Zwyczajny</center></td><td><center>0.2406</center></td><td><center>10%</center></td></tr><tr><td><center>Zwyczajny<br>Głęboka rana</center></td><td><center>0.1897<br>0.0367</center></td><td><center>10%<br>100%</center></td></tr><tr><td><center>Zwyczajny<br>Trucizna</center></td><td><center>0.1897<br>0.0335</center></td><td><center>10%<br>0%</center></td></tr><tr><td rowspan="3"><center>Różdżki</center></td><td><center>Ogień</center></td><td><center>0.3188</center></td><td><center>20%</center></td></tr><tr><td><center>Zimno</center></td><td><center>0.2709</center></td><td><center>0%</center></td></tr><tr><td><center>Błyskawice</center></td><td><center>0.3652</center></td><td><center>20%</center></td></tr><tr><td rowspan="3"><center>Orby</center></td><td><center>Ogień</center></td><td><center>0.1514</center></td><td><center>20%</center></td></tr><tr><td><center>Zimno</center></td><td><center>0.1355</center></td><td><center>0%</center></td></tr><tr><td><center>Błyskawice</center></td><td><center>0.1528</center></td><td><center>20%</center></td></tr><tr><td rowspan="5"><center>Kołczany</center></td><td><center>Zwyczajny</center></td><td><center>0.0303</center></td><td><center>10%</center></td></tr><tr><td><center>Trucizna</center></td><td><center>0.0271</center></td><td><center>0%</center></td></tr><tr><td><center>Ogień</center></td><td><center>0.0478</center></td><td><center>20%</center></td></tr><tr><td><center>Zimno</center></td><td><center>0.0430</center></td><td><center>0%</center></td></tr><tr><td><center>Błyskawice</center></td><td><center>0.0478</center></td><td><center>20%</center></td></tr></tbody></table><br><br>
Średnie obrażenia broni półtoraręcznej rosną o 22% przy zachowaniu rozrzutu 10%, jeżeli postać nie ma wyekwipowanej tarczy.<br>
<br>
Bronie i bronie pomocnicze, które oferują obrażenia od zimna oraz od trucizny, posiadają dodatkowy natywny bonus w <b>spowolnienie</b>. <br>
<b>Wartość spowolnienia</b> zależna jest od typu przedmiotu i jego poziomu zgodnie ze wzorem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>slow<sub>item</sub> = slow_factor<sub>item</sub> * lvl<sub>item</sub></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>slow<sub>item</sub></code> - spowolnienie dla broni <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>slow_factor<sub>item</sub></code> - współczynnik spowolnienia dla broni <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>item</sub></code> - poziom przedmiotu <code>item</code>.<br>
Współczynnik spowolnienia <code>slow_factor</code> został zestawiony w poniższej tabeli.<br>
<br><table id="t3241" style="width:500px">
<tbody><tr><th colspan="3" style="background-color:#546dd2"><center>Spowolnienie w broniach od zimna i trucizny</center></th></tr><tr><th><center>Klasa przedmiotu</center></th><th><center>Typ obrażeń</center></th><th><center>Współczynnik spowolnienia<br>(<code>slow_factor</code>)</center></th></tr><tr><td rowspan="2"><center>Jednoręczne</center></td><td><center>Zimno</center></td><td><center>0.009566</center></td></tr><tr><td><center>Trucizna</center></td><td><center>0.008925</center></td></tr><tr><td rowspan="2"><center>Dwuręczne</center></td><td><center>Zimno</center></td><td><center>0.010000</center></td></tr><tr><td><center>Trucizna</center></td><td><center>0.008925</center></td></tr><tr><td rowspan="2"><center>Półtoraręczne</center></td><td><center>Zimno</center></td><td><center>0.010000</center></td></tr><tr><td><center>Trucizna</center></td><td><center>0.008925</center></td></tr><tr><td rowspan="2"><center>Dystansowe</center></td><td><center>Zimno</center></td><td><center>0.0073529</center></td></tr><tr><td><center>Trucizna</center></td><td><center>0.0044625</center></td></tr><tr><td rowspan="1"><center>Pomocnicze</center></td><td><center>Trucizna</center></td><td><center>0.006375</center></td></tr><tr><td rowspan="1"><center>Różdżki</center></td><td><center>Zimno</center></td><td><center>0.010000</center></td></tr><tr><td rowspan="1"><center>Orby magiczne</center></td><td><center>Zimno</center></td><td><center>0.0073529</center></td></tr><tr><td rowspan="2"><center>Kołczany</center></td><td><center>Zimno</center></td><td><center>0.0073529</center></td></tr><tr><td><center>Trucizna</center></td><td><center>0.0044625</center></td></tr></tbody></table><br><br>
<br>
Część klas broni posiada natywne niszczenie pancerza lub odporności. Zestawienie wartości zostało zamieszczone w tabeli poniżej.<br>
Oznaczenia:<br>
<code>val</code> - szukana wartość.<br>
<code>lvl</code> - poziom przedmiotu.<br>
<br><table id="t3242" style="width:500px">
<tbody><tr><th colspan="4" style="background-color:#546dd2"><center>Natywne niszczenie w broniach</center></th></tr><tr><th><center>Klasa przedmiotu</center></th><th><center>Łączenie</center></th><th><center>Wartość atrybutu<br>niszczenie pancerza</center></th><th><center>Wartość atrybutu<br>niszczenie odporności</center></th></tr><tr><td><center>Jednoręczne</center></td><td><center>Paladyn</center></td><td><center>-</center></td><td><center><code>val = 1</code></center></td></tr><tr><td><center>Półtoraręczne</center></td><td><center>Paladyn</center></td><td><center>-</center></td><td><center><code>val = 1</code></center></td></tr><tr><td><center>Dwuręczne</center></td><td><center>Paladyn</center></td><td><center>-</center></td><td><center><code>val = 1</code></center></td></tr><tr><td rowspan="2"><center>Kołczan</center></td><td><center>Tropiciel</center></td><td><center>-</center></td><td><center><code>val = 1</code></center></td></tr><tr><td><center>Pozostałe</center></td><td><center><code>val = 0.04 * <a href="#f1">level_power<sub>lvl</sub></a></code></center></td><td><center>-</center></td></tr></tbody></table><br><br>
<h3><span class="color-blue">Obrona w pancerzach</span></h3>Wartość pancerza w zbroi, hełmie, rękawicach, butach i tarczach jest zależna od:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Typu przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziomu przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jakości przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dostępnych profesji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowych bonusów w pancerz lub obronę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowego ulepszenia przedmiotu (poziomu pozornego przedmiotu).<br>
<br>
<b>Wartość pancerza</b> obliczana jest zgodnie z następującą formułą:<br>
<code>ac<sub>item</sub> = 8 * armor_factor<sub>item</sub> * class_power<sub>item</sub> * (rarity_power<sub>item</sub> + level_power<sub>item</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;armor_factor<sub>item</sub> - współczynnik mocy pancerza zależny od podziału profesji dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>class_power<sub>item</sub></code> - moc klasy dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rarity_power<sub>item</sub></code> - moc rzadkości dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>level_power<sub>item</sub></code> - moc poziomu dla przedmiotu <code>item</code>.<br>
<b>Wartość odporności</b> na magię obliczana jest automatycznie i jest ściśle zależna od łączenia i niezależna od typu przedmiotu. <br>
Typ odporności na magię mogą zostać ustawione manualnie (<code>fire, frost, light</code>) w ramach atrybutu <code>autores</code>. Domyślnie odporności przyznawane są automatycznie zgodnie z zasadą:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• lvl % 3 == 0: odporność na ogień<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• lvl % 3 == 1: odporność na zimno<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• lvl % 3 == 2: odporność na błyskawice<br>
Jeżeli przedmiot posiada jakąkolwiek odporność magiczną, za każdy poziom jakości otrzymuje dodatkowo:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+2% odporności magicznej, jeżeli obowiązuje magiczny rozkład profesji: <code>m, t, pm, mt, pmt</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+1% odporności magicznej w przeciwnym wypadku.<br>
<br>
Absorpcję posiadają elementy pancerza, w których obowiązuje magiczny rozkład profesji: <code>m, t, pm, mt, pmt</code>.<br>
<b>Wartość absorpcji</b> obliczana jest zgodnie z następującą formułą: <br>
<code>absorb<sub>item</sub> = 8 * absorb_factor<sub>item</sub> * class_power<sub>item</sub> * (rarity_power<sub>item</sub> + level_power<sub>item</sub>)</code><br>
Natomiast wartość absorpcji magicznej zgodnie z formułą:<br>
<code>absorb_mag<sub>item</sub> = 4 * absorb_factor<sub>item</sub> * class_power<sub>item</sub> * (rarity_power<sub>item</sub> + level_power<sub>item</sub>)</code><br>
gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>absorb_factor<sub>item</sub></code> - współczynnik mocy absorpcji zależny od podziału profesji w przedmiocie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>class_power<sub>item</sub></code> - moc klasy dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rarity_power<sub>item</sub></code> - moc rzadkości dla przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>level_power<sub>item</sub></code> - moc poziomu dla przedmiotu <code>item</code>.<br>
<br>
<br><br>
<br><table id="t3251" style="width:500px">
<tbody><tr><th colspan="5" style="background-color:#546dd2"><center>Współczynnik pancerza, absorpcji oraz<br>bonusy natywne w elementach pancerza</center></th></tr><tr><th><center>Łączenie</center></th><th><center>armor_factor</center></th><th><center>Wartość odporności</center></th><th><center>absorb_factor</center></th><th><center>Bonusy natywne w zbroi</center></th></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>0.11250</center></td><td><center>magia: 2%<br>trucizna: 8%</center></td><td><center>-</center></td><td><center>+lvl/3 uniku</center></td></tr><tr><td><center>Wojownik</center></td><td><center>0.13500</center></td><td><center>trucizna: 1%</center></td><td><center>-</center></td><td><center>+lvl/100 życia za 1 pkt siły</center></td></tr><tr><td><center>Paladyn</center></td><td><center>0.12500</center></td><td><center>magia: 6%</center></td><td><center>-</center></td><td><center>+lvl/100 życia za 1 pkt siły</center></td></tr><tr><td><center>Mag</center></td><td><center>0.06250</center></td><td><center>magia: 10%</center></td><td><center>0.3750</center></td><td><center>+lvl/3 many<br>(od poziomu 21)</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>0.08750</center></td><td><center>magia: 8%<br>trucizna: 12%</center></td><td><center>0.2500</center></td><td><center>+lvl/6 many<br>(od poziomu 21)<br>+lvl/400 szybkości ataku</center></td></tr><tr><td><center>Łowca</center></td><td><center>0.10000</center></td><td><center>magia: 4%<br>trucizna: 16%</center></td><td><center>-</center></td><td><center>+lvl/200 szybkości ataku</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Wojownik</center></td><td><center>0.12375</center></td><td><center>magia: 1%<br>trucizna: 5%</center></td><td><center>-</center></td><td><center>+lvl/200 życia za 1 pkt siły</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Paladyn</center></td><td><center>0.11875</center></td><td><center>magia: 4%<br>trucizna: 4%</center></td><td><center>-</center></td><td><center>+lvl/200 życia za 1 pkt siły</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Tropiciel</center></td><td><center>0.10000</center></td><td><center>magia: 5%<br>trucizna: 10%</center></td><td><center>-</center></td><td><center>+lvl/550 szybkości ataku<br>+lvl/6 uniku</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Łowca</center></td><td><center>0.10625</center></td><td><center>magia: 3%<br>trucizna: 12%</center></td><td><center>-</center></td><td><center>+lvl/400 szybkości ataku<br>+lvl/6 uniku</center></td></tr><tr><td><center>Wojownik &amp; Paladyn</center></td><td><center>0.13000</center></td><td><center>magia: 3%<br>trucizna: 1%</center></td><td><center>-</center></td><td><center>+lvl/100 życia za 1 pkt siły</center></td></tr><tr><td><center>Paladyn &amp; Mag</center></td><td><center>0.09375</center></td><td><center>magia: 8%</center></td><td><center>0.1875</center></td><td><center>-</center></td></tr><tr><td><center>Paladyn &amp; Tropiciel</center></td><td><center>0.11500</center></td><td><center>magia: 7%<br>trucizna: 6%</center></td><td><center>0.0750</center></td><td><center>-</center></td></tr><tr><td><center>Mag &amp; Tropiciel</center></td><td><center>0.07500</center></td><td><center>magia: 9%<br>trucizna: 6%</center></td><td><center>0.3125</center></td><td><center>+lvl/6 many<br>(od poziomu 21)</center></td></tr><tr><td><center>Tropiciel &amp; Łowca</center></td><td><center>0.09375</center></td><td><center>magia: 6%<br>trucizna: 14%</center></td><td><center>-</center></td><td><center>+lvl/300 szybkości ataku</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Wojownik &amp; Paladyn</center></td><td><center>0.12000</center></td><td><center>magia: 2%<br>trucizna: 3%</center></td><td><center>-</center></td><td><center>+lvl/167 życia za 1 pkt siły</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Wojownik &amp; Łowca</center></td><td><center>0.11625</center></td><td><center>magia: 2%<br>trucizna: 8%</center></td><td><center>-</center></td><td><center>-</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Tropiciel &amp; Łowca</center></td><td><center>0.10000</center></td><td><center>magia: 5%<br>trucizna: 12%</center></td><td><center>-</center></td><td><center>+lvl/400 szybkości ataku<br>+lvl/7 uniku</center></td></tr><tr><td><center>Paladyn &amp; Mag &amp; Tropiciel</center></td><td><center>0.09375</center></td><td><center>magia: 8%<br>trucizna: 4%</center></td><td><center>0.2100</center></td><td><center>+lvl/6 many<br>(od poziomu 21)</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Wojownik &amp; Paladyn &amp; Łowca</center></td><td><center>0.12000</center></td><td><center>magia: 3%<br>trucizna: 6%</center></td><td><center>-</center></td><td><center>-</center></td></tr><tr><td><center>Tancerz ostrzy &amp; Wojownik<br>&amp; Paladyn &amp; Mag<br>&amp; Tropiciel &amp; Łowca</center></td><td><center>0.11250</center></td><td><center>-</center></td><td><center>-</center></td><td><center>-</center></td></tr><tr><td><center>Reszta połączeń</center></td><td><center>0.12500</center></td><td><center>-</center></td><td><center>-</center></td><td><center>-</center></td></tr></tbody></table><br><br>
Tarcze zawsze posiadają natywnie rozdany blok. Zestawienie wartości tej statystyki zostało zaprezentowane w poniższej tabeli.<br>
Oznaczenia:<br>
<code>block</code> - szukana wartość atrybutu blok.<br>
<code>lvl</code> - poziom przedmiotu.<br>
<br>
<br><table id="t3252" style="width:500px">
<tbody><tr><th colspan="2" style="background-color:#546dd2"><center>Natywny blok w tarczach</center></th></tr><tr><th><center>Łączenie</center></th><th><center>Wartość atrybutu blok</center></th></tr><tr><td><center>Paladyn</center></td><td><center><code>block = 1.2 * lvl</code></center></td></tr><tr><td><center>Wojownik &amp; Paladyn</center></td><td><center><code>block = 1.1 * lvl</code></center></td></tr><tr><td><center>Pozostałe</center></td><td><center><code>block = 1.0 * lvl</code></center></td></tr></tbody></table><br><br>
<h3><span class="color-blue">Wartości bonusów nadanych</span></h3>Oznaczenia:<br>
<code>val</code> - szukana wartość.<br>
<code>amt</code> - liczba bonusów danego typu występująca w przedmiocie.<br>
<code>lvl</code> - poziom przedmiotu.<br>
<code>level_power</code> - moc poziomu przedmiotu.<br>
<code>class_power</code> - moc klasy przedmiotu (moce przedmiotów zostały zestawione w <a href="#t322">tabeli</a>).<br>
<code>weapon_factor</code> - współczynnik ataku (współczynniki ataku zostały zestawione w <a href="#t323">tabeli</a>).<br>
<br>
<br><table id="t326" style="width:750px">
<tbody><tr><th colspan="4" style="background-color:#546dd2"><center>Wartości atrybutów rozdawanych w przedmiotach</center></th></tr><tr><th colspan="4"><center>Atrybuty dostępne we wszystkich przedmiotach w ramach bonusu</center></th></tr><tr><th><center>Atrybut<br>(nazwa silnikowa)</center></th><th><center>Wartość atrybutu</center></th><th><center>Zakres liczby bonusów<br>danego typu w przedmiocie</center></th></tr><tr><td><center>Wszystkie cechy (<code>da</code>)</center></td><td><center><code>val = 0.25 * lvl * amt + 8</code></center></td><td><center>[0 ; 6]</center></td></tr><tr><td><center>Siła (<code>ds</code>)</center></td><td><center><code>val = 5 * lvl * amt / 9 + 4</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Zręczność (<code>dz</code>)</center></td><td><center><code>val = 5 * lvl * amt / 9 + 4</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Intelekt (<code>di</code>)</center></td><td><center><code>val = 5 * lvl * amt / 9 + 4</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Szybkość ataku (<code>sa</code>)</center></td><td><center><code>val = 0.01 * round(8 + amt * 0.25 * lvl)</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Życie (<code>hp</code>)</center></td><td><center><code>val = amt * 3.08 * round(8 + lvl + 0.2 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a></code>)</center></td><td><center>[-2 ; 6]</center></td></tr><tr><td><center>Leczenie (<code>heal</code>)</center></td><td><center><code>val = 8 + amt * (0.8 * lvl + 0.2 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a>)</code></center></td><td><center>[0 ; 3]</center></td></tr><tr><td><center>Pancerz (<code>ac</code>)</center></td><td><center><code>val = amt * 0.15 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a></code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Pancerz magiczny (<code>acm</code>)</center></td><td><center><code>val = 0</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Odporność na truciznę (<code>act</code>)</center></td><td><center><code>val = 5 * amt</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Blok (<code>blok</code>)</center></td><td><center><code>val = amt * lvl * 3 / 20</code></center></td><td><center>[-1 ; 5]</center></td></tr><tr><td><center>Unik (<code>evade</code>)</center></td><td><center><code>val =  amt * lvl / 10</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Niszczenie pancerza (<code>acdmg</code>)</center></td><td><center><code>val = 1 + amt * <a href="#f1">level_power</a> / 50 [bronie]<br>val = 1 + amt * 0.75 * <a href="#f1">level_power</a> / 50 [pozostałe]</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Niszczenie odporności (<code>acmdmg</code>)</center></td><td><center><code>val = amt</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Ranienie posiadacza (<code>adest</code>)</center></td><td><center><code>val = 4 + amt * (0.5 * lvl + 0.1 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a>)</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Absorpcja (<code>absorb</code>)</center></td><td><center><code>val = amt * 0.6 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a></code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Absorpcja magiczna (<code>abrorbm</code>)</center></td><td><center><code>val = amt * 0.6 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a></code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Mana (<code>manabon</code>)</center></td><td><center><code>val = amt * (5 + lvl / 4)</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Energia (<code>energybon</code>)</center></td><td><center><code>val = amt * (<code>10 + lvl / 15</code>)</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Obniżanie szybkości<br>przeciwnika (<code>slow</code>)</center></td><td><code><center>val = 0.01 * round(8 + amt * 2 * lvl / 7)</center></code></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Cios krytyczny (<code>crit</code>)</center></td><td><center><code>val = amt</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Siła krytyka fizycznego (<code>critval</code>)</center></td><td><center><code>val = amt * 6</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Siła krytyka magicznego (<code>critmval</code>)</center></td><td><center><code>val = amt * 6</code></center></td><td><center>[-2 ; 5]</center></td></tr><tr><td><center>Obniżanie szansy na cios<br>krytyczny przeciwnika (<code>lowcrit</code>)</center></td><td><center><code>val = amt * 2</code></center></td><td><center>[0 ; 3]</center></td></tr><tr><td><center>Losowe niszczenie energii (<code>enfatig</code>)</center></td><td><center><code>chance [%] = min(100, 40% * amt)<br>val = 2 + 0.04 * lvl</code></center></td><td><center>[0 ; 3]</center></td></tr><tr><td><center>Losowe niszczenie many (<code>manafatig</code>)</center></td><td><center><code>chance [%] = min(100, 40% * amt)<br>val = 6 + 0.08 * lvl</code></center></td><td><center>[0 ; 3]</center></td></tr><tr><td><center>Niszczenie energii (<code>endest</code>)</center></td><td><center><code>val = amt * (2 + 0.02 * lvl)</code></center></td><td><center>[0 ; 2]</center></td></tr><tr><td><center>Niszczenie many (<code>manadest</code>)</center></td><td><center><code>val = amt * (5 + 0.04 * lvl)</code></center></td><td><center>[0 ; 2]</center></td></tr><tr><td><center>Obniżanie uniku (<code>lowevade</code>)</center></td><td><center><code>val =  amt * lvl / 10</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><th colspan="4"><center>Bonusy przeklęte</center></th></tr><tr><td><center>Obniżanie niszczenia energii i many (<code>resmanaendest</code>)</center></td><td><center><code>val = amt * (2 + 0.0133 * lvl) [energia]<br>val = amt * 0.75 * (5 + 0.04 * lvl) [mana]</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Obniżanie siły ciosu krytycznego (<code>lowcritallval</code>)</center></td><td><center><code>val = amt * 0.75 * (5 + ceil(0.02 * lvl))</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Obniżanie leczenia na 2 tury (<code>lowheal2turns</code>)</center></td><td><center><code>val = 0.75 * (8 + amt * (0.8 * lvl + 0.2 * <a href="#f1">level_power</a> * <a href="#t322">class_power</a>))</code></center></td><td><center>[0 ; 5]</center></td></tr><tr><td><center>Obniżanie niszczenia pancerza (<code>resacdmg</code>)</center></td><td><center><code>val = 1 + amt * 0.015 * <a href="#f1">level_power</a></code></center></td><td><center>[0 ; 5]</center></td></tr><tr><th colspan="4"><center>Bonusy dedykowane elementom pancerza</center></th></tr><tr><td><center>Obrona (<code>armor</code>)</center></td><td><center>Wartość pancerza odpowiada jakości przedmiotu wyższej o 1</center></td><td><center>[1 ; 3]</center></td></tr><tr><td><center>Odporność na ogień (<code>resfire</code>)</center></td><td><center><code>val = amt * 3</code></center></td><td><center>[-3 ; 10]</center></td></tr><tr><td><center>Odporność na zimno (<code>resfrost</code>)</center></td><td><center><code>val = amt * 3</code></center></td><td><center>[-3 ; 10]</center></td></tr><tr><td><center>Odporność na błyskawice (<code>reslight</code>)</center></td><td><center><code>val = amt * 3</code></center></td><td><center>[-3 ; 10]</center></td></tr><tr><th colspan="4"><center>Bonusy dedykowane broniom głównym oraz pomocniczym</center></th></tr><tr><td><center>Atak (<code>-</code>)</center></td><td><center>Wartość obrażeń odpowiada jakości przedmiotu wyższej o 1</center></td><td><center>[1 ; 3]</center></td></tr><tr><td><center>Przebicie pancerza<br>[dystansowe] (<code>pierce</code>)</center></td><td><center>Wartość ustalana manualnie</center></td><td><center>[0 ; 2]</center></td></tr><tr><td><center>Blok przebicia<br>[tarcze] (<code>pierceb</code>)</center></td><td><center>Wartość ustalana manualnie</center></td><td><center>[0 ; 1]</center></td></tr><tr><td><center>Kontra [jednoręczne]<br>(<code>contra</code>)</center></td><td><center>Wartość ustalana manualnie</center></td><td><center>[0 ; 2]</center></td></tr><tr><td><center>Niszczenie absorpcji<br>[bronie dowolne]<br>(<code>absdest</code>)</center></td><td><center><code>val = 0.33 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [jednoręczne tancerza ostrzy]<br>val = 0.33 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [półtoraręczne]<br>val = 0.36 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [dwuręczne]<br>val = 0.24 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [pomocnicze]<br>val = 0.21 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [orby]<br>val = 0.12 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [strzały]<br>val = 0.3 * (<a href="#f1">rarity_power</a> + <a href="#f1">level_power</a>) [pozostałe]</code></center></td><td><center>[0 ; 1]</center></td></tr></tbody></table><br><br>
<h3><span class="color-blue">Wartości bonusów ustalanych manualnie</span></h3>Część bonusów może przyjmować różne wartości z przedziału od zera do stu. Przyjęto koncepcję standaryzacji wartości tych bonusów w zależności od pochodzenia przedmiotu. Poniżej zestawiono wartości bonusów w zależności od klasy pochodzenia przedmiotu.<br>
<br>
<br><table id="t327" style="width:500px">
<tbody><tr><th colspan="5" style="background-color:#546dd2"><center>Wartości bonusów ustalanych manualnie<br>w zależności od klasy pochodzenia przedmiotu</center></th></tr><tr><th><center>Bonus</center></th><th><center>Liczba bonusów</center></th><th><center>Klasa I</center></th><th><center>Klasa II</center></th><th><center>Klasa III</center></th></tr><tr><td rowspan="2"><center>Kontra</center></td><td><center>1</center></td><td><center>40%</center></td><td><center>50%</center></td><td><center>50%</center></td></tr><tr><td><center>2</center></td><td><center>60%</center></td><td><center>60%</center></td><td><center>60%</center></td></tr><tr><td rowspan="2"><center>Przebicie pancerza</center></td><td><center>1</center></td><td><center>15%</center></td><td><center>20%</center></td><td><center>20%</center></td></tr><tr><td><center>2</center></td><td><center>25%</center></td><td><center>25%</center></td><td><center>25%</center></td></tr><tr><td><center>Blok przebicia</center></td><td><center>1</center></td><td><center>40%</center></td><td><center>50%</center></td><td><center>60%</center></td></tr><tr><td><center>Głęboka rana</center></td><td><center>0</center></td><td><center>20%</center></td><td><center>23%</center></td><td><center>25%</center></td></tr></tbody></table><br><br>
<b>Klasa I przedmiotów:</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z potworów zwyczajnych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z elit.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z elit II.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• oferty sklepów.<br>
<b>Klasa II przedmiotów:</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z elit III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z herosów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z kolosów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z elit eventowych, elit III eventowych, kolosów eventowych oraz tytanów eventowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty będące nagrodą za wykonanie zadania lub pośrednio związane z jego wykonaniem.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty wytworzone przy użyciu barteru lub rzemiosła.<br>
<b>Klasa III przedmiotów:</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z tytanów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z herosów eventowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• przedmioty pochodzące z limitowanych aukcji i licytacji.<br>
<br>
<br><br>
<h3><span class="color-blue">Bonusy legendarne</span></h3>Przedmioty legendarne posiadają dodatkowy ekskluzywny dla nich bonus zwany bonusem legendarnym, który oferuje specjalne efekty możliwe do wystąpienia podczas walki. Dostępne są następujące bonusy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Cios bardzo krytyczny<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dotyk anioła<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Klątwa<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Oślepienie<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ostatni ratunek<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Krytyczna osłona<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Fasada opieki<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Płomienne oczyszczenie<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Krwawa udręka<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przeszywająca skuteczność<br>
<br>
Z każdym bonusem powiązana jest początkowa wartość, która może określać prawdopodobieństwo wyzwolenia danego efektu lub określoną wartość procentową siły efektu. Założenie kolejnego przedmiotu z tym samym bonusem legendarnym sprawia, że wartość powiązana z efektem wzrasta jedynie o połowę poprzedniego efektu. W konsekwencji wartość efektu powiązanego z bonusem legendarnym, w zależności od liczby posiadanych przedmiotów z tym bonusem, można obliczyć ze wzoru:<br>
<code>value<sub>n,effect</sub> = value<sub>0,effect</sub> + <sup>N</sup>Σ<sub>n=1</sub>round(value<sub>n - 1,effect</sub> * 0.5)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>value<sub>n,effect</sub></code> - wartość efektu dla <code>n</code> wystąpień bonusu w ekwipunku.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>value<sub>0,effect</sub></code> - wartość początkowa efektu bonusu legendarnego.<br>
<br>
W przypadku posiadania wielu przedmiotów z tym samym bonusem legendarnym, które ulegają słabnięciu na skutek przewagi poziomowej postaci nad przedmiotem, zawsze najmniej osłabiona wartość zmiennej statystyki jest pierwszym wystąpieniem bonusu legendarnego. Kolejna najmniej osłabiona wartość jest kolejnym wystąpieniem - najbardziej osłabiona wartość jest ostatnim wystąpieniem bonusu i ulega największej redukcji.<br>
<br>
<b>Cios bardzo krytyczny (<code>verycrit</code>)</b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, zależne od posiadanej przez postać szansy na cios krytyczny, podczas którego zwiększa się siła ciosu krytycznego fizycznego oraz magicznego postaci o 75% posiadanej wartości oraz wyzwala się zdarzenie ciosu krytycznego na jedną turę.<br>
<i>Przykład</i>: szansa na zajście zdarzenia wynosi 17%, gracz posiada 10% szansy na cios krytyczny oraz 1.4 siły ciosu krytycznego fizycznego. Istnieje więc szansa 17% * 10% = 1.7% na zajście zdarzenia, podczas którego wyzwoli się cios krytyczny, a siła ciosu krytycznego fizycznego wyniesie 2.45 (obrażenia broni zostaną więc przemnożone o tę wartość).<br>
• Zdarzenie może zajść wyłącznie podczas wykonania ataku przez posiadacza bonusu.<br>
• Parametr zmienny: szansa na zajście zdarzenia.<br>
• Wartość początkowa: 17%.<br>
• Efekty umiejętności, zwiększające szansę na cios krytyczny postaci, wpływają na zajście zdarzenia ciosu bardzo krytycznego.<br>
• Efekty umiejętności przeciwnika, zmniejszające szansę na cios krytyczny postaci, nie wpływają na zajście zdarzenia ciosu bardzo krytycznego.<br>
• Obniżanie szansy na cios krytyczny przeciwnika, którego źródłem jest bonus <code>lowcrit</code> z ekwipunku, nie wpływa na zajście zdarzenia ciosu bardzo krytycznego.<br>
• Bonus ma charakter ofensywny i prowadzi do skrócenia walki.<br>
• Bonus jedynie wzmacnia siłę obrażeń wykonanych, które następnie są zmniejszane przez efekty zdarzeń (również niwelowanie obrażeń przez efekt <b>chybienia</b> oraz redukcji obrażeń).<br>
• Bronie pomocnicze z faktu posiadania osobnego zdarzenia dla ciosu krytycznego (pomocniczego) posiadają również osobne zdarzenie ciosu bardzo krytycznego pomocniczego, który zwiększa siłę ciosu krytycznego pomocniczego o 75%.<br>
<br>
<b>Dotyk anioła (<code>holytouch</code>)</b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, podczas którego postać aplikuje na siebie efekt rozłożony na 3 tury, którego każde wyzwolenie leczy postaci 6% puli punktów zdrowia.<br>
• Zdarzenie może zajść wyłącznie podczas wykonania ataku przez posiadacza bonusu. <br>
• Leczenie nie może przekroczyć poziomu zdrowia, z którym postać rozpoczynała walkę.<br>
• Parametr zmienny: szansa na zajście zdarzenia.<br>
• Wartość początkowa: 7%.<br>
• Zdarzenie może zajść w przypadku wykonania ataku bez konieczności trafienia przeciwnika.<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
• Efekty redukcji leczenia nie wpływają na przywracane zdrowie z dotyku anioła.<br>
• Efekty leczenia nie kumulują się. zajście kolejnego zdarzenia dotyku anioła odnawia czas trwania efektu.<br>
<br>
<b>Klątwa (<code>curse</code>)</b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, podczas którego postać aplikuje na przeciwnika efekt zaniechania wykonania jego następnej akcji. Przeciwnik objęty tym efektem w momencie wykonania tury, jest informowany o zaniechaniu jej wykonania.<br>
• Zdarzenie może zajść wyłącznie podczas wykonania ataku przez posiadacza bonusu oraz trafienia przeciwnika (brak zdarzenia <b>chybienia</b>).<br>
• Tura przeciwnika objętego Klątwą jest wykonywana automatycznie i nie może zostać skrócona żadnym efektem.<br>
• Parametr zmienny: szansa na zajście zdarzenia.<br>
• Wartość początkowa: 9%.<br>
• Bonus ma zarówno charakter defensywny oraz ofensywny w zależności od profesji uczestniczących w walce.<br>
• Efekt bonusu nie kumuluje się. Mimo aplikacji wielu bonusów w tego samego przeciwnika, wyzwalany jest tylko jeden podczas najbliższej tury. <br>
• Efekt bonusu jest tym samym efektem co u Oślepienia (<code>glare</code>) oraz Wytrącenia z równowagi (<code>distract</code>). Tylko jeden z tych efektów może być nałożony na postać w tej samej chwili.<br>
• Jeżeli na postać są nałożone jednocześnie efekty Ogłuszenia (<code>stun</code>) oraz przerwania tury (<code>curse, distract, glare</code>), to najpierw traci ona turę na skutek ogłuszenia, a następnie kolejną turę na skutek przerwania tury.<br>
<br>
<b>Oślepienie (<code>glare</code>)</b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, podczas którego postać aplikuje na przeciwnika efekt zaniechania wykonania jego następnej akcji. Przeciwnik objęty tym efektem w momencie wykonania tury, jest informowany o zaniechaniu jej wykonania.<br>
• Zdarzenie może zajść wyłącznie podczas przyjęcia trafionego ataku w posiadacza bonusu (brak zdarzenia <b>chybienia</b>).<br>
• Tura przeciwnika objętego Klątwą jest wykonywana automatycznie i nie może zostać skrócona żadnym efektem.<br>
• Parametr zmienny: szansa na zajście zdarzenia.<br>
• Wartość początkowa: 9%.<br>
• Bonus ma zarówno charakter defensywny oraz ofensywny w zależności od profesji uczestniczących w walce.<br>
• Efekt bonusu nie kumuluje się. Mimo aplikacji wielu bonusów w tego samego przeciwnika, wyzwalany jest tylko jeden podczas najbliższej tury.<br>
• Efekt bonusu jest tym samym efektem co u Klątwy (<code>curse, mcurse</code>) oraz Wytrącenia z równowagi (<code>distract</code>). Tylko jeden z tych efektów może być nałożony na postać w tej samej chwili.<br>
<br>
<b>Ostatni ratunek (<code>lastheal</code>)</b><br>
• Działanie: w przypadku przyjęcia przez postać obrażeń zmniejszających jej poziom punktów życia poniżej 18% puli zdrowia, zostaje ona jednorazowo uleczona o losową wartość z pewnego zakresu.<br>
• Efekt może zajść wyłącznie raz podczas walki i uaktywnia się kiedy poziom zdrowia jest niższy od 18%, ale postać jednocześnie nie przyjęła śmiertelnych obrażeń. Może zajść zarówno podczas zadawania obrażeń przez posiadacza bonusu (w wyniku odbicia części obrażeń w atakującego), przyjmowania obrażeń przez posiadacza bonusu, jak i w momencie wyzwolenia obrażeń rozłożonych w czasie raniących posiadacza bonusu.<br>
• Efekt nie może przywrócić więcej życia niż poziom zdrowia, z którym postać rozpoczęła walkę.<br>
• Parametr zmienny: poziom przywracanego zdrowia oraz rozrzut przywracania zdrowia.<br>
• Zakres początkowy: 36% - 44%<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
• Efekty redukcji leczenia nie wpływają na przywracane zdrowie z ostatniego ratunku.<br>
<br>
<b>Krytyczna osłona (<code>critred</code>)</b><br>
• Działanie: w przypadku przyjęcia przez postać ciosu krytycznego (lub ciosu krytycznego pomocniczego), wszystkie obrażenia od broni przeciwnika są zredukowane o pewną ich część.<br>
• Redukcja obrażeń na skutek krytycznej osłony następuje w tym samym momencie co <a href="#kkrd">redukcja obrażeń na skutek odporności</a>.<br>
• Efekt uaktywnia się wyłącznie podczas przyjęcia ataku w posiadacza bonusu.<br>
• Parametr zmienny: część redukowanych obrażeń od broni przeciwnika.<br>
• Wartość początkowa: 25%.<br>
• W przypadku otrzymania obrażeń od broni pomocniczej oraz zajściu zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, zarówno obrażenia od broni głównej jak i pomocniczej są redukowane.<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
<br>
<a name="fasada"></a><br>
<b>Fasada opieki (<code>facade</code>)</b><br>
• Działanie: w przypadku przyjęcia przez postać niezerowych obrażeń podczas ciosu, są one redukowane o pewną ich część. Redukowane są obrażenia fizyczne, pomocnicze, dystansowe oraz obrażenia magiczne - od magii ognia, błyskawic oraz zimna.<br>
• Redukcja obrażeń na skutek Fasady opieki następuje w tym samym momencie co <a href="#kkrd">redukcja obrażeń na skutek odporności</a>.<br>
• Efekt uaktywnia się wyłącznie podczas przyjęcia niezerowych obrażeń podczas ataku w posiadacza bonusu.<br>
• Parametr zmienny: część redukowanych obrażeń ciosu.<br>
• Wartość początkowa: 13% (kolejne wartości kumulacji: 20%, 23%, 25%, 26%, 26%).<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
• Bonus jest widoczny w logu walki wyłącznie w chwili przyjęcia obrażeń po raz pierwszy.<br>
• Bonus nie redukuje obrażeń rozłożonych w czasie.<br>
<br>
<b>Płomienne oczyszczenie (<code>cleanse</code>)</b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, podczas którego z postaci są zdejmowane wszystkie trwające w bieżącej turze efekty obrażeń rozłożonych w czasie, efekty spowolnienia i efekty ogłuszenia.<br>
• Zdarzenie może zajść wyłącznie podczas przyjęcia trafionego ataku w posiadacza bonusu oraz tylko w przypadku, gdy nałożony jest na niego jakikolwiek efekt ogłuszenia, spowolnienia lub obrażeń rozłożonych w czasie.<br>
• Parametr zmienny: prawdopodobieństwo zajścia zdarzenia.<br>
• Wartość początkowa: 12% (kolejne wartości kumulacji: 18%, 21%, 23%, 24%, 24%).<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
<br>
<a name="anguish"></a><br>
<b>Krwawa udręka (<code>anguish</code>)</b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, podczas którego na cel ataku zostają zaaplikowane obrażenia od krwawienia rozłożone w czasie na pięć tur.<br>
• Zdarzenie możesz zajść wyłącznie, jeżeli podczas ciosu nie zaszedł unik, neutralizacja strzały (<code>arrowblock</code>) oraz parowanie (<code>parry</code>).<br>
• Parametr zmienny: prawdopodobienstwo zajścia zdarzenia.<br>
• Wartość początkowa: 8% (kolejne wartości kumulacji: 12%, 14%, 15%, 16%, 16%).<br>
• Bonus ma charakter ofensywny i prowadzi do skrócenia walki.<br>
• Obrażenia od krwawienia są redukowane jedynie przez efekty takich umiejętności jak <i>Strach</i> (<code>dmg_from_player_per</code>) oraz <i>Toksyczne opary</i> (<code>poison_lowdmg_per-enemies</code>).<br>
• Efekt krwawienia może zostać usunięty, jeżeli podczas ataku zajdzie Płomienne oczyszczenie.<br>
• Obrażenia się nie kumulują, ulegają jedynie przedłużeniu czasowi trwania. Na postaci może być aktywna tylko jedna Krwawa udręka.<br>
• Ulepszenie przedmiotu powoduje wzrost obrażeń od krwawienia tylko wówczas, gdy poziom pozorny nie przekroczy 300.<br>
• Wartość obrażeń jest zależna od poziomu pozornego przedmiotu oraz od atrybutów podstawowych (siły, zręczności, intelektu) zgodnie z poniższym wzorem:<br>
<code>anguish_damage = (0.0025 * lvl + 0.3) * (str + int + 0.8 * agi)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom pozorny przedmiotu. Wartość nie może przekroczyć liczby 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>str</code> - liczba skumulowanych punktów w siłę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>int</code> - liczba skumulowanych punktów w intelekt.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>agi</code> - liczba skumulowanych punktów w zręczność.<br>
<i>Przykład</i>: postać na poziomie 123 posiadająca 200 punktów siły, 400 punktów intelektu oraz 555 punktów zręczności zadaje obrażenia równe wynikowi poniższych obliczeń:<br>
<code>damage = (0.0025 * 123 + 0.3) * (200 + 400 + 0.8 * 555) = (0.6075) * (200 + 400 + 444) = 634.23 = 634</code><br>
<br>
<a name="puncture"></a><br>
<b>Przeszywająca skuteczność (<code>puncture</code>)</b><br>
• Działanie: podczas walki ataki posiadacza ignorują statystyki defensywne celu - pancerz, odporności magiczne, absorpcję oraz absorpcję magiczną, punkty uniku i punkty bloku.<br>
• Parametr zmienny: część ignorowanej defensywy.<br>
• Wartość początkowa: 12% (kolejne wartości kumulacji: 18%, 21%, 23%, 24%, 24%).<br>
• Bonus ma charakter ofensywny i prowadzi do skrócenia walki.<br>
• Bonus jest widoczny w logu walki wyłącznie w chwili wykonania ataku po raz pierwszy.<br>
• Bonus sprawia, że podczas ataku w cel, ignorowana jest część jego statystyk defensywnych. Osłabienie to odbywa się w zakresie pojedynczego ataku i nie powoduje wzrostu siły ataków sojuszników przeciw temu samemu przeciwnikowi. Nie powoduje też obniżenia odporności tuż po zadaniu ciosu (na przykład odporności na truciznę lub głęboką ranę).<br>
• Sposób zmniejszania defensywy zależy od statystyki - każda statystyka defensywna jest redukowana inną metodą.<br>
• Podczas obliczania redukcji obrażeń wynikającej z pancerza, bieżąca wartość pancerza jest pomniejszona. Zmniejszenie następuje po zniszczeniu pancerza przez statystykę <code>acdmg</code> oraz uwzględnia efekty umiejętności zwiększające pancerz (takie jak <code>acshield_per</code>, <code>sunshield_per</code>, <code>ac_per</code>, <code>aura-ac_per</code>). Pancerz ulega zmniejszeniu nawet wtedy, gdy zniszczono połowę jego początkowej wartości.<br>
<i>Przykład</i>: wojownik posiada bonus Przeszywająca skuteczność o wartości 12% i atakuje paladyna z mocą 7500 obrażeń fizycznych przeciwnika posiadającego 2500 pancerza. Wojownik atakując niszczył 700 pancerza. Paladyn miał aktywną na sobie umiejętność Aurę ochrony zwiększającą jego pancerz o 10%. Obrażenia zadane wyniosą:<br>
<code>damage = 7500 - [(1 - 0.12) * (1.1 * 2500 - 700) * (1.13 - 0.31 * ((1 - 0.12) * 1.1 * 2500 - 700) / 7500)] = 5589.73 = 5590</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Stałe parametry <code>1.13</code> oraz <code>0.31</code> wynikają ze wzoru na <a href="#damages">redukcję obrażeń fizycznych przez pancerz</a>.<br>
• Podczas obliczania redukcji obrażeń wynikającej z odporności, bieżąca wartość odporności wyrażona w punktach procentowych jest pomniejszona. Odporność po obniżeniu może przyjąć ujemne wartości, co powoduje zwiększenie obrażeń zamiast jego obniżenia.<br>
<i>Przykład</i>: mag posiadający Przeszywającą skuteczność o wartości 12% atakuje z mocą 4500 obrażeń od ognia łowcę posiadającego 6% odporności na ogień oraz 500 pancerza. Obrażenia wyniosą:<br>
<code>damage = [4500 - (1 - 0.12) * 0.5 * 500 * (1.13 - 0.31 * (1 - 0.12) * 0.5 * 500 / 4500)] * (1 - 0.06 + 0.12) = 4510</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Stały mnożnik <code>0.5</code> wynika z tego, że podczas obliczania obrażeń magicznych brana pod uwagę jest jedynie połowa wartości pancerza.<br>
• Podczas obliczania redukcji obrażeń przez absorpcję oraz absorpcję magiczną, brana pod uwagę jest obniżona jej bieżąca wartość. Oznacza to, że działanie bonusu jest zauważalne wtedy, kiedy wartość ciosu jest większa niż pomniejszona pula absorpcji (ograniczona przez skuteczność absorpcji przeciw typowi obrażeń) i powoduje on jedynie opóźnienie momentu zniszczenia pozostałych punktów.<br>
<i>Przykład</i>: mag posiadający Przeszywającą skuteczność o wartości 12% atakuje tropiciela z mocą 5000 obrażeń, które zostały pomniejszone przez pancerz do 4500 obrażeń. Absorpcja magiczna tropiciela wynosi 3000 punktów. Pomijamy odporności magiczne. Obrażenia maga wyniosą:<br>
<code>damage = 4500 - 3000 * 0.9 * (1 - 0.12) = 2124</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pula absorpcji magicznej tropciela zostanie pomniejszona o 4500 - 2124 = 2376 punktów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Stały mnożnik <code>0.9</code> to skuteczność absorpcji przeciw obrażeniom magicznym.<br>
• Podczas losowania zdarzenia uniku, liczba punktów jest najpierw pomniejszana o wartość Przeszywającej skuteczności, a następnie obniżana o liczbę punktów obniżania uniku z ekwipunku (<code>lowevade</code>) oraz efektów umiejętności (<code>active_decevade_per</code>, <code>decevade_per</code>).<br>
<i>Przykład</i>: wojownik z poziomem 133 posiadający Przeszywającą skuteczność o wartości 12%, 111 obniżania uniku z ekwipunku oraz 10% obniżania uniku z umiejętności <i>Celny cios</i> atakuje łowcę z poziomem 144 posiadającego 220 punktów uniku. Szansa na unik łowcy wyniesie:<br>
<code>evade[%] = (220 * (1 - 0.12) - 111) * 20 / 133 [%] - 10 [%] = 2.42 [%]</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Należy pamiętać, że podczas obliczania szansy na unik, brany pod uwagę jest poziom gracza atakującego.<br>
• Podczas losowania zdarzenia bloku, liczba punktów jest najpierw pomniejszana o wartość Przeszywającej skuteczności, a następnie obniżana przez efekty umiejętności (<code>active_decblock_per</code>, <code>active_decblock_per-enemies</code>, <code>decblock_per</code>).<br>
<br>
<b>Fizyczna osłona (<code>dmgred</code>) - <span class="color-red">Bonus wycofany</span></b><br>
• Działanie: w przypadku przyjęcia przez postać obrażeń fizycznych (również dystansowych oraz obrażeń od broni pomocniczej), są one redukowane o pewną ich część.<br>
• Redukcja obrażeń na skutek fizycznej osłony następuje w tym samym momencie co <a href="#kkrd">redukcja obrażeń na skutek odporności</a>.<br>
• Efekt uaktywnia się wyłącznie podczas przyjęcia trafionego ataku z obrażeniami fizycznymi, dystansowymi lub pomocniczymi w posiadacza bonusu.<br>
• Parametr zmienny: część redukowanych obrażeń fizycznych.<br>
• Wartość początkowa: 16%.<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
• Bonus jest widoczny w logu walki wyłącznie w chwili przyjęcia obrażeń po raz pierwszy.<br>
<br>
<b>Ochrona żywiołów (<code>resgain</code>) - <span class="color-red">Bonus wycofany</span></b><br>
• Działanie: podczas walki istnieje prawdopodobieństwo na zajście zdarzenia, podczas którego odporności magiczne postaci (odporność na ogień, zimno, błyskawice) zwiększają się do 90% na jedną turę.<br>
• Zdarzenie może zajść wyłącznie podczas przyjęcia trafionego ataku z obrażeniami magicznymi (od ognia, zimna lub błyskawic) w posiadacza bonusu.<br>
• Odporności na żywioły są zwiększane dopiero po ich obniżeniu przez atrybut niszczenia odporności, zatem zawsze wynoszą 90%.<br>
• Parametr zmienny: prawdopodobieństwo zajścia zdarzenia.<br>
• Wartość początkowa: 16%.<br>
• Bonus ma charakter defensywny i prowadzi do przedłużenia walki.<br>
<br>
<br><br>
<h3><span class="color-blue">Słabnięcie bonusów legendarnych</span></h3>Wraz ze wzrostem poziomu postaci nad poziomem przedmiotu legendarnego, dochodzi do rozpoczęcia słabnięcia parametrów zmiennych bonusów legendarnych. Od określonego poziomu ich wartość zaczyna maleć do zera. Spadek wartości jest liniowy na przestrzeni 50 poziomów - po 25 poziomach słabnięcia (czyli połowy zakresu słabnięcia), wartość bonusu spada o połowę. W przypadku bonusów, których wartość jest przedstawiana jako liczba całkowita, następuje zawsze zaokrąglenie matematyczne siły bonusu. Słabnięcie obowiązuje również w przypadku błogosławieństw.<br>
W przypadku postaci z poziomem przekraczającym 300, wartość parametrów zmiennych jest obliczana na podstawie <a href="op_lvl">poziomu operacyjnego</a>.<br>
W przypadku, gdy postać znajduje się na mapie, na której wyłączony jest bonus do przewagi poziomowej oraz jej poziom przekracza 300, słabnięcie bonusów legendarnych obliczane jest tak, jakby miała ona poziom 300. Zasada ta dotyczy również obliczania słabnięcia bonusów legendarnych w ekwipunkach postaci walczących na Otchłani.<br>
<b><a href="https://youtube.com/shorts/WGMKKV6ZCdw">Krótki film</a></b> omawiający mechanikę słabnięcia bonusów legendarnych.<br>
Poniżej zestawiono sposób obliczania poziomu, od którego bonus legendarny zaczyna słabnąć oraz poziom, od którego następuje jego całkowite wygaszenie.<br>
<br>
<br><table id="t328" style="width:500px">
<tbody><tr><th colspan="4" style="background-color:#546dd2"><center>Słabnięcie bonusów legendarnych w przedmiotach jakości legendarnej</center></th></tr><tr><th colspan="2"><center>Poziom pierwszego osłabienia przedmiotu</center></th><th colspan="2"><center>Poziom wygaszenia działania bonusu</center></th></tr><tr><th><center>&lt;120 lvl</center></th><th><center>&gt;=120lvl</center></th><th><center>&lt;120lvl</center></th><th><center>&gt;=120lvl</center></th></tr><tr><td><center>30 + lvl<sub>item</sub></center></td><td><center>1.25 * lvl<sub>item</sub></center></td><td><center>80 + lvl<sub>item</sub></center></td><td><center>50 + 1.25 * lvl<sub>item</sub></center></td></tr></tbody></table><br><br>
<h3><span class="color-blue">Błogosławieństwa</span></h3>Błogosławieństwa są przedmiotem, który po nałożeniu na postać działa jedynie przez określony czas, po którym zanika. Błogosławieństwo można zdjąć z postaci w dowolnym momencie, jednak spowoduje to jego usunięcie. Mogą mieć one określony poziom lub dopasowywać się do poziomu gracza (jednak nie przekraczają nigdy poziomu 300).<br>
<br>
<br><br>
<a name="ekwipowalne"></a><br>
<h3><span class="color-blue">Przedmioty ekwipowalne</span></h3>Zmiana stanu na skutek operacji ulepszania, obniżania wymagań lub przekuwania może być przeprowadzona jedynie na nieulotnych przedmiotach ekwipowalnych. Są to przedmioty posiadające klasę: jednoręczne, dwuręczne, półtoraręczne, dystansowe, pomocnicze, różdżki, orby magiczne, zbroje, hełmy, buty, rękawice, pierścienie, naszyjniki, tarcze, strzały.<br>
<br>
<br>
<br><br>
<h3><span class="color-blue">Przedmioty przeklęte</span></h3>Przedmioty przeklęte to specjalne <a href="#ekwipowalne">przedmioty ekwipowalne</a>, które posiadają swoją ilość i zmniejszają ją o 1 po każdej stoczonej walce. W przypadku gdzy ilość spadnie do zera, przedmiot nie znika, ale nie można go wyekwipować.<br>
Przedmioty przeklęte posiadają jeden bonus więcej, którym jest jeden z ekskluzywnych dla nich atrybutów:<br>
• Obniżanie niszczenia energii i many - zmniejsza niszczenie energii i many z ekwipunku przeciwnika (obniżenie występuje przed redukcją z efektu umiejętności <code>reddest_per</code>).<br>
• Obniżanie leczenia - zmniejsza leczenie z ekwipunku przeciwnika na 2 tury od momentu wykonania udanego ataku (obniżenie występuje przed redukcją z efektów <code>heal_per-enemies, critpoison_per</code>).<br>
• Obniżanie niszczenia pancerza - zmniejsza niszczenie pancerza z ekwipunku przeciwnika (obniżenie występuje przed redukcją z efektu <code>redacdmg_per</code>).<br>
• Obniżanie siły ciosu krytycznego - zmniejsza moc ciosu krytycznego fizycznego (również pomocniczego) i magicznego przeciwnika.<br>
<br>
<br><br>
<h3><span class="color-blue">Obniżanie wymagań przedmiotu</span></h3>Istnieją specjalne przedmioty ulepszające (ulepszenia) z atrybutem <code>lowreq</code>, które po użyciu na nieulotnym <a href="#ekwipowalne">ekwipowalnym przedmiocie</a>, zmieniają jego wymagania poziomowe. Obniżenie wymagań nie wpływa na wartości atrybutów przedmiotu i względem niego nie są obliczanie żadne dodatkowe przyrosty poziomowe.<br>
Liczba poziomów, o jaką maleje wymóg poziomowy zależy od rzadkości przedmiotu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 3 poziomy - dla przedmiotów pospolitych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 2 poziomy - dla przedmiotów unikatowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 1 poziom - dla przedmiotów heroicznych i ulepszonych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Brak możliwości obniżenia - dla przedmiotów legendarnych i artefaktów.<br>
<br>
Obniżenie wymagań może zostać usunięte, jeżeli na danym przedmiocie zostanie użyty specjalny Zwój oczyszczenia (przedmiot z trybutem <code>undoupg</code>).<br>
Nie można obniżyć wymagań poziomowych przedmiotów, które zostały przekute.<br>
<br>
<br><br>
<h3><span class="color-blue">Wytwarzanie przedmiotów</span></h3>Istnieją specjalne bartery, w których można wymieniać przedmioty (składniki) na inne przedmioty (produkty). W przypadku większości wytwarzanych przedmiotów, wymagane do tego jest złoto oraz określone składniki. Część ofert może mieć limit dzienny, tygodniowy lub miesięczny ich wytworzeń przypadających na postać.<br>
<br>
Bartery posiadają następujące pola:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Listę produktów podzieloną na klasy przedmiotów wraz z polem filtrowania po nazwie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Podgląd produktu wraz z ilością przedmiotów tworzonych w torbie gracza po zakończeniu operacji sukcesem.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Suwak umożliwiający określenie jak dużo produktów zostanie wytworzonych w ramach operacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Listę składników niezbędnych do wytworzenia produktu uwzględniając walutę (złoto, Smocze Łuski, Punkty Honoru lub przedmiot) wraz z ilością każdego przedmiotu. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Limit czasowy wytworzeń przedmiotów (limit na dzień, limit na tydzień lub limit na miesiąc).<br>
<b><a href="https://youtube.com/shorts/RdyctT4msAY">Krótki film</a></b> wizualizujący proces tworzenia przedmiotów w barterze.<br>
<br>
Znaczna część produktów do wytworzenia wymaga opłaty w złocie. Koszt wytworzenia przedmiotu w złocie wynosi:<br>
<code>create_cost<sub>item</sub> = floor(rarity_cost_factor<sub>item</sub> * (2.4 * lvl<sub>item</sub>^2 + 10 * lvl<sub>item</sub>))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>create_cost<sub>item</sub></code> - koszt wytworzenia przedmiotu w barterze podawany w złocie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>item</sub></code> - poziom przedmiotu (produktu).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>rarity_cost_factor</code> - współczynnik kosztu zależny od jakości przedmiotu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5 dla przedmiotów pospolitych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5 dla przedmiotów unikatowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;10 dla przedmiotów heroicznych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;50 dla przedmiotów legendarnych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja zaokrąglenia w dół do dwóch cyfr znaczących.<br>
<br>
Wytwarzane przedmioty posiadają dodatkowy bonus za nagrodę.<br>
<br>
<br><br>
<h3><span class="color-blue">Wytwarzanie legendarnych zbroi</span></h3>Legendarne zbroje są specjalnym typem wytwarzanych przedmiotów, które podlegają szczególnym zasadom tworzenia. Wytworzyć legendarne zbroje można u postaci Melio, Drohi, Drimi występujących w Kuźni Giriela w mieście Mirvenis-Adur. Podczas tworzenia legendarnej zbroi, możliwe są do wyboru trzy warianty, różniące się bonusem legendarnym, dla każdej profesji.<br>
<br>
Składniki do wytworzenia zbroi na określony poziom są następujące:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 1 milion sztuk złota.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• 100 sztuk Esencji Sakryfikacji, pochodzącej z rozbijania przedmiotów w module rzemiosła (nie dotyczy zbroi na poziomie 300).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Sztabek platyny, wymienianych w zamian za 100 milionów złota (u Kowala Jaki), w ilości:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 5 sztuk - zbroje na poziom 40, 58, 70.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 6 sztuk - zbroje na poziom 83, 100.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 7 sztuk - zbroje na poziom 120, 144.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 8 sztuk - zbroje na poziom 163, 180, 190.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 9 sztuk - zbroje na poziom 210, 227.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 sztuk - zbroje na poziom 244, 271.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 20 sztuk - zbroje na poziom 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Kamienie dostępne z elit II oraz herosów, będących poziomowo w sąsiedztwie legendarnej zbroi, w ilości:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 40: 3 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 58: 5 sztuk różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 70: 2 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 83: 6 sztuk różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 100: 4 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 120: 7 sztuk różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 144: 5 sztuk różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 163: 5 sztuk różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 180: 3 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 190: 6 sztuk różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 210: 3 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 227: 3 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 244: 3 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 271: 4 sztuki różnych heroicznych kamieni.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zbroja na poziom 300: 3 sztuki różnych legendarnych kamieni.<br>
<br>
Szanse na zdobycie kamienia na odpowiedni poziom z elity II lub herosa, zależą od liczby kamieni wymaganych do utworzenia legendarnej zbroi oraz od liczby źródeł pozyskania tego samego kamienia. <br>
W przypadku mniejszej liczby wymaganych kamieni - szansa na zdobycie kamienia jest odpowiednio niższa.<br>
W przypadku większej liczby źródeł tego samego kamienia - szansa na zdobycie kamienia jest odpowiednio niższa.<br>
<br>
Legendarne zbroje po utworzeniu są permanentnie związane.<br>
Zbroje na poziom 300 poza bonusem za nagrodę, posiadają 3 dodatkowe bonusy.<br>
<br>
Legendarne zbroje można wymieniać na zezwolenia na inną legendarną zbroję u postaci Tharin, a zezwolenia na inną legendarną zbroję, która jest na ten sam poziom co zbroja pierwotna, u postaci Kazdrin. Warunki otrzymania zezwolenia są następujące:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Legendarna zbroja oraz 8000 SŁ - poziom zbroi od 40 do 100.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Legendarna zbroja oraz 10000 SŁ - poziom zbroi od 120 do 190.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Legendarna zbroja oraz 12000 SŁ - poziom zbroi od 210 do 300.<br>
<b><a href="https://youtube.com/shorts/Pyj8w61RmLo">Krótki film</a></b> wizualizujący proces wymiany legendarnych zbroi.<br>
<br>
<br><br>
<h3><span class="color-blue">Poziom przedmiotu</span></h3>W celu wyekwipowania przedmiotu, poziom postaci gracza nie może być mniejszy niż poziom przedmiotu.<br>
Przedmioty mogą posiadać atrybut <code>lvladjust</code>, który sprawia, że po utworzeniu przedmiotu w ekwipunku gracza, jego poziom jest ustalany na podstawie najniższego poziomu dozwolonego, który jest niższy od poziomu postaci. Dozwolone poziomy, jakie mogą wystąpić w przedmiocie, różnią się o 5 i są zależne od klasy przedmiotu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dla zestawu <b>broni</b> (jednoręczne, dwuręczne, półtoraręczne, pomocnicze, dystansowe, różdżka, orb magiczny, kołczan, tarcza) dozwolone poziomy kończą się cyfrą 5 lub 0 (na przykład: 55, 60, 65, 70).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dla zestawu <b>pancerzy</b> (zbroja, hełm, rękawice, buty) dozwolone poziomy kończą się cyfrą 2 i 7 (na przykład: 52, 57, 62, 67).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dla zestawu <b>biżuterii</b> (pierścień, naszyjnik) dozwolone poziomy kończą się cyfrą 1 i 6 (na przykład: 51, 56, 61, 66).<br>
Poziom przedmiotu nie może być mniejszy niż 40 oraz większy niż 300.<br>
<b><a href="https://youtube.com/shorts/6YXHdaM9mVY">Krótki film</a></b> omawiający przedmioty z poziomem przystosowującym się do postaci gracza.<br>
<br>
<br><br>
<h3><span class="color-blue">Wiązanie przedmiotów</span></h3>Przedmioty ekwipowalne mogą znajdować się w jednym z czterech stanów związania z graczem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Brak wzmianki odnośnie wiązania - przedmiot nie jest związany z graczem i nie wiąże się z nim po wyekwipowaniu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wiąże po założeniu (<code>binds</code>) - przedmiot nie jest związany z graczem, ale wiąże się z nim po założeniu, ulepszeniu lub użyciu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Związany z właścicielem (<code>soulbound</code>) - przedmiot został związany z graczem w wyniku wyekwipowania, ulepszenia lub użycia, ale może zostać odwiązany poprzez użycie na nim odpowiedniego przedmiotu, poprzez aukcję lub handel. <b><a href="https://www.youtube.com/shorts/P59CaZoa0tk">Krótki film</a></b> obrazujący proces odwiązywania przedmiotu w handlu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Związany z właścicielem na stałe (<code>permbound</code>) - przedmiot jest związany z graczem i nie można go odwiązać.<br>
<br>
Zmiana stanu wiązania przedmiotu powoduje utratę możliwości wykonania na nim części akcji. Zestawienie dozwolonych czynności zostało zestawione w poniższej tabeli.<br>
<br>
<br><table id="t329" style="width:500px">
<tbody><tr><th colspan="3" style="background-color:#546dd2"><center>Akcje możliwe do wykonania na przedmiotach</center></th></tr><tr><th><center>Akcja wykonywana na przedmiocie</center></th><th><center>Czy akcja jest dozwolona na przedmiocie związanym</center></th><th><center>Czy akcja jest dozwolona na przedmiocie związanym na stałe</center></th></tr><tr><th><center>Założenie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Przełożenie w torbie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Zniszczenie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Wyrzucenie</center></th><td><span class="color-red"><center>Nie</center></span></td><td><span class="color-red"><center>Nie</center></span></td></tr><tr><th><center>Wystawienie na aukcję</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-red"><center>Nie</center></span></td></tr><tr><th><center>Przechowanie w depozycie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Przechowanie w depozycie klanowym</center></th><td><span class="color-red"><center>Nie</center></span></td><td><span class="color-red"><center>Nie</center></span></td></tr><tr><th><center>Przesłanie pocztą</center></th><td><span class="color-red"><center>Nie</center></span></td><td><span class="color-red"><center>Nie</center></span></td></tr><tr><th><center>Sprzedanie u handlarza</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Przekazanie w handlu</center></th><td><span class="color-red"><center>Nie</center></span></td><td><span class="color-red"><center>Nie</center></span></td></tr><tr><th><center>Ulepszenie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Ekstrakcja</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Rozbicie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Przekucie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Obniżenie wymagań</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Pokazywanie w handlu</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Pokazywanie na chatcie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-light-green"><center>Tak</center></span></td></tr><tr><th><center>Odwiązanie</center></th><td><span class="color-light-green"><center>Tak</center></span></td><td><span class="color-red"><center>Nie</center></span></td></tr></tbody></table><br><br>
Każdy przedmiot możliwy do ulepszenia lub będący składnikiem ulepszenia, wiąże po założeniu lub jest związany z właścicielem.<br>
<br>
Przedmioty, które zawsze są związane na stałe z właścicielem:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty pochodzące z tytanów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty pochodzące z wszelkich potworów posiadających osobisty łup (kolosi, kolosi eventowi, elity III eventowe).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty ekwipowalne będące nagrodą za wykonanie zadania.<br>
<br>
<br><br>
<h3><span class="color-blue">Zestawy do walk (zestaw ekwipunku)</span></h3>W interfejsie użytkownika, w prawym górnym rogu sekcji ekwipunku postaci, znajduje przycisk zmiany zestawu do walki. Odpowiada on za stan, w którym znajduje się obecnie ekwipunek postaci. Stan ekwipunku zapamiętuje bieżące ułożenie przedmiotów w ekwipunku postaci oraz wybrany zestaw umiejętności. Zmiana stanu ekwipunku do zestawu <code>X</code> powoduje przywrócenie wyekwipowanych przedmiotów oraz zestawu umiejętności do stanu, w którym był przed przełączeniem z zestawu <code>X</code> do innego zestawu. <br>
Dodatkowe właściwości zestawów do walk:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Każda postać może korzystać z trzech zestawów do walk, jednak za złoto lub Smocze Łuski można zakupić sześć dodatkowych zestawów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• W przypadku, gdy przedmiotu należący do zestawu ekwipunku nie ma w żadnej z toreb należących do postaci, miejsce w ekwipunku dla danej klasy przedmiotu pozostaje puste.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• W przypadku, gdy podczas zmiany zestawu przedmioty mają być zdjęte, ale w torbie brakuje miejsca, próba zdjęcia przedmiotu kończy się niepowodzeniem i zostaje on na swojej pozycji, jednak zestaw ekwipunku się nie nadpisuje.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przełożenie przedmiotu, który jest w danym zestawie, do depozytu, nie powoduje usunięcie go z zestawów. Ponowne przeniesienie do torby postaci przedmiotu, który został wcześniej przypisany do któregokolwiek zestawu, zachowuje to przypisanie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Odwiązanie przedmiotu powoduje jego usunięcie ze wszystkich zestawów. Do zestawów mogą być przypisane wyłącznie przedmioty, które są związane z postacią (widnieje na nich informacja <i>Związany z właścicielem</i> lub <i>Związany na stałe z właścicielem</i>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zestawy można modyfikować tylko po wybraniu ich na postaci. Nie można modyfikować zestawu do walki, który nie jest aktywny w danej chwili na postaci.<br>
<b><a href="https://youtube.com/shorts/zQB2twbPlJ0">Krótki film</a></b> opisujący obsługę zestawów do walki.<br>
<br>
<br>
<br><br>
<h3><span class="color-blue">Odzyskiwanie przedmiotów</span></h3>Zniszczone lub sprzedane u handlarza przedmioty o rzadkości wyższej niż unikatowa, można odzyskać korzystając z przycisku <i>Odzyskaj przedmioty</i> mieszczącego się w oknie handlu u dowolnego kupca (NPC). Operacja pobiera Smocze Łuski z Konta i powoduje zmniejszenie bazowej wartości przedmiotu do 1.<br>
Przedmioty zniszczone na skutek braku miejsca w ekwipunku lub spaleniu z wykorzystaniem okna rzemiosła (poprzez ulepszenie innego przedmiotu lub rozbicie na składniki) nie są możliwe do odzyskania.<br>
Jeżeli w walce grupowej podczas wylosowania postaci, której przyznany będzie łup, nie będzie ona miała wolnego miejsca w torbie, losowanie jest powtarzane bez jej udziału.<br>
Zniszczenie przedmiotu przedawnionego (bez względu na rangę) nie powoduje umieszczenia go w oknie odzyskania.<br>
<b><a href="https://youtube.com/shorts/WjVeqzjOWrQ">Krótki film</a></b> omawiający zasady odzyskiwania przedmiotów.<br>
<br>
<br><br>
<a name="k33"></a><b><h3>3.3. System ulepszania przedmiotów</h3></b><br>
System ulepszania pozwala poświęcać przedmioty celem zwiększenia wartości atrybutów innego przedmiotu. Skorzystać z systemu ulepszenia można posługując się modułem <i>Rzemiosła</i> dostępnym od 20 poziomu postaci.<br>
<b><a href="https://youtube.com/shorts/tWD3B2wbXF0">Krótki film</a></b> opisujący ogólne zasady systemu ulepszania oraz <b><a href="https://youtube.com/shorts/8PvNDrhf-pc">zapowiedź</a></b> wprowadzonych już zmian do systemu.<br>
<br>
Z systemu ulepszeń są wyłączone przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Nieekwipowalne (konsumpcyjne, neutralne, waluty, ulepszenia, torby).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przeklęte.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Posiadające stat <code>expire_duration</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Strzały.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Błogosławieństwa.<br>
<br>
Każdy przedmiot, który podlega pod system ulepszeń, ma wartość wyrażaną w <b>punktach ulepszania</b> oraz w walucie <b>punktów rozbicia</b> i może być użyty jako składnik ulepszenia. <br>
• W momencie ulepszenia przedmiotu (produktu), składnik bezpowrotnie znika z torby postaci, a jego punkty ulepszenia są transferowane do produktu i świadczą o poziomie jego ulepszenia. Po przekroczeniu określonego progu wyrażanego w punktach ulepszenia, przedmiot zyskuje poziom ulepszenia. Czynność tę można powtórzyć 5 razy - maksymalny poziom ulepszenia wynosi 5. Każdy poziom ulepszenia podnosi <b>poziom pozorny</b> przedmiotu, który wpływa na wartość jego atrybutów.<br>
• W momencie rozbicia przedmiotu, składnik bezpowrotnie znika z torby postaci, a gracz otrzymuje walutę o równowartości punktów rozbicia przedmiotu. Każdy poziom rzadkości przedmiotu (poza artefaktem) ma osobną walutę i służy ona do:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zwiększenie poziomu ulepszenia produktu tej samej rzadkości z 4 do 5.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przelosowanie dodatkowego bonusu produktu rzadkości wyższej o 1 (dla rzadkości unikatowej, heroicznej, ulepszonej i legendarnej) lub takiej samej (dla rzadkości pospolitej).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Utworzeniu specjalnych przedmiotów poprzez barter (dotyczy tylko legendarnej Esencji Sakryfikacji).<br>
<br>
<h3><span class="color-blue">Poziom przedmiotu a poziom pozorny</span></h3><b>Poziom</b> przedmiotu, to wymagany poziom do założenia przedmiotu. Na poziom wpływ mają następujące czynniki:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zadeklarowany poziom przedmiotu w bazie danych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Obniżenie wymagań przedmiotu poprzez nałożenie na niego statystyki <code>lowreq=N</code> (N to liczba obniżanych poziomów), bez zmiany wartości atrybutów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przekucie przedmiotu o pewien poziom, co zwiększa również wartości jego atrybutów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Poziom postaci w przypadku pozyskiwania przedmiotów z elastycznym poziomem, za który odpowiada atrybut <code>lvladjust</code>.<br>
<br>
<b>Poziom pozorny przedmiotu</b> to poziom, względem którego są obliczane atrybuty (wartość bonusów) przedmiotu. Poziom pozorny oblicza się w następującej kolejności:<br>
1. Pobranie poziomu przedmiotu z szablonu przedmiotu (nie są uwzględniane statystyki zmienne takie jak <code>lowreq</code>).<br>
2. Uwzględnienie zwiększenia poziomu przedmiotu na skutek przekucia.<br>
3. Obliczenie poziomu pozornego przedmiotu na skutek wyrównania siły w walce na Otchłani (pojedynkach 1 vs 1). Jeżeli poziom gracza jest niższy, poziom pozorny jego przedmiotów zwiększa się o różnicę poziomów między graczami.<br>
<code>item_level<sub>virtual</sub> = item_level + max (0 , enemy<sub>lvl</sub> - player<sub>lvl</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>item_level<sub>virtual</sub></code> - poziom pozorny przedmiotu<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>item_level</code> - poziom przedmiotu pobrany z jego oryginalnego szablonu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>player<sub>lvl</sub></code> - poziom gracza posiadającego przedmiot<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>enemy<sub>lvl</sub></code> - poziom przeciwnika<br>
4. Ulepszenie przedmiotu zgodnie ze wzorem:<br>
<code>item<sub>virtual, lvl</sub> = item_level<sub>virtual</sub> + round( item_level<sub>virtual</sub> * 0.03 ) * enhancement_level</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>item_level<sub>virtual</sub></code> - poziom pozorny przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>enhancement_level</code> - poziom ulepszenia przedmiotu (od 0 do 5).<br>
<br>
Poziom pozorny dodatkowo wpływa również na moment rozpoczęcia słabnięcia parametrów zmiennych bonusów legendarnych oraz na moment ich całkowitego wygaszenia. Oba progi są obliczane względem poziomu pozornego przedmiotu.<br>
<b><a href="https://youtube.com/shorts/5_3_IKvZb8I">Krótki film</a></b> opisujący mechanikę wzrostu poziomu pozornego przedmiotu.<br>
<br>
<h3><span class="color-blue">Wartość składników systemu ulepszenia</span></h3>Każdy przedmiot objęty systemem ulepszenia, którego wartość rzemieślnicza jest różna od zera, ma wartość wyrażaną w punktach ulepszenia (objawiającą się podczas korzystania z przedmiotu jako składnik ulepszenia innego przedmiotu) oraz wartość wyrażaną w punktach rozbicia (objawiającą się podczas rozbicia przedmiotu i otrzymania odpowiadającej jego rzadkości waluty).<br>
<br>
Wartość przedmiotu w punktach ulepszania opisana jest następującym wzorem:<br>
<code>upgrade_points<sub>item</sub> = 0.1 * upgrade_rarity_factor<sub>item</sub> * (180 + lvl<sub>item</sub>) * artisanbon</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_rarity_factor<sub>item</sub></code> - współczynnik rzadkości ulepszanego przedmiotu <code>item</code> (zestawienie współczynnika znajduje się w <a href="#t331">tabeli</a>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>item</sub></code>- poziom przedmiotu <code>item</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>artisanbon [%]</code>- wartość składnika rzemieślniczego wyrażana w procentach.<br>
<br>
Wartość przedmiotu w punktach rozbicia opisana jest następującym wzorem:<br>
<code>essence_points<sub>item,N</sub> = (lvl<sub>item</sub> / 10 + 10) * (1 + 0.2 * N) * artisanbon</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>essence_points<sub>item,N</sub></code> - liczba punktów rozbicia wyrażanej w odpowiedniej dla przedmiotu <code>item</code> na poziomie ulepszenia <code>N</code> rzadkości.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>N</code> - poziom ulepszenia przedmiotu (od 0 do 5).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>artisanbon [%]</code> - wartość składnika rzemieślniczego wyrażana w procentach.<br>
<br>
Punkty rozbicia są wyrażane za pomocą odpowiedniej dla danej rzadkości przedmiotu waluty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Okruchy przeciętności (waluta za rozbicie przedmiotów pospolitych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Ekstrakt unikalności (waluta za rozbicie przedmiotów unikatowych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przyzmat heroicznej magii (waluta za rozbicie przedmiotów heroicznych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Płomień lepszej mocy (waluta za rozbicie przedmiotów ulepszonych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Esencja sakryfikacji (waluta za rozbicie przedmiotów legendarnych).<br>
<br>
<h3><span class="color-blue">Ulepszanie przedmiotu</span></h3>Przedmiot (produkt) można ulepszyć innymi przedmiotami (składnikami) przy użyciu operacji ulepszania w module Rzemiosła. Podczas tej operacji do produktu jest transferowana liczba punktów ulepszenia równa wartości składników. W procesie ulepszania zarówno jako produkt jak i składnik mogą brać udział tylko przedmioty z wymaganym poziomem równym lub przewyższającym 20.<br>
W trakcie operacji pojedynczy przedmiot może wnieść większą wartość punktów ulepszenia w produkt, w przypadku spełnienia określonych warunków:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeśli klasa przedmiotu produktu i składnika jest taka sama, liczba punktów ulepszenia rośnie o 25% wartości początkowej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeśli rzadkość przedmiotu produktu i składnika jest taka sama, liczba punktów ulepszenia rośnie o 200% wartości początkowej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeśli zarówno klasa oraz rzadkość przedmiotu produktu i składnika jest taka sama, liczba punktów ulepszenia rośnie o 225% wartości początkowej.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Jeśli produkt i składnik to ten sam przedmiot (duplikat), liczba punktów ulepszenia rośnie o 300% wartości początkowej.<br>
Maksymalny wzrost wartości w punkach ulepszania wynosi więc sumarycznie 300% - podczas operacji transferowana jest czterokrotność liczby punktów ulepszania z przedmiotu.<br>
<br>
Istnieją dodatkowe przedmioty ulepszające, które wystarczy użyć na przedmiocie ulepszanym, by zwiększyć jego liczbę punktów. Są one klasy <i>Ulepszenia</i> i dzielą się na:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty ulepszające o jeden punkt (<code>enhancement_add_point</code>) - liczba punktów ulepszenia o jakie rośnie przedmiot zależy od ilości tych przedmiotów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty ulepszające o procent (<code>enhancement_add</code>) - przedmiot zwiększa progres do następnego poziomu ulepszenia przedmiotu o zadany procent. W tym wypadku ma znaczenie moment, w którym korzysta się z przedmiotu - ulepszenie o 10% posiadając poziom ulepszenia +1 oferuje mniej punktów, niż ulepszając o 10% na poziomie ulepszenia +4.<br>
Ulepszenie przedmiotu powoduje jego związanie z właścicielem.<br>
<br>
<h3><span class="color-blue">Koszt ulepszania przedmiotu</span></h3>Koszt ulepszenia przedmiotu, wyrażany w punktach ulepszenia, dla rzadkości innych niż ulepszona, można obliczyć ze wzoru:<br>
<code>upgrade_cost<sub>N,item</sub> = upgrade_rarity_factor<sub>item</sub> * upgrade_level_factor<sub>N</sub> * (180 + lvl<sub>item</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_cost<sub>N,item</sub></code> - liczba punktów ulepszania do zwiększenia poziomu ulepszenia przedmiotu <code>item</code> z zera na <code>N</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>item</sub></code> - poziom przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_level_factor<sub>N</sub></code> - współczynnik poziomu ulepszenia dla poziomu ulepszenia przedmiotu <code>N</code> (zestawiony w tabeli poniżej).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_rarity_factor<sub>item</sub></code> - współczynnik rzadkości ulepszanego przedmiotu <code>item</code> (zestawiony w tabeli poniżej).<br>
<br>
Koszt ulepszenia przedmiotu o rzadkości ulepszonej wynosi:<br>
<code>upgrade_cost = upgrade_level_factor<sub>N</sub> * (150 * lvl<sub>item</sub> + 27000)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_level_factor<sub>N</sub></code> - współczynnik poziomu ulepszenia dla poziomu ulepszenia przedmiotu <code>N</code> (zestawiony w tabeli poniżej).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl<sub>item</sub></code> - poziom przedmiotu.<br>
<br>
Ulepszenie przedmiotu na poziom 5 dodatkowo wymaga uiszczenia opłaty w złocie oraz w punktach rozbicia, ale dopiero w momencie wprowadzenia wymaganych punktów ulepszenia.<br>
Ilość złota potrzebna do ulepszenia przedmiotu na poziom 5 wynosi:<br>
<code>gold_cost = (10 * lvl + 1300) * lvl * upgrade_gold_factor<sub>item</sub></code> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>gold_cost</code> - ilość złota pobierana z postaci gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_gold_factor<sub>item</sub></code> - współczynnik złota ulepszanego przedmiotu <code>item</code> zależny od jego rzadkości (zestawiony w tabeli poniżej).<br>
<br>
Ilość punktów rozbicia, wyrażanych w walucie odpowiedniej dla rzadkości przedmiotu, które są wymagane do ulepszenia go na poziom 5 wynosi:<br>
<code>essence_cost<sub>item</sub> = 3 * essence_points<sub>item,0</sub></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>essence_cost<sub>item</sub></code> - ilość punktów rozbicia wyrażanych w walucie odpowiadającej dla rzadkości przedmiotu <sub>item</sub> pobierana z postaci gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;essence_points<sub>item,0</sub> - ilość waluty otrzymywanej po rozbiciu nieulepszonego przedmiotu <code>item</code>.<br>
<br>
<br><table id="t331" style="width:500px">
<tbody><tr><th colspan="3" style="background-color:#546dd2"><center>Zestawienie współczynnika poziomu ulepszenia przedmiotu</center></th></tr><tr><th><center>Poziom ulepszenia przedmiotu</center></th><th colspan="2"><center>Współczynnik poziomu ulepszenia<br>(<code>upgrade_level_factor)</code></center></th></tr><tr><th><center>0</center></th><td colspan="2"><center>0.0</center></td></tr><tr><th><center>1</center></th><td colspan="2"><center>1.0</center></td></tr><tr><th><center>2</center></th><td colspan="2"><center>2.1</center></td></tr><tr><th><center>3</center></th><td colspan="2"><center>3.4</center></td></tr><tr><th><center>4</center></th><td colspan="2"><center>5.0</center></td></tr><tr><th><center>5</center></th><td colspan="2"><center>7.0</center></td></tr><tr><th colspan="3" style="background-color:#546dd2"><center>Zestawienie współczynników zależnych od rzadkości przedmiotu</center></th></tr><tr><th><center>Rzadkość przedmiotu</center></th><th><center>Współczynnik rzadkości ulepszanego przedmiotu<br>(<code>upgrade_rarity_factor)</code></center></th><th><center>Współczynnik złota ulepszanego przedmiotu<br>(<code>upgrade_gold_factor</code>)</center></th></tr><tr><th><center>Pospolity</center></th><td><center>1</center></td><td><center>1</center></td></tr><tr><th><center>Unikatowy</center></th><td><center>10</center></td><td><center>10</center></td></tr><tr><th><center>Heroiczny</center></th><td><center>100</center></td><td><center>30</center></td></tr><tr><th><center>Ulepszony</center></th><td><center>-</center></td><td><center>40</center></td></tr><tr><th><center>Legendarny</center></th><td><center>1000</center></td><td><center>60</center></td></tr></tbody></table><br><br>
<br>
<h3><span class="color-blue">Dodatkowa wartość rzemieślnicza</span></h3>Część przedmiotów zawiera dodatkową manualnie ustawianą wartość statystyki <b>artisanbon</b>, która odpowiada za zwiększenie wartości przedmiotu w punktach ulepszenia i punktach rozbicia. Wartość ta powinna być interpretowana jako procentowa wartość przedmiotu, gdzie 100 oznacza 100% wartości, czyli wartość domyślną, natomiast 200 to 200% wartości, czyli wzrost o 100%.<br>
Wartość rzemieślnicza może w specjalnych przedmiotach z eventów (które istnieją już w ekwipunkach graczy) rosnąć co rok maksymalnie do 50 punktów procentowych. W przypadku potrzeby zwiększenia wartości rzemieślniczej o więcej niż 50 punktów procenowych, wartość rzemieślnicza w przedmiotach istniejących już w grze nie ulega zmianie, natomiast jest dodawana nowa seria takich samych (lub podobnych) przedmiotów.<br>
<br>
<br><table id="t332" style="width:500px">
<tbody><tr><th colspan="2" style="background-color:#546dd2"><center>Bonus artisanbon w zalezności od pochodzenia przedmiotu</center></th></tr><tr><th><center>Pochodzenie</center></th><th><center>Mnożnik rzemieślniczy<br>(<code>artisanbon</code>)</center></th></tr><tr><th><center>Handlarze przedmiotów za złoto</center></th><td><center>0</center></td></tr><tr><th><center>Kolos wiosenny<br>(event)</center></th><td><center>250</center></td></tr><tr><th><center>Kolos jesienny<br>(event)</center></th><td><center>250</center></td></tr><tr><th><center>Elity III Eventowe</center></th><td><center>150</center></td></tr><tr><th><center>Skrzynia z Otchłani</center></th><td><center>250</center></td></tr><tr><th><center>Skrzynia Smoczych Kowali</center></th><td><center>losowo<br>od 150 do 250</center></td></tr><tr><th><center>Pozostałe</center></th><td><center>100</center></td></tr></tbody></table><br><br>
<br>
<h3><span class="color-blue">Dodatkowy bonus do przedmiotu wynikający z ulepszenia</span></h3>Ulepszenie przedmiotu na poziom 5 umożliwia graczowi wybór jednego z trzech wylosowanych z określonej puli (zależnej od klasy przedmiotu) bonusu, który dołączy do listy atrybutów przedmiotu. Sam wybór bonusu jest darmowy. Wybranie bonusu lub przerolowanie bonusu zawsze powoduje związanie przedmiotu z właścicielem.<br>
<b><a href="https://youtube.com/shorts/1uguEuROSEM">Krótki film</a></b> wizualizujący proces wyboru bonusu.<br>
Klasy przedmiotów zostały podzielone na trzy <b>zestawy</b>, które posiadają odrębną pulę losowanych w tym systemie bonusów. <br>
• Do zestawu <b>broni</b> zaliczamy klasy: jednoręczne, dwuręczne, półtoraręczne, pomocnicze, dystansowe, różdżka, orb magiczny, kołczan.<br>
• Do zestawu <b>pancerzy</b> zaliczamy klasy: zbroja, hełm, rękawice, buty, tarcza.<br>
• Do zestawu <b>biżuterii</b> zaliczamy klasy: pierścień, naszyjnik.<br>
<br>
Bonusy natomiast należą do jednej z trzech <b>grup</b>, które różnią się od siebie szansą na wylosowanie dowolnego bonusu z grupy. Szansa ta określona jest poprzez <b>moc bonusu</b> i obliczana jest poprzez iloraz mocy bonusu z sumą mocy wszystkich dostępnych bonusów ze wszystkich grup danego zestawu:<br>
<code>p(bonus) = power<sub>bonus</sub> / (<sup>Ω</sup>Σ<sub>ω</sub> power<sub>ω</sub>)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>p(bonus)</code> - szansa na wylosowanie bonusu <code>bonus</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>power<sub>bonus</sub></code> - moc bonusu <code>bonus</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>power<sub>ω</sub></code> - moc bonusu <code>ω</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>Ω</code> - zbiór wszystkich dostępnych bonusów bonusów w puli.<br>
Podczas losowania trzech dostępnych bonusów, nie mogą wystąpić powtórzenia, zatem obecność jednego bonusu wyrzuca go z puli dostępnych do wylosowania bonusów.<br>
<br>
Zestawienie mocy bonusów oraz puli dla określonych zestawów oraz grup, zostało zaprezentowane w tabeli poniżej.<br>
<br>
<br><table id="t333" style="width:500px">
<tbody><tr><th colspan="4" style="background-color:#546dd2"><center>Zestawienie mocy bonusów, zestawów oraz grup</center></th></tr><tr><th><center>Klasyfikator</center></th><th><center>Grupa I</center></th><th><center>Grupa II</center></th><th><center>Grupa III</center></th></tr><tr><th><center>Moc pojedynczego bonusu</center></th><td><center>10</center></td><td><center>5</center></td><td><center>1</center></td></tr><tr><th><center>Zestaw broni</center></th><td>• Wszystkie cechy<br>• Intelekt<br>• Siła<br>• Zręczność</td><td>• Szybkość ataku<br>• Cios krytyczny</td><td>• Niszczenie pancerza<br>• Niszczenie odporności<br>• Niszczenie energii<br>• Niszczenie many<br>• Niszczenie absorpcji</td></tr><tr><th><center>Zestaw pancerzy</center></th><td>• Wszystkie cechy<br>• Intelekt<br>• Siła<br>• Zręczność</td><td>• Pancerz<br>• Odporność na ogień<br>• Odporność na zimno<br>• Odporność na błyskawice<br>• Odporność na truciznę</td><td>• Życie<br>• Blok<br>• Absorpcja<br>• Absorpcja magiczna<br>• Unik</td></tr><tr><th><center>Zestaw biżuterii</center></th><td>• Wszystkie cechy<br>• Intelekt<br>• Siła<br>• Zręczność</td><td>• Energia<br>• Mana<br>• Siła ciosu krytycznego fizycznego<br>• Siła ciosu krytycznego magicznego<br>• Obniżanie szansy na cios krytyczny przeciwnika</td><td>• Leczenie<br>• Spowolnienie<br>• Zmniejszanie uniku przeciwnika</td></tr></tbody></table><br><br>
<br>
Przelosowanie bonusu polega na zmianie dodatkowego bonusu wynikającego z ulepszenia na inny, który również jest dostępny dla danej grupy przedmiotów. Przelosowanie polega na zaproponowanie graczowi do wyboru 3 bonusów z puli. Pierwszy bonus jest tym, który został wybrany przez gracza podczas poprzedniego losowania (również podczas pierwszego ulepszania na +5), natomiast pozostałe dwa są losowane z puli metodą "bez powtórzeń". Oznacza to, że suma mocy zbioru jest różna w zależności od tego, jaki bonus aktualnie gracz posiada w przedmiocie. Celując w wylosowanie określonego bonus, warto mieć przypisany do przedmiotu bonus z największą mocą, ponieważ najbardziej "odchudza" on zbiór.<br>
<br>
Dodatkowy bonus można przelosować poprzez:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Użycie specjalnego przedmiotu konsumpcyjnego zmieniającego wylosowanie bonusu (posiadającego atrybut <code>bonus_reselect</code>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Wybór specjalnej opcji dialogowej u kowali:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Alrik (Torneg)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Unil (Ithan)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Jaki (Mirvenis-Adur)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Frasson (Mythar)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Kendal (Tuzmer)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Granihotems (Brama Północy)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Drowin (Thuzal)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Thorgrim (Karka-han)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kowal Grisza (Nithal)<br>
<br>
Przelosowanie bonusu u handlarzy wymaga odpowiedniej opłaty w punktach rozbicia. Załóżmy, że <code>item</code> to przedmiot o tym samym poziomie co przedmiot (unikatowej, heroicznej/ulepszonej lub legendarnej), u którego chcemy przelosować bonus, jednak o rzadkości o jeden niższej. Wtedy koszt w punktach rozbicia do przelosowania bonusu wynosi:<br>
<code>essence_cost = 3 * essence_points<sub>item,0</sub></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>essence_cost<sub>item</sub></code> - ilość punktów rozbicia wyrażanych w walucie odpowiadającej dla rzadkości przedmiotu <sub>item</sub> pobierana z postaci gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;essence_points<sub>item,0</sub> - ilość waluty otrzymywanej po rozbiciu nieulepszonego przedmiotu <code>item</code>.<br>
Przelosowanie bonusu w przedmiocie pospolitym wymaga wyjątkowo pospolitych punktów rozbicia (Okruchów przeciętności). W przypadku przedmiotów wyższej rzadkości, waluta potrzebna do przelosowania bonusu jest o jeden poziom rzadkości niższa.<br>
<i>Przykład</i>: przelosowanie bonusu w przedmiocie heroicznym wymaga Ekstraktu unikalności.<br>
Do przelosowania bonusu w przedmiocie pospolitym są natomiast wymagane Okruchy przeciętności w ilości:<br>
<code>essence_cost = essence_points<sub>item,0</sub></code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>essence_cost<sub>item</sub></code> - ilość punktów rozbicia wyrażanych w walucie odpowiadającej dla rzadkości przedmiotu <sub>item</sub> pobierana z postaci gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;essence_points<sub>item,0</sub> - ilość waluty otrzymywanej po rozbiciu nieulepszonego przedmiotu <code>item</code>.<br>
<br>
<br><br>
<h3><span class="color-blue">Ekstrakcja</span></h3>Ekstrakcja jest opcją dostępną w module Rzemiosła, która umożliwia odzyskanie części zasobów poświęconych na ulepszenie przedmiotu, w postaci:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punktów ulepszenia wyrażanych poprzez Kryształową kulę, osobną dla każdego poziomu rzadkości przedmiotu, która umożliwia przeniesienie punktów ulepszenia <b>wyłącznie</b> do przedmiotów posiadających tę samą rzadkość (na skutek występowania atrybutu <code>target_rarity</code>). <b><a href="https://youtube.com/shorts/R0LBkk4Xkc8">Krótki film</a></b> opisujący działanie Kryształowych kul.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kryształowa kula pospolitej magii (w przypadku eksktracji przedmiotów pospolitych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kryształowa kula unikatowej magii (w przypadku eksktracji przedmiotów unikatowych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kryształowa kula heroicznej magii (w przypadku eksktracji przedmiotów heroicznych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kryształowa kula ulepszonej magii (w przypadku eksktracji przedmiotów ulepszonych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kryształowa kula legendarnej magii (w przypadku eksktracji przedmiotów legendarnych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Punktów rozbicia (w przypadku ulepszenia przedmiotu na poziom 5) wyrażanych w odpowiedniej walucie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Okruchy przeciętności (w przypadku eksktracji przedmiotów pospolitych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ekstrakt unikalności (w przypadku eksktracji przedmiotów unikatowych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przyzmat heroicznej magii (w przypadku eksktracji przedmiotów heroicznych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Płomień lepszej mocy (w przypadku eksktracji przedmiotów ulepszonych).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Esencja sakryfikacji (w przypadku eksktracji przedmiotów legendarnych).<br>
<br>
Użycie Kryształowej kuli wymusza wiązanie ulepszanego przedmiotu z właścicielem. <br>
<br>
Część zasobów, która jest zwracana w wyniku ekstrakcji, wynosi <b>75%</b> punktów ulepszania oraz punktów rozbicia zainwestowanych w przedmiot.<br>
<b><a href="https://youtube.com/shorts/UUbwI80Q9EI">Krótki film</a></b> opisujący działanie ekstrakcji.<br>
<br>
Operację ekstrakcji można dokonać płacąc w złocie lub w Smoczych Łuskach.<br>
Koszt wykonania operacji ekstrakcji wyrażony w złocie wynosi:<br>
<code>extraction_gold_cost = 60 * upgrade_points</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>extraction_gold_cost</code> - koszt ekstrakcji w złocie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_points</code> - liczba punktów ulepszenia, która została zainwestowana w przedmiot.<br>
Koszt wykonania operacji ekstrakcji wyrażony w Smoczych Łuskach wynosi:<br>
<code>extraction_dt_cost = 0.001 * upgrade_points</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>extraction_dt_cost</code> - koszt ekstrakcji w Smoczych Łuskach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>upgrade_points</code> - liczba punktów ulepszenia, która została zainwestowana w przedmiot.<br>
<br>
Istnieją przedmioty, na których można dokonać skończonej liczby ekstrakcji zwracającej wszystkie zasoby, jakie zostały zainwestowane w przedmiot. Mają one zaznaczoną specjalną statystykę <code>enhancement_refund=N</code> opisaną jako <i>Ekstrakcja przywróci wszystkie zasoby</i>, gdzie <code>N</code> oznacza liczbę ekstrakcji, jaką można przeprowadzić na przedmiocie, podczas których nie traci się żadnych zasobów. Koszt ekstrakcji takiego przedmiotu nie ulega zmianie (nie jest ona darmowa).<br>
Przedmiot ma opisaną liczbę ekstrakcji przywracających pełnię zasobów tylko wtedy, kiedy jest ona większa od 1.<br>
Odwiązanie takiego przedmiotu (przy użyciu przedmiotu, aukcji lub handlu) powoduje całkowitą utratę tej statystyki.<br>
Istnieją przedmioty ulepszające, które nakładają statystykę <code>enhancement_refund</code>. Sprawiają, że wartość statystyki wzrasta o 1. Użycie tego przedmiotu ulepszającego zawsze powoduje związanie przedmiotu ulepszanego z właścicielem.<br>
<br>
<br>
<br><br>
<a name="k34"></a><b><h3>3.4. System przekuwania przedmiotów</h3></b><br>
System przekuwania dotyczy tylko przedmiotów posiadających atrybut <code>lvlupgs</code>. W atrybutach tych przedmiotów widnieje informacja o <b>koszcie przekucia</b> przedmiotu oraz <b>ilości przekuć</b>. Z systemu przekuwania są wyłączone również przedmioty, które mają obniżone wymagania poziomowe (atrybut <code>lowreq</code>).<br>
<b><a href="https://youtube.com/shorts/YOGczq8TVNc">Krótki film</a></b> opisujący ogólne zasady systemu przekuwania.<br>
<br>
<h3><span class="color-blue">Przekuwanie przedmiotów</span></h3>Przekucie przedmiotu to zwiększenie jego <b>poziomu</b> o 1 po każdym wykonaniu operacji. Wpływa więc ono na wartości atrybutów przedmiotu oraz jego wymagania. Wzrost poziomu powoduje:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Uniemożliwienie obniżenia wymagań poziomowych przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększenie wymaganego poziomu do założenia przedmiotu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększenie wartości atrybutów przedmiotu do nowego poziomu po przekuciu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększenie wymaganej liczby punktów ulepszenia oraz punktów rozbicia w celu ulepszenia przedmiotu w module rzemiosła.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zwiększenie poziomu broni, od którego obliczany jest poziom pozorny przedmiotu (z faktu ulepszenia i nierównej walki na Otchłani).<br>
Maksymalna dozwolona liczba wykonania tej operacji jest określana poprzez atrybut <code>lvlupgs</code>. <br>
<br>
Z mechanizmu przekucia wyłączone są przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Bez podanej dostępnej liczby przekuć (bez atrybutu <code>lvlupgs</code>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Z obniżonym wymaganiem poziomowym (z atrybutem <code>lowreq</code>).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Posiadające poziom 300.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Przedmioty nieekwipowalne.<br>
<br>
Operacja wymaga użycia na danym przedmiocie specjalnego surowca klasy <i>Ulepszenia</i>, posiadającego atrybut <code>upglvl</code>, który określa zestaw klas przedmiotów możliwych do przekucia za jego pomocą.<br>
Dozwolone zestawy to:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zestaw <b>bronie</b> (weapon), grupujący klasy: jednoręczne, dwuręczne, półtoraręczne, pomocnicze, dystansowe, różdżka, orb magiczny, kołczan, tarcza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zestaw <b>pancerzy</b> (armor), grupujący klasy: zbroja, hełm, rękawice, buty.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Zestaw <b>biżuterii</b> (jewels), grupujący klasy: pierścień, naszyjnik.<br>
<br>
Dodatkowo przedmioty ulepszające mogą wymagać określonej rzadkości (atrybut <code>target_rarity</code>) przedmiotu przekuwanego: pospolitej, unikatowej, heroicznej, ulepszonej, legendarnej.<br>
<br><br>
<h3><span class="color-blue">Koszt przekucia</span></h3>Koszt przekucia jest zależny klasy oraz rzadkości przedmiotu i wyraża się go wzorem:<br>
<code>forging_cost = 5 * bonus_amount</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>forging_cost</code> - koszt przekucia przedmiotu wyrażony w liczbie specjalnej waluty.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>bonus_amount</code> - liczba bonusów możliwych do rozdania w przedmiocie danego typu o danej rzadkości.<br>
Zestawienie liczby bonusów w przedmiotach znajduje się w <a href="#t321">tabeli</a>.<br>
<br>
Dodatkowe bonusy a wzrost kosztu przekucia:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowy bonus typu nagroda wpływa na koszt przekucia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowy bonus wynikający z ulepszenia na poziom 5 nie wpłwa na koszt przekucia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Dodatkowy bonus przeklęty w przedmiotach przeklętych wpływa na koszt przekucia.<br>
<br><br>
<h3><span class="color-blue">Cofnięcie przekucia</span></h3>Operację przekucia można cofnąć, jeżeli na danym przedmiocie zostanie użyty specjalny Zwój oczyszczenia (przedmiot z trybutem <code>undoupg</code>). Podczas cofnięcia przekucia, zwracana jest domyślna liczba przekuć, o którą można na nowo zwiększyć poziom przedmiotu, a poziom przedmiotu jest przywracany do bazowego. Nie można jednak cofnąć operacji przekucia, jeżeli poziom przedmiotu jest elastyczny (dopasowuje się do poziomu gracza na skutek atrybutu <code>lvladjust</code>).<br>
<br>
<br><br>
<a name="k35"></a><b><h3>3.5. Statystyki NPC</h3></b><br>
<h3><span class="color-blue">Statystyki natywne</span></h3>Każdy typ potwora posiada inny zestaw mnożników statystyk względem potwora bezklasowego, który z kolei uzależnia swoją siłę wyłącznie od swojego poziomu. <br>
Dostępne są następujące typy potworów:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Potwór zwyczajny<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Elita<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Elita II<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Elita III<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Heros<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tytan<br>
<br>
Istnieje dodatkowy wyświetlany osobny typ potwora - <b>Kolos</b>, który jest odpowiednikiem Tytanów dla map typu <b>Próba sił</b>. Kolosi zachowują ten sam szablon statystyk, jednak od Tytanów różnią się sposobem rozdzielania łupu, szablonem przedmiotów, ustawieniami mapy, czasem odrodzenia.<br>
Zestawienie typów potworów oraz ich siły zostało zestawione w poniższej tabeli.<br>
<br>
<br><table id="t351" style="width:750px">
<tbody><tr><th colspan="9" style="background-color:#546dd2"><center>Zestawienie statystyk potworów</center></th></tr><tr><th><center>Profesja</center></th><th><center>Mnożnik<br>pancerza</center></th><th><center>Mnożnik<br>odporności<br>magicznej</center></th><th><center>Mnożnik<br>odporności<br>na truciznę</center></th><th><center>Mnożnik<br>obrażeń<br>fizycznych</center></th><th><center>Mnożnik<br>obrażeń<br>magicznych</center></th><th><center>Mnożnik<br>życia</center></th><th><center>Mnożnik<br>szybkości<br>ataku</center></th><th><center>Statystyki<br>dodatkowe</center></th></tr><tr><th colspan="9"><center>Potwór zwyczajny</center></th></tr><tr><td><center>Wojownik</center></td><td><center>2.0</center></td><td><center>0.0</center></td><td><center>0.2</center></td><td><center>3.0</center></td><td><center>0.0</center></td><td><center>0.7</center></td><td><center>1.0</center></td><td><center>-</center></td></tr><tr><td><center>Wojownik<br>z tarczą</center></td><td><center>2.5</center></td><td><center>0.0</center></td><td><center>0.5</center></td><td><center>2.3</center></td><td><center>0.0</center></td><td><center>1.0</center></td><td><center>0.8</center></td><td><center>-</center></td></tr><tr><td><center>Wojownik<br>z trucizną</center></td><td><center>2.0</center></td><td><center>0.0</center></td><td><center>0.3</center></td><td><center>2.3</center></td><td><center>0.0</center></td><td><center>0.7</center></td><td><center>1.0</center></td><td><center>trucizna (slow): lvl<br>trucizna (dmg): 0.8</center></td></tr><tr><td><center>Paladyn</center></td><td><center>2.0</center></td><td><center>0.0</center></td><td><center>0.3</center></td><td><center>2.6</center></td><td><center>2.0</center></td><td><center>0.6</center></td><td><center>1.0</center></td><td><center>blok: 15</center></td></tr><tr><td><center>Mag</center></td><td><center>1.5</center></td><td><center>0.0</center></td><td><center>0.1</center></td><td><center>0.0</center></td><td><center>3.0</center></td><td><center>0.6</center></td><td><center>1.0</center></td><td><center>-</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>1.5</center></td><td><center>0.0</center></td><td><center>0.3</center></td><td><center>2.0</center></td><td><center>2.5</center></td><td><center>0.6</center></td><td><center>1.1</center></td><td><center>unik: 2.0<br>przebicie: 15</center></td></tr><tr><td><center>Łowca</center></td><td><center>1.5</center></td><td><center>0.0</center></td><td><center>0.5</center></td><td><center>2.3</center></td><td><center>0.0</center></td><td><center>0.6</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 17</center></td></tr><tr><td><center>Łowca<br>z trucizną</center></td><td><center>1.5</center></td><td><center>0.0</center></td><td><center>0.7</center></td><td><center>2.0</center></td><td><center>0.0</center></td><td><center>0.6</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 17<br>trucizna (slow): lvl<br>trucizna (dmg): 0.8</center></td></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>1.5</center></td><td><center>0.0</center></td><td><center>0.2</center></td><td><center>2.3</center></td><td><center>0.0</center></td><td><center>0.6</center></td><td><center>1.2</center></td><td><center>obrażenia pomocnicze<br>unik: 4.0<br>trzeci cios: 5</center></td></tr><tr><th colspan="9"><center>Elita</center></th></tr><tr><td><center>Wojownik</center></td><td><center>2.4</center></td><td><center>1.0</center></td><td><center>0.6</center></td><td><center>3.6</center></td><td><center>0.0</center></td><td><center>3.0</center></td><td><center>1.0</center></td><td><center>-</center></td></tr><tr><td><center>Paladyn</center></td><td><center>2.4</center></td><td><center>1.0</center></td><td><center>0.4</center></td><td><center>3.2</center></td><td><center>2.3</center></td><td><center>2.4</center></td><td><center>1.0</center></td><td><center>blok: 17</center></td></tr><tr><td><center>Mag</center></td><td><center>1.8</center></td><td><center>1.0</center></td><td><center>0.2</center></td><td><center>0.0</center></td><td><center>3.6</center></td><td><center>2.4</center></td><td><center>1.0</center></td><td><center>absorpcja dystansowa: 20</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>1.8</center></td><td><center>1.0</center></td><td><center>0.4</center></td><td><center>2.3</center></td><td><center>3.0</center></td><td><center>2.4</center></td><td><center>1.1</center></td><td><center>unik: 2.0<br>przebicie: 17<br>absorpcja dystansowa: 15</center></td></tr><tr><td><center>Łowca</center></td><td><center>1.8</center></td><td><center>1.0</center></td><td><center>0.7</center></td><td><center>2.7</center></td><td><center>0.0</center></td><td><center>2.4</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 19<br>niszczenie pancerza: lvl * 0.3</center></td></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>1.8</center></td><td><center>1.0</center></td><td><center>0.4</center></td><td><center>2.7</center></td><td><center>0.0</center></td><td><center>2.4</center></td><td><center>1.2</center></td><td><center>obrażenia pomocnicze<br>unik: 4.0<br>trzeci cios: 10</center></td></tr><tr><th colspan="9"><center>Elita II</center></th></tr><tr><td><center>Wojownik</center></td><td><center>2.8</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>4.2</center></td><td><center>0.0</center></td><td><center>6.0</center></td><td><center>1.0</center></td><td><center>ogłuszenie: 15<br>niszczenie pancerza: lvl * 0.6</center></td></tr><tr><td><center>Paladyn</center></td><td><center>2.8</center></td><td><center>2.0</center></td><td><center>0.5</center></td><td><center>3.7</center></td><td><center>2.7</center></td><td><center>4.8</center></td><td><center>1.0</center></td><td><center>blok: 19<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.3<br>ogłuszenie: 10</center></td></tr><tr><td><center>Mag</center></td><td><center>2.1</center></td><td><center>2.0</center></td><td><center>0.5</center></td><td><center>0.0</center></td><td><center>4.2</center></td><td><center>4.8</center></td><td><center>1.0</center></td><td><center>absorpcja dystansowa: 25<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.3<br>ogłuszenie: 10</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>2.1</center></td><td><center>2.0</center></td><td><center>0.5</center></td><td><center>2.5</center></td><td><center>3.4</center></td><td><center>4.8</center></td><td><center>1.1</center></td><td><center>unik: 2.0<br>przebicie: 19<br>absorpcja dystansowa: 20<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.3<br>ogłuszenie: 10</center></td></tr><tr><td><center>Łowca</center></td><td><center>2.1</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>3.2</center></td><td><center>0.0</center></td><td><center>4.8</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 21<br>niszczenie pancerza: lvl * 0.5<br>ogłuszenie: 10</center></td></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>2.1</center></td><td><center>2.0</center></td><td><center>0.7</center></td><td><center>3.2</center></td><td><center>0.0</center></td><td><center>4.8</center></td><td><center>1.2</center></td><td><center>obrażenia pomocnicze<br>unik: 4.0<br>trzeci cios: 15<br>niszczenie pancerza: lvl * 0.5<br>ogłuszenie: 10</center></td></tr><tr><th colspan="9"><center>Elita III</center></th></tr><tr><td><center>Wojownik</center></td><td><center>3.2</center></td><td><center>3.0</center></td><td><center>0.5</center></td><td><center>5.2</center></td><td><center>0.0</center></td><td><center>24.0</center></td><td><center>1.0</center></td><td><center>ogłuszenie: 20<br>niszczenie pancerza: lvl * 0.8<br>blok: 10</center></td></tr><tr><td><center>Paladyn</center></td><td><center>3.4</center></td><td><center>3.0</center></td><td><center>0.4</center></td><td><center>4.4</center></td><td><center>3.4</center></td><td><center>22.0</center></td><td><center>1.0</center></td><td><center>blok: 20<br>ogłuszenie: 10<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.6</center></td></tr><tr><td><center>Mag</center></td><td><center>2.2</center></td><td><center>3.0</center></td><td><center>0.4</center></td><td><center>0.0</center></td><td><center>5.2</center></td><td><center>18.0</center></td><td><center>1.0</center></td><td><center>absorpcja dystansowa: 25<br>ogłuszenie: 10<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.2</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>2.2</center></td><td><center>3.0</center></td><td><center>0.6</center></td><td><center>3.3</center></td><td><center>3.8</center></td><td><center>18.0</center></td><td><center>1.1</center></td><td><center>unik: 2.0<br>przebicie: 20<br>absorpcja dystansowa: 25<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.3<br>ogłuszenie: 10</center></td></tr><tr><td><center>Łowca</center></td><td><center>2.4</center></td><td><center>3.0</center></td><td><center>0.8</center></td><td><center>4.0</center></td><td><center>0.0</center></td><td><center>18.0</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 20<br>niszczenie pancerza: lvl * 0.5<br>ogłuszenie: 5</center></td></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>2.6</center></td><td><center>3.0</center></td><td><center>0.6</center></td><td><center>4.4</center></td><td><center>0.0</center></td><td><center>18.0</center></td><td><center>1.1</center></td><td><center>obrażenia pomocnicze<br>unik: 4.0<br>trzeci cios: 15<br>niszczenie pancerza: lvl * 0.6<br>ogłuszenie: 10</center></td></tr><tr><th colspan="9"><center>Heros</center></th></tr><tr><td><center>Wojownik</center></td><td><center>3.2</center></td><td><center>3.0</center></td><td><center>1.0</center></td><td><center>4.8</center></td><td><center>0.0</center></td><td><center>18.0</center></td><td><center>1.0</center></td><td><center>niszczenie pancerza: lvl * 0.7<br>ogłuszenie: 22</center></td></tr><tr><td><center>Paladyn</center></td><td><center>3.2</center></td><td><center>3.0</center></td><td><center>0.6</center></td><td><center>4.0</center></td><td><center>3.0</center></td><td><center>14.4</center></td><td><center>1.0</center></td><td><center>blok: 21<br>niszczenie odporności: 1<br>niszczenie pancerza: lvl * 0.6<br>ogłuszenie: 15</center></td></tr><tr><td><center>Mag</center></td><td><center>2.4</center></td><td><center>3.0</center></td><td><center>0.6</center></td><td><center>0.0</center></td><td><center>4.8</center></td><td><center>14.4</center></td><td><center>1.0</center></td><td><center>absorpcja dystansowa: 30<br>niszczenie odporności: 2<br>niszczenie pancerza: lvl * 0.4<br>ogłuszenie: 15</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>2.4</center></td><td><center>3.0</center></td><td><center>0.9</center></td><td><center>2.8</center></td><td><center>3.8</center></td><td><center>14.4</center></td><td><center>1.1</center></td><td><center>unik: 2.0<br>przebicie: 21<br>absorpcja dystansowa: 20<br>niszczenie odporności: 2<br>niszczenie pancerza: lvl * 0.5<br>ogłuszenie: 15</center></td></tr><tr><td><center>Łowca</center></td><td><center>2.4</center></td><td><center>3.0</center></td><td><center>0.9</center></td><td><center>3.6</center></td><td><center>0.0</center></td><td><center>14.4</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 23<br>niszczenie pancerza: lvl * 0.6<br>ogłuszenie: 15</center></td></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>2.4</center></td><td><center>3.0</center></td><td><center>0.6</center></td><td><center>3.6</center></td><td><center>0.0</center></td><td><center>14.4</center></td><td><center>1.2</center></td><td><center>obrażenia pomocnicze<br>unik: 4.0<br>trzeci cios: 20<br>niszczenie pancerza: lvl * 0.6<br>ogłuszenie: 15</center></td></tr><tr><th colspan="9"><center>Tytan</center></th></tr><tr><td><center>Wojownik</center></td><td><center>3.6</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>12.0</center></td><td><center>0.0</center></td><td><center>75.0</center></td><td><center>1.0</center></td><td><center>niszczenie pancerza: lvl * 0.8<br>ogłuszenie: 30</center></td></tr><tr><td><center>Paladyn</center></td><td><center>3.6</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>10.0</center></td><td><center>8.0</center></td><td><center>60.0</center></td><td><center>1.0</center></td><td><center>blok: 23<br>niszczenie odporności: 2<br>niszczenie pancerza: lvl * 0.7<br>ogłuszenie: 20</center></td></tr><tr><td><center>Mag</center></td><td><center>2.7</center></td><td><center>2.0</center></td><td><center>0.5</center></td><td><center>0.0</center></td><td><center>12.0</center></td><td><center>60.0</center></td><td><center>1.0</center></td><td><center>absorpcja dystansowa: 35<br>niszczenie odporności: 3<br>niszczenie pancerza: lvl * 0.5<br>ogłuszenie: 20</center></td></tr><tr><td><center>Tropiciel</center></td><td><center>2.7</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>8.0</center></td><td><center>10.0</center></td><td><center>60.0</center></td><td><center>1.1</center></td><td><center>unik: 2.0<br>przebicie: 23<br>absorpcja dystansowa: 20<br>niszczenie odporności: 2<br>niszczenie pancerza: lvl * 0.7<br>ogłuszenie: 20</center></td></tr><tr><td><center>Łowca</center></td><td><center>2.7</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>9.0</center></td><td><center>0.0</center></td><td><center>60.0</center></td><td><center>1.3</center></td><td><center>unik: 3.0<br>przebicie: 25<br>niszczenie pancerza: lvl * 0.7<br>ogłuszenie: 20</center></td></tr><tr><td><center>Tancerz ostrzy</center></td><td><center>2.7</center></td><td><center>2.0</center></td><td><center>1.0</center></td><td><center>9.0</center></td><td><center>0.0</center></td><td><center>60.0</center></td><td><center>1.2</center></td><td><center>obrażenia pomocnicze<br>unik: 4.0<br>trzeci cios: 25<br>niszczenie pancerza: lvl * 0.7<br>ogłuszenie: 20</center></td></tr></tbody></table><br><br>
Dokładna wartość obrażeń, życia, pancerza, odporności, uniku oraz absorpcji nie jest upubliczniana. Powyżej zostały opisane jedynie ich proporcje jakimi różnią się między sobą określone typy potworów.<br>
<br>
<h3><span class="color-blue">Statystyki nadane manualnie</span></h3>Część statystyk potwora może zostać nadana lub zmieniona manualnie. Poniżej zostały opisane wszystkie statystyki, które można nadać potworom.<br>
<br>
<br><table id="t351" style="width:750px">				
<tbody><tr><th colspan="2" style="background-color:#546dd2"><center>Statystyki potworów</center></th></tr><tr><th><center>Statystyka</center></th><th><center>Właściwości</center></th></tr><tr><td><center><b>Czas odrodzenia</b><center> (<code>resp</code>)<br>
</center></center></td><td>• Odpowiada za ustawienie potworowi czasu odrodzenia. <br>
• Minimalna wartość wynosi 1 godzina.<br>
• Rozrzut czasu odrodzenia NPC po ustawieniu tej statystyki wynosi 25%.</td></tr><tr><td><center><b>Atak</b> (<code>attack</code>)<center></center></center></td><td>• Odpowiada za ustawienie typu obrażeń potwora:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ ogień (<code>fire</code>) - dla profesji mag, paladyn, tropiciel.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ zimno (<code>frost, N</code>) - dla profesji mag, paladyn, tropiciel, umożliwia również ustalenie stałej wartości spowolnienia <code>N</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błyskawice (<code>light</code>) - dla profesji mag, paladyn, tropiciel.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trucizna (<code>poison,N</code>) - dla profesji wojownik, tancerz ostrzy, łowca, umożliwia również ustalenie stałej wartości spowolnienia <code>N</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ głęboka rana (<code>wound,N</code>) - dla profesji wojownik, tancerz ostrzy, łowca, umożliwia również ustalenie stałej szansy na aplikację głębokiej rany <code>N</code>.<br>
• W przypadku braku tej statystyki, typ obrażeń potwora jest domyślny:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ obrażenia fizyczne - dla profesji wojownik, tancerz ostrzy, jeżeli w definicji potwora nie ma ustawionej trucizny. Część obrażeń fizycznych zawsze posiada profesja paladyna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ obrażenia dystansowe - dla profesji łowcy, jeżeli w definicji potwora nie ma ustawionej trucizny. Część obrażeń dystansowych zawsze posiada profesja tropiciela.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ ogień - dla profesji mag, paladyn, tropiciel, jeżeli jest spełnione równanie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;lvl % 3 == 0<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ zimno - dla profesji mag, paladyn, tropiciel, jeżeli jest spełnione równanie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;lvl % 3 == 1<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błyskawice - dla profesji mag, paladyn, tropiciel, jeżeli jest spełnione równanie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;lvl % 3 == 2<br>
</td></tr><tr><td><center><b>Zwiększenie obrażeń</b> (<code>dmg_to_player_per</code>)</center><br>
</td><td>• Odpowiada za zwiększenie obrażeń od ataku oraz wszelkich umiejętności potwora.<br>
• Jest wyrażane w procentach.<br>
• Łączy się addytywnie z efektami umiejętności <code>poison_lowdmg_per-enemies, dmg_from_npc_per</code>.<br>
• Łączy się z efektem <i>Ciosu krytycznego</i> w sposób multiplikatywny.</td></tr><tr><td><center><b>Szybkość ataku</b> (<code>sa</code>)</center><br>
</td><td>• Odpowiada za zwiększenie szybkości ataku potwora.<br>
</td></tr><tr><td><center><b>Cios krytyczny</b> (<code>crit</code>)</center><br>
</td><td>• Odpowiada za zwiększenie szansy na zajście zdarzenia <i>Cios krytyczny</i>.<br>
</td></tr><tr><td><center><b>Siła ciosu krytycznego fizycznego</b> (<code>critval</code>)</center><br>
</td><td>• Odpowiada za zwiększenie siły ciosu krytycznego fizycznego.<br>
</td></tr><tr><td><center><b>Siła ciosu krytycznego magiczny</b> (<code>critmval</code>)</center><br>
</td><td>• Odpowiada za zwiększenie siły ciosu krytycznego magicznego dla wszystkich żywiołów.<br>
</td></tr><tr><td><center><b>Niszczenie pancerza</b> (<code>acdmg</code>)</center><br>
</td><td>• Odpowiada za zwiększenie niszczenia pancerza potwora.<br>
</td></tr><tr><td><center><b>Ogłuszenie</b> (<code>stun2</code>)</center><br>
</td><td>• Odpowiada za określenie szansy na zajście zdarzenia <i>Ogłuszenie</i>.<br>
• Zdarzenie jest wyzwalane podczas wykonywania ataku przez potwora.<br>
• Efekt zdarzenia prowadzi do ogłuszenia gracza na 2 tury, podczas których nie może zajść zdarzenie Bloku, Uniku, Parowania i Bloku strzały.<br>
• Obrażenia dodatkowe są losowane z zakresu obrażeń broni głównej i nie ulegają zwiększeniu ani zmniejszeniu na skutek efektów umiejętności i zdarzeń (takich jak cios krytyczny).<br>
• Pozycja początkowa postaci, która jest celem efektu, musi wynosić 1.</td></tr><tr><td><center><b>Odporności</b> (<code>res</code>)</center><br>
</td><td>• Odpowiadają za ustalenie odporności na ogień, błyskawice, zimno i truciznę potwora.<br>
</td></tr><tr><td><center><b>Życie</b> (<code>hp</code>)</center><br>
</td><td>• Odpowiada za zwiększenie puli zdrowia potwora.<br>
</td></tr><tr><td><center><b>Pancerz</b> (<code>ac</code>)</center><br>
</td><td>• Odpowiada za zwiększenie pancerza potwora.<br>
</td></tr><tr><td><center><b>Absorpcja</b> (<code>absorb</code>)</center><br>
</td><td>• Odpowiada za zwiększenie absorpcji fizycznej potwora.</td></tr><tr><td><center><b>Absorpcja magiczna</b> (<code>absorbm</code>)</center><br>
</td><td>• Odpowiada za zwiększenie absorpcji magicznej potwora.</td></tr><tr><td><center><b>Unik</b> (<code>evade</code>)</center><br>
</td><td>• Odpowiada za zwiększenie szansy na unik potwora.</td></tr><tr><td><center><b>Blok</b> (<code>block</code>)</center><br>
</td><td>• Odpowiada za zwiększenie szansy na blok potwora.</td></tr><tr><td><center><b>Redukcja spowolnień</b> (<code>redslow</code>)</center><br>
</td><td>• Odpowiada za zmniejszenie wartości spowolnień stałych nałożonych na potwora.</td></tr><tr><td><center><b>Skracanie czasu trwania ogłuszen</b> (<code>redstun</code>)</center><br>
</td><td>• Odpowiada za skrócenie czasu trwania ataku, podczas której potwór znajduje się w stanie ogłuszenia.</td></tr><tr><td><center><b>Zmniejszanie szansy na efekt zaniechania akcji</b> (<code>lowskipturn</code>)</center><br>
</td><td>• Odpowiada za zmniejszenie szansy na zajście w trakcie walki zdarzenia Klątwy oraz Oślepienia.</td></tr><tr><td><center><b>Odporność na głęboką ranę</b> (<code>woundred</code>)</center><br>
</td><td>• Odpowiada za zwiększenie odporności na głęboką ranę.</td></tr><tr><td><center><b>Szeroki zamach</b> (<code>swing</code>)</center><br>
</td><td>• Odpowiada za określenie szansy na zajście zdarzenia <i>Szeroki zamach</i>.<br>
• Zdarzenie jest wyzwalane podczas wykonywania trafionego ataku przez potwora.<br>
• Efekt zdarzenia prowadzi do zaatakowania w trakcie ataku dodatkowych dwóch celów.<br>
• Obrażenia dodatkowe są losowane z zakresu obrażeń broni głównej i nie ulegają zwiększeniu ani zmniejszeniu na skutek efektów umiejętności i zdarzeń (takich jak cios krytyczny).<br>
• Celem efektu mogą być wszystkie postacie z drużyny przeciwnej, do których zaatakowania nie jest konieczna zmiana pozycji potwora.<br>
• Efekt nie zachodzi podczas ataku będącego ciosem śmiertelnym.<br>
• Efekt może zajść na postaci dystansowej, ale wyłącznie jeżeli przeciwnicy (cel ataku wraz z postaciami sąsiadującymi) rozpoczęli walkę z pozycji pierwszej i zmienili pozycję w kierunku postaci dystansowej co najmniej raz.</td></tr><tr><td><center><b>Wściekłość</b> (<code>rage</code>)</center><br>
</td><td>• Odpowiada za wyzwolenie efektu <i>Wściekłości</i>, wraz z każdym trafionym w potwora ciosem krytycznym, na określoną liczbę tur.<br>
• Zwiększa obrażenia fizyczne o 10%.</td></tr><tr><td><center><b>Wściekłość na 3 tury</b> (<code>rage_3turns</code>)</center><br>
</td><td>• Odpowiada za wyzwolenie efektu <i>Wściekłości</i>, wraz z każdym trafionym w potwora ciosem krytycznym, na 3 tury.<br>
• Zwiększa obrażenia fizyczne o wartość określoną jako parametr statystyki.</td></tr><tr></tr><tr><td><center><b>Kontra</b> (<code>contra</code>)</center><br>
</td><td>• Odpowiada za określenie szansy na zajście zdarzenia <i>Kontra</i> po przyjęciu przez potwora ciosu krytycznego.<br>
• Zdarzenie jest wyzwalane podczas przyjmowania obrażeń przez potwora.<br>
• Efekt zdarzenia wyzwala automatyczny atak w obrębie tej samej tury potwora.</td></tr><tr><td><center><b>Parowanie</b> (<code>parry</code>)</center><br>
</td><td>• Odpowiada za określenie szansy na zajście zdarzenia <i>Parowania</i> po przyjęciu obrażeń od postaci walczącej w zwarciu.<br>
• Zdarzenie jest wyzwalane podczas przyjmowania obrażeń przez potwora.<br>
• Pozycja początkowa postaci, która wyzwala efekt u potwora, musi wynosić 1.<br>
• Efekt zdarzenia powoduje zniwelowanie przychodzących obrażeń od broni głównej lub pomocniczej na jedną turę, wprowadzając efekt <i>chybienia</i>.</td></tr><tr><td><center><b>Blok strzały</b> (<code>arrowblock</code>)</center><br>
</td><td>• Odpowiada za określenie szansy na zajście zdarzenia <i>Bloku strzały</i> po przyjęciu obrażeń od postaci walczącej w dystansie (korzystającej z broni dystansowej).<br>
• Zdarzenie jest wyzwalane podczas przyjmowania obrażeń przez potwora.<br>
• Pozycja początkowa postaci, która wyzwala efekt u potwora, musi wynosić 3.<br>
• Efekt zdarzenia powoduje zniwelowanie przychodzących obrażeń od broni głównej na jedną turę, wprowadzając efekt <i>chybienia</i>.</td></tr><tr><td><center><b>Zranienie</b> (<code>injure</code>)</center></td><td>• Określa szansę na zajście zdarzenia powodującego nałożenie na gracza efektu obrażeń rozłożonych w czasie, wyzwalających się po każdej turze przeciwnika.<br>
• Zdarzenie jest wyzwalane podczas wykonywania ataku przez potwora.<br>
• Wartość obrażeń wynosi 15% obrażeń zadanych w gracza.<br>
• Obrażenia nie kumulują się.</td></tr><tr><td><center><b>Wzrost siły potwora dla małej grupy</b><br>(<code>surpass_bonus, suprass_treshold</code>)</center><br>
</td><td>• Odpowiada za zwiększenie statystyk potwora o wartość określoną w <code>surpass_bonus</code>:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wzrostu do obrażeń - zwiększenie statystyki <code>dmg_to_player_per</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Życia - zwiększenie statystyki <code>hp</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Pancerza - zwiększenie statystyki <code>ac</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Odporności (na magię oraz na truciznę) - zwiększenie statystyki <code>res</code>.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szybkości ataku - zwiększenie szybkości ataku o procent z uwzględnieniem jedynki, która jest sumowana podczas wyliczania czasu trwania ataku. Wzrost szybkości ataku posiada górną granicę.<br>
• Wartość statystyk rośnie o część ich wartości bazowej zależną od parametru <code>surpass_treshold</code> określającego liczbę graczy, poniżej której zaczyna być naliczana kara do wzrostu siły potwora. Wzmocnienie jest obliczane zgodnie ze wzorem:<br>
<code>boost [%]= max(0, (surpass_treshold - players_amount) * surpass_bonus[%])</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>boost</code> - wzrost do statystyk potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>players_amount</code> - liczba graczy rozpoczynających walkę.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>surpass_treshold</code> - granica liczby graczy, poniżej której siła potwora zaczyna rosnąć.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>surpass_bonus</code> - część statystyk ulegająca wzmocnieniu wraz z każdym brakującym graczem.</td></tr><tr><td><center><b>Cios bardzo krytyczny</b> (<code>verycrit</code>)</center></td><td>• Odpowiada za zamianę każdego ciosu krytycznego potwora na cios bardzo krytyczny, którego siła większa o 75%.<br>
• Jest włączony w przypadku walki pojedynczo z herosem.<br>
• Heros może również wylosować Cios bardzo krytyczny podczas walki z drużyną, jeżeli różnica poziomów jest zbyt duża (co jest jednoznaczne z utratą wielu łupów na skutek zbyt dużej różnicy poziomowej między członkami drużyny - zredukowaniem liczby łupów do jednego).<br>
</td></tr><tr><td><center><b>Efekty pasywne</b> (<code>passives</code>)</center></td><td>• Wewnątrz efektów pasywnych można umieścić te same statystyki oraz efekty pasywne umiejętności, jakie może mieć postać gracza, na przykład: manę, energię, przywracanie energii co turę, bonusy legendarne, niszczenie zasobów, odporność na niszczenie pancerza, krytyczne przyspieszenie.<br>
</td></tr></tbody></table><br><br>
<br>
<h3><span class="color-blue">Umiejętności specjalne i ładowane potworów</span></h3><b>Cel umiejętności specjalnej</b><br>
Umiejętności wykonywane przez potwora mogą być używane na następujące cele:<br>
• Potwór - NPC rzuca umiejętność na samego siebie (leczenie, oczyszczenie ze spowolnień).<br>
• Atakowany gracz - NPC rzuca umiejętność na gracza, który przyjął na siebie agresję potwora.<br>
• Losowy gracz - NPC rzuca umiejętność na losowego gracza w drużynie.<br>
• Linia - NPC rzuca umiejętność w linię atakowanego gracza (wszystkie postacie występujące na tej samej pozycji).<br>
• Losowa linia - NPC rzuca umiejętność w linię, na której stoi losowo wybrany gracz (wszystkie postacie występujące na tej samej pozycji).<br>
• Wszyscy gracze - NPC rzuca umiejętność na wszystkich graczy w drużynie.<br>
<br>
Dodatkowo wszystkie umiejętności mogą również być używane wraz z domyślnym atakiem potwora. W przypadku, gdy umiejętność zadaje obrażenia, po ustawieniu ich momentu wyzwalania wraz z atakiem, są one dodawane do ataku potwora.<br>
<br>
<b>Efekty umiejętności specjalnych i ładowanych potworów</b><br>
Każda umiejętność zbudowana jest z efektów. Umiejętności specjalne z jednego efektu, a umiejętności ładowane z dowolnej liczby efektów. Poniżej zestawiono wszystkie efekty, które mogą wystąpić w umiejętnościach potwora.<br>
<br><table id="t352" style="width:750px">			
<tbody><tr><th colspan="2" style="background-color:#546dd2"><center>Efekty umiejętności potworów</center></th></tr><tr><th><center>Efekt umiejętności</center></th><th><center>Działanie</center></th></tr><tr><td><center><b>Obrażenia fizyczne</b> (<code>dmg</code>)</center></td><td>W cel wykonywane są obrażenia fizyczne.</td></tr><tr><td><center><b>Obrażenia pomocnicze</b> (<code>dmgo</code>)</center></td><td>W cel wykonywane są obrażenia pomocnicze.</td></tr><tr><td><center><b>Obrażenia dystansowe</b> (<code>dmgd</code>)</center></td><td>W cel wykonywane są obrażenia dystansowe.</td></tr><tr><td><center><b>Obrażenia od głębokiej rany</b> (<code>dmgw</code>)</center></td><td>W cel są wykonane obrażenia fizyczne, a następnie aplikowane obrażenia od głębokiej rany.</td></tr><tr><td><center><b>Obrażenia od trucizny</b> (<code>dmgp</code>)</center></td><td>W cel wykonywane są obrażenia fizyczne, a następnie aplikowane obrażenia od trucizny i idące wraz z nimi spowolnienie.</td></tr><tr><td><center><b>Obrażenia od ognia</b> (<code>dmgf</code>)</center></td><td>W cel wykonywane są obrażenia od ognia.</td></tr><tr><td><center><b>Obrażenia od zimna</b> (<code>dmgc</code>)</center></td><td>W cel wykonywane są obrażenia od zimna oraz aplikowany efekt spowolnienia z tych obrażeń.</td></tr><tr><td><center><b>Obrażenia od błyskawic</b> (<code>dmgl</code>)</center></td><td>W cel wykonywane są obrażenia od błyskawic.</td></tr><tr><td><center><b>Usunięcie spowolnień z potwora</b> (<code>removeslow</code>)</center></td><td>Usuwa wszelkie spowolnienia nałożone na NPC.</td></tr><tr><td><center><b>Uleczenie</b> (<code>heal</code>)</center></td><td>Leczy potwora o określoną wartość puli zdrowia (nie może przekroczyć puli, z którą NPC rozpoczął walkę).</td></tr><tr><td><center><b>Przebicie pancerza</b> (<code>pierce</code>)</center></td><td>Podczas ataku wykonanego przez NPC zachodzi zdarzenie przebicia pancerza.</td></tr><tr><td><center><b>Ogłuszenie</b> (<code>stun</code>)</center></td><td>Cel umiejętności zostaje ogłuszony na określoną liczbę tur.</td></tr><tr><td><center><b>Odrzut</b> (<code>pushback</code>)</center></td><td>Cel umiejętności zostaje odrzucony o określoną liczbę pozycji.</td></tr><tr><td><center><b>Tarcza słońca</b> (<code>sunshield</code>)</center></td><td>Pancerz potwora zostaje zwiększony o określoną wartość procentową na 5 tur. Z każdą turą wartość dodatkowego pancerza maleje o 20 punktów procentowych.</td></tr></tbody></table><br><br>
<br>
<b>Specjalne umiejętności (<code>spec</code>)</b><br>
• Specjalna umiejętność ma określoną szansę na wyzwolenie jednego efektu umiejętności.<br>
• Podczas walki losowane są wszystkie specjalne umiejętności. Jeżeli żadna nie zostanie wylosowana lub na określoną turę została zaplanowana umiejętność ładowana, wykonywany jest zwykły atak.<br>
<br>
<b>Umiejętności ostateczne (<code>super</code>)</b><br>
• Umiejętność ładowana wyzwala się zawsze w określonej turze i powtarza się co określoną liczbę tur.<br>
• Umiejętność ta ładuje się przez określoną liczbę tur (nazywanych turami ładującymi). Do momentu naładowania umiejętności na 100%, może zostać ona przerwana na skutek przyjęcia przez potwora efektów: <i>Ogłuszenia/Zamrożenia, Klątwy, Oślepienia, Wytrącenia z równowagi</i>. Czas ładowania może wynieść również zero tur (umiejętność od razu jest naładowana na 100%).<br>
• Może wywoływać więcej niż jeden efekt umiejętności jednocześnie.<br>
• Rozpoczęcie ładowania umiejętności ładującej się dłużej niż 0 tur, zawsze idzie w parze z wykonaniem przez NPC zwykłego ataku lub umiejętności specjalnej, który poprzedza pierwszą turę ładującą.<br>
<br>
<b>Umiejętności (<code>skills_active, skills_mastery</code>)</b><br>
• Potwory mogą posiadać umiejętności (aktywne i pasywne) zbudowane z efektów, które zostały opisane w sekcji <a href="#k36">3.6. Efekty umiejętności w walkach PvP</a>.<br>
• Potwory mogą używać tych samych umiejętności, jakie zostały utworzone dla graczy, o ile spełniają warunki i wymogi, jakie są zdefiniowane w umiejętności (poziom, profesja, typ obrażeń, pozycja postaci, mana, energia).<br>
• Potwory mogą korzystać z ukrytych przed graczami umiejętności. Nie wymagają one od potwora posiadania konkretnej profesji.<br>
• Każdy potwór może mieć zdefiniowane własne Mistrzostwo walk, czyli kolejkę wykonywanych umiejętności współdzielonych z graczami. Wystąpienie umiejętności ładowanej lub Specjalnej umiejętności w momencie gdy aktywne jest Mistrzostwo walk, powoduje opóźnienie wykonania zaplanowanej na daną turę umiejętność współdzieloną z graczami.<br>
<br>
<a name="npc_mw"></a><b>Kolejność wykonywania umiejętności potworów</b><br>
• Najwyższy priorytet ma Mistrzostwo walk. Jeżeli umiejętność została zakolejkowana na konkretną turę, zostanie ona wykonana zawsze pod warunkiem spełnienia wymogu zasobów (many i energii), pozycji i czasu odnowienia.<br>
• Umiejętności ostateczne i Specjalne umiejętności mogą być wykonane jedynie wówczas, gdy w Mistrzostwie walk występuje zwykły atak lub nie zostało one aktywowane.<br>
• Umiejętności ostateczne mają wyższy priorytet niż Specjalne umiejętności i wykonują się zawsze po przekroczeniu licznika tur Umiejętności ostatecznych. Licznik jest inicjowany wartością 1 i zwiększa się o 1 po każdej Specjalnej umiejętności lub zwykłym ataku. Do zwiększenia licznika o 1 nie dochodzi, gdy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ rozpoczynane jest ładowanie Umiejętności ostatecznej, również poprzedzająca to akcja nie jest liczona,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ następują kolejne kroki ładowania Umiejętności ostatecznej,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ dochodzi do rzucenia Umiejętności ostatecznej,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ dochodzi do użycia Umiejętności z Mistrzostwa walk.<br>
<br>
<br>
<h3><span class="color-blue">Czas odrodzenia potworów</span></h3>Każdy potwór ma natywnie określony oczekiwany czas odrodzenia oraz rozrzut względem tej wartości. <br>
Czas odrodzenia:<br>
<code>respawn_time<sub>lvl</sub> = 40 + 10.85 * min(200 , lvl) - 0.02721 * min(200 ,lvl)^2</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>respawn_time<sub>lvl</sub></code> - czas odrodzenia potwora podany w sekundach.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>lvl</code> - poziom potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min</code> - funkcja matematyczna minimum.<br>
Rozrzut dla potworów z natywnym czasem odrodzenia wynosi zawsze 10%.<br>
<br>
Czas odrodzenia można modyfikować poprzez:<br>
• Zmianę natywnego czasu odrodzenia poprzez zmianę poziomu potwora.<br>
• Ustalenie czasu odrodzenia na określonych koordynatach z rozrzutem 50%.<br>
• Statystykę <code>resp</code> z rozrzutem 25%.<br>
• Zmianę szybkości odradzania potworów w ustawieniach serwera (zmiana wartości mnożnika między 1.0 a 3.0).<br>
• Wzrost liczby graczy na serwerze, który powoduje skrócenie czasu odradzania, zgodnie ze wzorem:<br>
<code>resp_boost = min(2 , max(1 , players_amount / 500))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>resp_boost</code> - przyspieszenie czasu odradzania się potworów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>players_amount</code> - liczba graczy na serwerze.<br>
<i>Komentarz</i>: mnożniki łączą się w sposób multiplikatywny.<br>
<br>
<h3><span class="color-blue">Statystyki potwora zależne od poziomu gracza</span></h3><br><table id="t353" style="width:750px">
<tbody><tr><th colspan="6" style="background-color:#546dd2"><center>Zachowanie potwora zależne od poziomu gracza</center></th></tr><tr><th><center>Typ potwora</center></th><th><center>Ograniczona widoczność</center></th><th><center>Ograniczony atak</center></th><th><center>Cios bardzo krytyczny</center></th><th><center>Niszczenie łupu</center></th><th><center>Wiele losowań</center></th></tr><tr><td>Zwykły Potwór</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Elita</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Elita II</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-light-green">Tak</span></center></td></tr><tr><td>Elita III</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Heros</td><td><center><span class="color-light-green">Tak<br>Standardowa</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-light-green">Tak</span></center></td></tr><tr><td>Kolos</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Tytan</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-light-green">Tak</span></center></td></tr><tr><td>Elita Eventowa</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Elita III Eventowa</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Heros Eventowy</td><td><center><span class="color-light-green">Tak<br>Specjalna</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td></tr><tr><td>Kolos Eventowy</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td></tr><tr><td>Tytan Eventowy</td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-red">Nie</span></center></td><td><center><span class="color-light-green">Tak</span></center></td></tr></tbody></table><br><br>
<br>
<b>Ograniczona widoczność</b><br>
Tylko postacie posiadające poziom mieszczący się w określonych granicach mogą zobaczyć potwora z tym ograniczeniem.<br>
Ograniczona górna widoczność odnosi się do włączenia ograniczenia dla postaci przekraczających określony poziom.<br>
Ograniczona dolna widoczność odnosi się do włączenia ograniczenia, jeśli postać nie przekracza określonego poziomu.<br>
Ponadto potwór wyświetlany jest wyłącznie w odległości mniejszej niż 12 kratek od pozycji NPC (wliczając przekątne).<br>
<br>
Poziom, dla ograniczonej górnej widoczności, oblicza się zgodnie ze wzorem:<br>
<code>max_player_lvl = npc_lvl + max(13 , config)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max_player_lvl</code> - maksymalny poziom gracza, który widzi potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>npc_lvl</code> - poziom potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>config</code> - maksymalny poziom, do którego łup z potwora się nie niszczy, będący ustawieniem serwera.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja matematyczna maksimum.<br>
<br>
Poziom, dla ograniczonej dolnej widoczności, oblicza się zgodnie ze wzorem:<br>
<code>min_player_lvl = max(npc_lvl - 50 , floor(npc_lvl / 2))</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min_player_lvl</code> - minimalny poziom gracza, który widzi potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>npc_lvl</code> - poziom potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja matematyczna podłoga.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja matematyczna maksimum.<br>
<br>
Herosi eventowi nie posiadają górnej maksymalnej widoczności, a poziom minimalny dolnej widoczności herosa oblicza się zgodnie ze wzorem:<br>
<code>min_player_lvl = floor(npc_lvl / 2)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>min_player_lvl</code> - minimalny poziom gracza, który widzi potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>npc_lvl</code> - poziom potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>floor</code> - funkcja matematyczna podłoga.<br>
<br>
<b>Ograniczony atak</b><br>
Jest to ograniczenie ataku NPC, jeżeli poziom postaci przekracza maksymalny poziom, do którego łup się nie niszczy. Ograniczenie jest wyłączone w przypadku potworów z poziomem większym bądź równym 250.<br>
W przypadku, gdy w drużynie gracza znajduje się postać, która ograniczałaby atakowanie potwora, nie bierze ona udziału w walce.<br>
<br>
<b>Cios bardzo krytyczny</b><br>
Wszystkie ciosy krytyczne potwora są zamieniane w ciosy bardzo krytyczne w przypadku, gdy gracz zaatakował NPC w pojedynkę lub różnica poziomów między członkami drużyny jest zbyt duża i liczba losowań została zredukowana do jednego.<br>
<br>
<b>Niszczenie łupu</b><br>
Łup z potwora jest niszczony, jeżeli jego poziom jest niższy od 250, a poziom gracza przekracza:<br>
<code>max_player_lvl = npc_lvl + max(13 , config)</code><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gdzie:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max_player_lvl</code> - maksymalny poziom gracza, dla którego łup nie jest niszczony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>npc_lvl</code> - poziom potwora.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>config</code> - maksymalny poziom, do którego łup z potwora się nie niszczy, będący ustawieniem serwera.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<code>max</code> - funkcja matematyczna maksimum.<br>
<br>
<b>Wiele losowań</b><br>
Po zabiciu potwora, istnieje szansa na więcej niż jeden łup pod warunkiem występowania wielu graczy w drużynie. Wiele losowań zawsze zależy od różnicy poziomów między graczami w drużynie - zbyt duża różnica poziomowa zawsze powoduje zmniejszenie liczby łupów do jednego. Szczegóły zostały opisane w sekcji <a href="#k18">zdobyczy</a>.<br>
<br>
<h3><span class="color-blue">Dodatkowe cechy potworów</span></h3>Istnieją dodatkowe cechy, które mogą posiadać niektóre potwory.<br>
<br>
<b>Agresywność</b><br>
Agresywność oznacza, że potwór sam atakuje gracza, jeżeli zbliżył się do niego na odległość:<br>
• 1 kratki - jeżeli potwór jest wojownikiem, paladynem lub tancerzem ostrzy.<br>
• 2 kratek - jeżeli potwór jest magiem.<br>
• 3 kratek - jeżeli potwór jest łowcą lub tropicielem.<br>
W przypadku, gdy potwór sam atakuje gracza, decyzja o tym czy walka jest automatyczna czy turowa, zależy od zaznaczonej opcji <i>Kiedy atakuje potwór pozwalaj wybrać tryb walki</i> w ustawieniach postaci.<br>
Potwór nie atakuje gracza, gdy ten ma więcej niż 1 poziom przewagi nad nim.<br>
<br>
<b>Dialog</b><br>
Potwór może mieć ustawiony dialog, wykonujący pewne operacje przed rozpoczęciem walki. Potworów z ustawionym dialogiem nie można atakować prawym przyciskiem myszy, a w grze mogą być wyświetlane jak inne postacie niezależne. Gdy potwów z ustawionym dialogiem wywołuje walkę, jest ona rozpoczynana tak, jakby miał włączoną <b>Agresywność</b> - w konsekwencji rozpatrywana jest opcja <i>Kiedy atakuje potwór pozwalaj wybrać tryb walki</i> z ustawień postaci.<br>
<br>
<b>Losowe koordynaty</b><br>
Potwór o randze Elita II, wraz z jego obstawą, odradza się w losowych oddalonych od 4 do 10 kratek od miejsca początkowego. Potwór wraca na swoje koordynaty początkowe po przerwie o godzinie 5:25.<br>
<br>
<b>Możliwość wyszukania</b><br>
Potwory możliwe do wyszukania są lokalizowane przy użyciu Wykrywacza herosów - przedmiotu konsumpcyjnego z atrybutem <code>nloc</code>. Zlokalizowany potwór jest losowany z puli wszystkich potworów z tą cechą, które gracz może zaatakować, zobaczyć, nie niszczy z nich łupu i różnica poziomu potwora z poziomem gracza nie przekracza 13.<br>
<br>
<br><br>
<a name="k36"></a><b><h3>3.6. Efekty umiejętności w walkach PvP</h3></b><br>
<br>
<h3><span class="color-blue">Wyzwalanie i aplikowanie efektów</span></h3>Działanie&nbsp;efektów&nbsp;wewnątrz&nbsp;systemu&nbsp;umiejętności&nbsp;można&nbsp;opisać&nbsp;następującym&nbsp;schematem&nbsp;blokowym:<br>
<code><br>
+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+<br>
|&nbsp;&nbsp;&nbsp;warstwa&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;warstwa&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;warstwa&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;warstwa&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;warstwa&nbsp;&nbsp;&nbsp;|<br>
|&nbsp;&nbsp;&nbsp;warunków&nbsp;&nbsp;|&nbsp;---&gt;&nbsp;&nbsp;|&nbsp;&nbsp;inicjacji&nbsp;&nbsp;|&nbsp;---&gt;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;zdarzeń&nbsp;&nbsp;&nbsp;|&nbsp;---&gt;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;obrażeń&nbsp;&nbsp;&nbsp;|&nbsp;---&gt;&nbsp;&nbsp;|&nbsp;finalizacji&nbsp;|<br>
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|<br>
+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+-------------+<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↑&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↑&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↑&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↑&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Sprawdzanie warunków&nbsp;&nbsp;&nbsp;&nbsp;Losowanie zdarzeń&nbsp;&nbsp;&nbsp;&nbsp;Obliczanie obrażeń&nbsp;&nbsp;&nbsp;&nbsp;Obliczanie obrażeń&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;wykonania akcji&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;regularnych&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;wykonanych&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;zadanych&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
</code><br>
<br>
<br>
<b>Warstwa warunków</b> agreguje efekty, które są odpowiedzialne za sprawdzenie, czy umiejętność może zostać wykonana. Wymaga takich informacji jak profesja postaci, pozycja postaci, pozycja oraz typ gracza będącego celem umiejętności, zasoby postaci oraz jej ekwipunek. Przechodzenie przez warstwę warunku ma miejsce już w interfejsie użytkownika, w momencie kiedy gracz informowany jest odpowiednim efektem wizualnym, że nie może użyć danej umiejętności. Zaraz po warstwie warunku ma miejsce sprawdzenie warunków wykonania akcji przez gracza (postać może mieć nałożony efekt <i>oślepienia</i>, <i>klątwy</i> lub <i>wytrącenia z równowagi</i>).<br>
Przykład: Dostępna dla każdej postaci umiejętność <i>Krok do przodu</i> wymaga, żeby postać walczyła w zwarciu (jej pozycja wynosiła 1). W przypadku niespełnienia tego warunku, umiejętność nie może zostać użyta.<br>
<br>
<b>Warstwa inicjacji</b> agreguje efekty, które inicjują zachowanie umiejętności jeszcze przed rozpoczęciem obliczania zdarzeń i wartości ataku w trakcie akcji postaci. Mogą to być efekty związane z zadawaniem obrażeń po wyzwoleniu punktów kombinacji, efekty związane ze wzmacnianiem postaci na wiele tur lub efekty związane z osłabieniem przeciwnika już w ramach tej samej akcji. Wymaga informacji o stanie postaci gracza oraz postaci celu umiejętności (sojusznika lub przeciwnika).<br>
Przykład: Efekt zwiększenia szansy na cios krytyczny umiejętności <i>Krytyczne wzmocnienie</i> ma miejsce jeszcze przed obliczeniem szansy na <i>cios krytyczny</i>.<br>
<br>
<b>Warstwa zdarzeń</b> agreguje efekty, które są związane ze zdarzeniami jakie zachodzą podczas walki. Zdarzenia efektów umiejętności są obliczane po zdarzeniach regularnych (takich jak <i>cios krytyczny, przebicie pancerza</i>), które są obliczane w ścisłej kolejności (zdarzenie <i>blok przebicia</i> nie jest obliczane przed zdarzeniem <i>przebicie pancerza</i>). Najczęściej są to efekty umiejętności pasywnych. Warstwa wymaga informacji o stanie postaci gracza oraz postaci przeciwnika.<br>
Przykład: Efekt umiejętności <i>Wytrącenie z równowagi</i> jest obliczany po sprawdzeniu czy nie zaszły zdarzenia związane z chybieniem przeciwnika oraz po sprawdzeniu zajścia zdarzenia <i>ciosu krytycznego</i>.<br>
<br>
<b>Warstwa obrażeń</b> agreguje efekty nakładane na postać lub postać przeciwnika między momentem obliczenia obrażeń wykonanych przez postać, a momentem rozpoczęcia redukcji tych obrażeń. Bezpośrednio po warstwie obrażeń ma miejsce obliczanie redukcji obrażeń przez efekty odporności, pancerza itp. Wymaga informacji o stanie postaci gracza, stanie postaci przeciwnika oraz o wszystkich zdarzeniach, jakie zaszły podczas tury.<br>
Przykład: Efekt osłabienia obrażeń przeciwnika od umiejętności <i>Zatruta strzała</i> jest nakładany w przypadku trafienia przeciwnika. Jeżeli zaszło zdarzenie <i>uniku</i> podczas ciosu, efekt umiejętności nie zostanie nałożony na przeciwnika.<br>
<br>
<b>Warstwa finalizacji</b> agreguje efekty nakładane na postać lub postać przeciwnika między momentem zakończenia redukcji obrażeń (obliczeniem obrażeń zadanych), a odebraniem na skutek tych obrażeń przeciwnikowi zdrowia. Wymaga informacji o stanie postaci gracza, stanie postaci przeciwnika oraz o wszystkich zdarzeniach, jakie zaszły podczas tury.<br>
Przykład: Efekt <i>Zmiażdżenia</i> jest nakładany w przypadku, gdy obrażenia zadane są odpowiednią częścią obrażeń wykonanych, co jest obliczane dopiero po zakończeniu efektów redukcji obrażeń.<br>
<br>
<br><br>
<h3><span class="color-blue">Budowa umiejętności</span></h3>Umiejętności są zbudowane z następujących składowych:<br>
• Listy wymogów użycia umiejętności, do których zaliczamy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymóg profesji (<code>reqp</code>) - profesja postaci używającej umiejętność musi być zgodna z oznaczeniem.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymóg broni (<code>reqw</code> - broń postaci musi należeć do określonej klasy lub zestawu klas (np: miecze, błyskawice).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymóg strzał (<code>reqarrows</code>) - konieczność posiadania danej ilości strzał.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymóg pozycji (<code>melee</code>) - konieczność posiadania określonej pozycji względem przeciwnika (zwarcie lub zasięg większy niż zwarcie).<br>
• Cel umiejętności:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przeciwnik (domyślnie) - umiejętność rzucana tylko na przeciwnika.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Gracz rzucający umiejętność (<code>self</code>) - umiejętność, którą postać może użyć tylko na siebie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Sojusznik (<code>friend</code>) - umiejętność rzucana na sojusznika.<br>
• Sposób użycia:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czar (<code>spl</code>) - umiejętność aktywna, której efekty występują w sekcji umiejętności.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czar rzucany wraz z atakiem (<code>sum</code>) - umiejętność, która poza efektami występującymi w sekcji umiejętności, również wyzwala zwykły atak. Występuje zawsze w parze ze statystyką <code>spl</code>.<br>
• Zestaw nazwy wyzwalanych efektów i sposób ich zmiany wraz z liczbą rozdanych punktów w umiejętność - szczegółowo opisane w tabeli zamieszczonej poniżej. W przypadku, gdy umiejętność posiada co najmniej jeden efekt ze stanem aktywnym, może być ona użyta przez gracza w trakcie walki.<br>
• Pozycja umiejętności w module umiejętności.<br>
• Wymóg poziomowy do odblokowania umiejętności: 25, 35, 50, 80, 120, 170, 230.<br>
• Nazwa umiejętności.<br>
• Opis.<br>
• Efekt audiowizualny umiejętności występujący po jej użyciu w trakcie walki.<br>
<br>
Pod adresem <a href="https://public-api.margonem.pl/we_get/skills/">Publicznego API umiejętności</a> znajduje się zestawienie z jakich efektów zbudowane są aktualnie występujące na serwerze deweloperskim umiejętności.<br>
Szczegóły działania efektów zostały zestawione w tabeli poniżej.<br>
<br>
<br><table id="t361" style="width:750px">
<tbody><tr><th colspan="3" style="background-color:#546dd2"><center>Opis efektów umiejętności</center></th></tr><tr><th><center>Efekt</center></th><th><center>Właściwości<center></center></center></th><th><center>Stan</center></th></tr><tr><td><center><code>absagain_per</code></center></td><td>• Działanie: przywrócenie części absorpcji (fizycznej i magicznej) po trafionym ataku.<br>
• Zmienna: część przywracanej absorpcji.<br>
• Wyzwolenie: podczas warstwy obrażeń.<br>
• Postać nie może przywrócić więcej absorpcji ani absorpcji magicznej niż pula, z którą rozpoczynała walkę.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>absorb_per</code></center></td><td>• Działanie: wzmocnienie absorpcji fizycznej o część absorpcji posiadanej z przedmiotów.<br>
• Zmienna: część posiadanej absorpcji, która zostaje dodana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Dodatkowa absorpcja nie jest przyznawana, jeśli przekroczyłaby maksymalną wartość absorpcji, jaką postać może skumulować.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>absorbd</code></center></td><td>• Działanie: redukcja części obrażeń dystansowych przyjętych przez postać poprzez absorpcję fizyczną.<br>
• Zmienna: maksymalna część obrażeń dystansowych przyjętych przez postać, która ulega redukcji.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>absorbm_per</code></center></td><td>• Działanie: wzmocnienie absorpcji magicznej o część absorpcji posiadanej z przedmiotów.<br>
• Zmienna: część posiadanej absorpcji magicznej, która zostaje dodana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Dodatkowa absorpcja magiczna nie jest przyznawana, jeśli przekroczyłaby maksymalną wartość absorpcji magicznej, jaką postać może skumulować.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>ac</code></center></td><td>• Działanie: zwiększenie pancerza o stałą wartość.<br>
• Zmienna: ilość pancerza dodana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>ac_per</code></center></td><td>• Działanie: zwiększenie pancerza o część posiadanej statystyki.<br>
• Zmienna: część posiadanego pancerza, która zostaje dodana do statystyk postaci.<br>
• Wyzwolenie: w warstwie inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>ac2_per</code></center></td><td>• Działanie: zwiększenie pancerza o część posiadanej statystyki.<br>
• Zmienna: część posiadanego pancerza, która zostaje dodana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Pancerz jest przydzielany po obliczeniu i zsumowaniu wszystkich źródeł stałego pancerza z umiejętności oraz ekwipunku.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>acdmg</code></center></td><td>• Działanie: dodaje stałą wartość niszczenia pancerza.<br>
• Zmienna: liczba punktów w niszczenie pancerza, która zostaje dodana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>achpp_per</code></center></td><td>• Działanie: dodaje 1% pancerza za każdą część brakującego zdrowia.<br>
• Zmienna: część brakującego zdrowia, za którą postać otrzymuje 1% posiadanego przez nią pancerza.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>acshield_per</code></center></td><td>• Działanie: zwiększenie pancerza o stałą wartość, zależną od ilości pancerza w posiadanej tarczy.<br>
• Zmienna: część pancerza z posiadanej tarczy, o którą zostaje zwiększony pancerz postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>act</code></center></td><td>• Działanie: zwiększa odporność na truciznę o stałą wartość wyrażoną w punktach procentowych.<br>
• Zmienna: liczba punktów procentowych redukcji obrażeń od trucizny, która zostaje dodana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>actdmg</code></center></td><td>• Działanie: obniża odporność na truciznę przeciwnika po zajściu zdarzenia ciosu krytycznego.<br>
• Zmienna: liczba punktów procentowych odporności na truciznę, o którą pomniejszone zostają statystyki przeciwnika.<br>
• Wyzwolenie: warstwa obrażeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>active_absorbdest_per</code></center></td><td>• Działanie: niszczy bieżącą część absorpcji oraz absorpcji magicznej przeciwnika.<br>
• Zmienna: część bieżącej absorpcji, która ulega zniszczeniu.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt jest redukowany przez efekt umiejętności <code>redabdest_per</code>.<br>
• Niszczenie absorpcji następuje przed zmniejszeniem ataku o wszystkie formy redukcji obrażeń.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_acdmg_physical-perw</code></center></td><td>• Działanie: zwiększa niszczenie pancerza postaci o część wykonanych obrażeń.<br>
• Zmienna: część wykonanych obrażeń, która zwiększa niszczenie pancerza postaci.<br>
• Wyzwolenie: warstwa obrażeń.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_acdmg_per</code></center></td><td>• Działanie: zwiększa niszczenie pancerza postaci o posiadanego przez przeciwnika pancerza.<br>
• Zmienna: część pancerza przeciwnika, która ulega redukcji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_add_light_cumulaction</code></center></td><td>• Działanie: dodatkowo zwiększa poziom kumulacji obrażeń od błyskawic o 1.<br>
• Zmienna: liczba poziomów kumulacji o jaką zwiększa się stan obrażeń od błyskawic postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Poziom kumulacji obrażeń od błyskawic nie może przekroczyć limitu - 20 poziomów kumulacji.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_block_per</code></center></td><td>• Działanie: zwiększa szansę na blok celu.<br>
• Zmienna: liczba punktów procentowych, o którą wzrasta szansa na blok postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
• Celem umiejętności może być również sojusznik.<br>
• Szansa na blok nie może wzrosnąć powyżej 50%.<br>
• Łączy się w sposób addytywny z efektami umiejętności: <code>blok_per, decblock_per, active_decblock_per, active_decblock_per-enemies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_crit</code></center></td><td>• Działanie: zwiększa szansę na cios krytyczny postaci.<br>
• Zmienna: liczba punktów procentowych, o którą wzrasta szansa na cios krytyczny.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt umiejętności wpływa na szansę na cios krytyczny pomocniczy.<br>
• Efekt umiejętności wpływa na zajście zdarzenia cios bardzo krytyczny oraz cios bardzo krytyczny pomocniczy.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt łączy się addytywnie z efektem umiejętności <code>active_crit-allies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_crit-allies</code></center></td><td>• Działanie: zwiększa szansę na cios krytyczny wszystkich członków drużyny.<br>
• Zmienna: liczba punktów procentowych, o którą wzrasta szansa na cios krytyczny.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt umiejętności wpływa na szansę na cios krytyczny pomocniczy.<br>
• Efekt umiejętności wpływa na zajście zdarzenia cios bardzo krytyczny oraz cios bardzo krytyczny pomocniczy.<br>
• Czas trwania efektu może być większy od 1.<br>
• Postać rzucająca umiejętność otrzymuje tylko połowę wzrostu statystyki z efektu.<br>
• Efekt kumuluje się do dwóch najwyższych źródeł.<br>
• Efekt łączy się addytywnie z efektem umiejętności <code>active_crit</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_decblock_per</code></center></td><td>• Działanie: zmniejsza szansę na blok celu.<br>
• Zmienna: liczba punktów procentowych, o którą maleje szansa na blok postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
• Szansa na blok jest redukowana tylko w ramach ataku, podczas którego rzucono umiejętność. Czas trwania umiejętności zależy od tur ukończonych przez postać rzucającą efekt.<br>
• Szansa na blok nie może spaść poniżej zera.<br>
• Łączy się w sposób addytywny z efektami umiejętności: <code>blok_per, decblock_per, active_block_per, active_decblock_per-enemies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_decblock_per-enemies</code></center></td><td>• Działanie: zmniejsza szansę na wszystkich przeciwników.<br>
• Zmienna: liczba punktów procentowych, o którą maleje szansa na blok wszystkich przeciwników.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
• Czas trwania umiejętności zależy od tur przeciwników, na który nałożony jest efekt.<br>
• Szansa na blok nie może spaść poniżej zera.<br>
• Łączy się w sposób addytywny z efektami umiejętności: <code>blok_per, decblock_per, active_block_per, active_decblock_per</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_decevade_per</code></center></td><td>• Działanie: zmniejsza szansę na unik przeciwnika.<br>
• Zmienna: liczba punktów procentowych, o którą maleje szansa na unik przeciwnika.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
• Szansa na unik nie może spaść poniżej zera.<br>
• Najpierw przebiega wzrost uniku z efektu <code>evade_per</code>, następnie przyrostu z <code>adrenalin_evade_per</code>, następnie zmniejszenie o punkty stałe z <code>lowevade</code>, a na koniec zmniejszenie o punkty procentowe z efektów <code>decevade_per</code> i <code>active_decevade_per</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>active_redstun</code></center></td><td>• Działanie: zwiększa redukcję czasu trwania ogłuszenia postaci.<br>
• Zmienna: liczba punktów procentowych o jaką wzrasta redukcja czasu trwania ogłuszenia.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt umiejętności łączy się addytywnie z efektem <code>redstun</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>add_attacks</code></center></td><td>• Działanie: podczas tury wykonane zostaje więcej ataków.<br>
• Zmienna: liczba dodatkowych ataków wykonanych w trakcie tury.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Wszystkie ataki są traktowane jako jedna tura, zatem wszelkie efekty, które działają podczas tury, w której wykonywana jest umiejętność, również obejmują każdy wykonany cios.<br>
• Podczas dodatkowych ataków (innych niż ostatni) nie może dojść do zdarzeń takich jak: kontra.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>adddmg_fire-perw</code></center></td><td>• Działanie: zwiększa obrażenia od ognia o część określoną w parametrze efektu.<br>
• Zmienna: część wylosowanych podczas ataku obrażeń od ognia, o którą zwiększany jest atak.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Obrażenia łączą się addytywnie z innymi wzmocnieniami.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>adddmg_physical-perw</code></center></td><td>• Działanie: zwiększa obrażenia fizyczne o część określoną w parametrze efektu.<br>
• Zmienna: część wylosowanych podczas ataku obrażeń fizycznych, o którą zwiększany jest atak.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Obrażenia łączą się addytywnie z innymi wzmocnieniami. Efekt nie zwiększa zatem dodatkowo obrażeń spowodowanych ciosem krytycznym - jest obliczany względem obrażeń przed wzmocnieniem.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>adrenalin_evade_per</code></center></td><td>• Działanie: zwiększa szansę na unik o określoną liczbę punktów procentowych, w przypadku, gdy procentowa pula punktów zdrowia postaci jest niższa niż wartość podana jako parametr efektu <code>adrenalin_evade_threshold_per</code>.<br>
• Zmienna: liczba punktów procentowych o jaką rośnie unik postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt wyłącza się, jeżeli poziom zdrowia postaci ponownie przekroczy wartość podaną w parametrze <code>adrenalin_evade_threshold_per</code>.<br>
• Dodatkowy unik może być obniżony przez przeciwnika.<br>
• Najpierw przebiega wzrost uniku z efektu <code>evade_per</code>, następnie przyrostu z <code>adrenalin_evade_per</code>, następnie zmniejszenie o punkty stałe z <code>lowevade</code>, a na koniec zmniejszenie o punkty procentowe z efektów <code>decevade_per</code> i <code>active_decevade_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>adrenalin_evade_threshold_per</code></center></td><td>• Działanie: ustala poziom zdrowia wyrażony w procentach, poniżej którego wyzwala się efekt <code>adrenalin_evade_per</code>.<br>
• Zmienna: liczba punktów procentowych zdrowia postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>adrenalin_reddest_per_sum</code></center></td><td>• Działanie: obniża niszczenie energii i many przez przeciwnika z jego ekwipunku o określoną część, w przypadku, gdy procentowa pula punktów zdrowia postaci jest niższa niż wartość podana jako parametr efektu <code>adrenalin_reddest_threshold_per</code>.<br>
• Zmienna: część wartości o jaką maleją niszczenia energii i many wymierzone w postać.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt wyłącza się, jeżeli poziom zdrowia postaci ponownie przekroczy wartość podaną w parametrze <code>adrenalin_reddest_threshold_per</code>.<br>
• Redukcja łączy się w sposób addytywny z efektem <code>reddest_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>adrenalin_reddest_threshold_per</code></center></td><td>• Działanie: ustala poziom zdrowia wyrażony w procentach, poniżej którego wyzwala się efekt <code>adrenalin_reddest_per_sum</code>.<br>
• Zmienna: liczba punktów procentowych zdrowia postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>adrenalin_sa_per</code></center></td><td>• Działanie: zwiększa szybkość ataku postaci o pewną jej część, w przypadku, gdy procentowa pula punktów zdrowia postaci jest niższa niż wartość podana jako parametr efektu <code>adrenalin_sa_threshold_per</code>.<br>
• Zmienna: część wartości o jaką wzrasta szybkość ataku postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt wyłącza się, jeżeli poziom zdrowia postaci ponownie przekroczy wartość podaną w parametrze <code>adrenalin_sa_threshold_per</code>.<br>
• Przyspieszenie łączy się w sposób addytywny z efektami <code>critsa_per, sa_per, sa2_per, aura-sa_per, allslow_per, critslow_per, lightshield_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>adrenalin_sa_threshold_per</code></center></td><td>• Działanie: ustala poziom zdrowia wyrażony w procentach, poniżej którego wyzwala się efekt <code>adrenalin_sa_per</code>.<br>
• Zmienna: liczba punktów procentowych zdrowia postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>agi</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadaną przez postać zręczność i wynik dodaje do obrażeń minimalnych oraz maksymalnych postaci.<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń za każdy punkt zręczności.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>alllowdmg</code></center></td><td>• Działanie: zmniejsza obrażenia wszystkich postaci w drużynie przeciwnej o określoną w parametrze część.<br>
• Zmienna: część o jaką zmniejszają się obrażenia podczas ataku przeciwników.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnego gracza.<br>
• Obrażenia łączą się addytywnie z innymi wzmocnieniami oraz osłabieniami.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>allslow_per</code></center></td><td>• Działanie: zmniejsza szybkość ataku wszystkich postaci w drużynie przeciwnej o określoną w parametrze część.<br>
• Zmienna: część wartości o jaką maleje szybkość ataku postaci przeciwników.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Spowolnienie łączy się w sposób addytywny z efektami <code>critsa_per, sa_per, sa2_per, aura-sa_per, adrenalin_sa_per, critslow_per, lightshield_per</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na przeciwnika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>antidote</code></center></td><td>• Działanie: zwiększa odporność postaci na truciznę.<br>
• Zmienna: liczba punktów procentowych o jaką rośnie odporność na truciznę.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Dodatkowe punkty odporności na truciznę nie mogą zostać obniżone przez przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą lub sojusznika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>arrowrain</code></center></td><td>• Działanie: zadaje maksymalnie 9 razy obrażenia fizyczne w losowe cele. Jeżeli cel został wylosowany trzeci raz, obrażenia nie są wyzwalane.<br>
• Zmienna: liczba punktów obrażeń fizycznych.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Jeżeli cel przejmie obrażenia po raz drugi, są one zmniejszone o 33%.<br>
• Obrażenia są redukowane przez pancerz i w logu walki widnieje już wartość obniżona.<br>
• Efekt wymaga posiadania przez postać broni dystansowej.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>arrowrain_all-perw</code></center></td><td>• Działanie: zadaje maksymalnie 9 razy obrażenia w losowe cele. Jeżeli cel został wylosowany trzeci raz, obrażenia nie są wyzwalane.<br>
• Zmienna: część posiadanych przez postać średnich obrażeń, przekazana jako obrażenia pierwszego wyzwolenia ciosu.<br>
• W przypadku posiadania łuku zaklętego magią ognia, zimna lub błyskawic - obrażeniami zadawanymi jest odpowiednia magia żywiołów. W przeciwnym wypadku są to obrażenia dystansowe.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Jeżeli cel przejmie obrażenia po raz drugi, są one zmniejszone o 33%.<br>
• Obrażenia są redukowane przez pancerz oraz odporności magiczne i w logu walki widnieje już wartość obniżona.<br>
• Efekt wymaga posiadania przez postać broni dystansowej.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>aura-ac_per</code></center></td><td>• Działanie: zwiększa pancerz wszystkich członków drużyny.<br>
• Zmienna: część posiadanej przez każdego członka drużyny wartości, o którą rośnie pancerz.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń przeciwnika.<br>
• Dodatkowe punkty w pancerz nie mogą zostać obniżone przez przeciwnika.<br>
• Efek zwiększa pancerz o część początkowej wartości pancerza przed jego zredukowaniem w trakcie walki.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą oraz sojuszników i zależy od liczby wykonanych przez nich tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>aura-adddmg2_per-meele</code></center></td><td>• Działanie: zwiększa obrażenia wszystkich członków drużyny, którzy na początku walki zajmują pierwszą pozycję (od broni białej).<br>
• Zmienna: część obrażeń fizycznych, która zostaje zwiększona.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą oraz sojuszników i zależy od liczby wykonanych przez nich tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>aura-resall</code></center></td><td>• Działanie: zwiększa odporności na magię wszystkich członków drużyny.<br>
• Zmienna: liczba punktów procentowych o jaką rosną odporności na ogień, zimno oraz błyskawice.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń przeciwnika.<br>
• Dodatkowe punkty w odporność na magię nie mogą zostać obniżone przez przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą oraz sojusznika i zależy od liczby wykonanych przez nich tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>aura-sa_per</code></center></td><td>• Działanie: zwiększa szybkość ataku wszystkich postaci w drużynie o określoną w parametrze część.<br>
• Zmienna: część wartości o jaką wzrasta szybkość ataku postaci w drużynie.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Na postać rzucającą efekt, wartość przyspieszenia jest o połowę niższa.<br>
• Przyspieszenie łączy się w sposób addytywny z efektami <code>critsa_per, sa_per, sa2_per, adrenalin_sa_per, allslow_per, critslow_per, lightshield_per</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą oraz sojusznika i zależy od liczby wykonanych przez nich tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>bandage_per</code></center></td><td>• Działanie: przywraca część puli punktów zdrowia postaci.<br>
• Zmienna: część puli punktów zdrowia, jaka ulega przywróceniu.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt leczenia może zostać zredukowany przez efekt <code>lowheal_per-enemies</code>.<br>
• Każde kolejne użycie umiejętności z tym efektem, zmniejsza część przywracanego zdrowia o 25% wartości bazowej.<br>
• Efekt nie może przywrócić więcej punktów życia niż poziom zdrowia posiadany przez postać na początku walki.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>blok_per</code></center></td><td>• Działanie: zwiększa szansę na blok postaci.<br>
• Zmienna: liczba punktów procentowych szansy na blok, dodawana do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>combo_dmg_hpp-target</code></center></td><td>• Działanie: zadaje obrażenia od umiejętności zależne od puli zdrowia przeciwnika oraz od liczby skumulowanych punktów kombinacji. Zostaje użyta liczba skumulowanych punktów kombinacji o liczbie ustalonej w parametrze <code>combo-max</code>.<br>
• Zmienna: część zdrowia przeciwnika, która zostaje odebrana z obrażeń od umiejętności.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Obrażenia są redukowane przez efekty <code>dmg_from_player_per</code> oraz <code>poison_lowdmg_per-enemies</code>.<br>
• Obrażenia działają tylko na graczy. Potwory nie otrzymują obrażeń.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>combo_energyrestore_per</code></center></td><td>• Działanie: przywraca część posiadanej przez postać energii w zależności od liczby skumulowanych punktów kombinacji. Zostaje użyta liczba skumulowanych punktów kombinacji o liczbie ustalonej w parametrze <code>combo-max</code>.<br>
• Zmienna: część przywracanej przez postać energii.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Zwrócona energia nie może przekroczyć liczby punktów, z którą postać rozpoczynała walkę.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>combo_heal_per</code></center></td><td>• Działanie: przywraca część puli zdrowia postaci w zależności od liczby skumulowanych punktów kombinacji. Zostaje użyta liczba skumulowanych punktów kombinacji o liczbie ustalonej w parametrze <code>combo-max</code>.<br>
• Zmienna: część przywracanej puli punktów zdrowia postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Zwrócone punkty życia nie mogą przekroczyć poziomu zdrowia, z którym postać rozpoczynała walkę.<br>
• Leczenie może być zredukowane przez efekt <code>lowheal_per-enemies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>combo_lowdmg_enemy</code></center></td><td>• Działanie: zmniejsza obrażenia przeciwnika w zależności od liczby skumulowanych punktów kombinacji. Zostaje użyta liczba skumulowanych punktów kombinacji o liczbie ustalonej w parametrze <code>combo-max</code>.<br>
• Zmienna: część redukowanych obrażeń wykonanych przez przeciwnika.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł spośród efektów: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code>.<br>
• Efekt łączy się w sposób addytywny z pozostałymi efektami: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code><br>
• Wzmocnienie łączy się w sposób multiplikatywny z innymi modyfikatorami obrażeń (również z przyrostem obrażeń na skutek ciosu krytycznego).<br>
• Obrażenia widoczne w logu walki są już pomniejszone przez ten efekt.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>combo_perdmg</code></center></td><td>• Działanie: zwiększa obrażenia od ataku o zadaną w parametrze część zależnie od liczby skumulowanych punktów kombinacji. Zostaje użyta liczba skumulowanych punktów kombinacji o liczbie ustalonej w parametrze <code>combo-max</code>.<br>
• Zmienna: część o jaką są zwiększane obrażenia od ataku.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Wzmocnienie łączy się multiplikatywnie z innymi wzmocnieniami lub osłabieniami do obrażeń (również ciosem krytycznym).<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>combo-block</code></center></td><td>• Działanie: generuje punkty kombinacji za każde zdarzenie bloku, które zaszło podczas przyjmowania przez postać obrażeń od ataku.<br>
• Zmienna: liczba punktów kombinacji generowanych podczas zdarzenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>combo-crit</code></center></td><td>• Działanie: generuje punkty kombinacji za każde zdarzenie ciosu krytycznego lub ciosu krytycznego pomocniczego, które zaszło podczas wykonywania przez postać ataku.<br>
• Zmienna: liczba punktów kombinacji generowanych podczas zdarzenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Podczas zajścia obu zdarzeń w ramach jednej tury (cios krytyczny oraz cios krytyczny pomocniczy), generowanych jest dwa razy więcej punktów kombinacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>combo-evade</code></center></td><td>• Działanie: generuje punkty kombinacji za każde zdarzenie uniku, które zaszło podczas przyjmowania przez postać obrażeń od ataku.<br>
• Zmienna: liczba punktów kombinacji generowanych podczas zdarzenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>combo-max</code></center></td><td>• Działanie: określa maksymalną liczbę punktów kombinacji, jakie skumulować może dana umiejętność oraz liczbę punktów kombinacji jakie są odbierane postaci podczas wyzwolenia tego efektu poprzez użycie umiejętności.<br>
• Zmienna: maksymalna liczba możliwych do skumulowania punktów kombinacji.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>combo-pierce</code></center></td><td>• Działanie: generuje punkty kombinacji za każde zdarzenie przebicia pancerza, które zaszło podczas wykonywania przez postać ataku.<br>
• Zmienna: liczba punktów kombinacji generowanych podczas zdarzenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>combo-skill</code></center></td><td>• Działanie: generuje punkty kombinacji za każde użycie umiejętności z tym efektem.<br>
• Zmienna: liczba punktów kombinacji generowanych podczas użycia umiejętności.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>combo-wound</code></center></td><td>• Działanie: generuje punkty kombinacji za każde zdarzenie głębokiej rany lub głębokiej rany pomocniczej, które zaszło podczas wykonywania przez postać ataku.<br>
• Zmienna: liczba punktów kombinacji generowanych podczas zdarzenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Podczas zajścia obu zdarzeń w ramach jednej tury (głęboka rana oraz głęboka rana pomocnicza), generowanych jest dwa razy więcej punktów kombinacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>contra</code></center></td><td>• Działanie: zwiększa szansę na zajście zdarzenia kontry.<br>
• Zmienna: liczba punktów procentowych o jakie rośnie szansa na kontrę w statystykach postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Zdarzenie kontry może zajść wyłącznie podczas przyjęcia przez postać ciosu krytycznego lub ciosu krytycznego pomocniczego.<br>
• Efekt kontry polega na wykonaniu automatycznego ataku w przeciwnika, podczas którego czas trwania ataku wynosi zero.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center>cooldown</center></td><td>• Działanie: określa czas odnowienia umiejętności liczony w turach.<br>
• Zmienna: liczba tur, po których można ponownie użyć umiejętności.<br>
• Wyzwolenie: warstwa warunków.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>crit</code></center></td><td>• Działanie: zwiększa szansę na cios krytyczny postaci (oraz cios krytyczny pomocniczy jeżeli postać wyekwipuje przedmiot o klasie <i>pomocnicze</i>).<br>
• Zmienna: liczba punktów procentowych o jakie rośnie szansa na cios krytyczny w statystykach postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critmval_c</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego magicznego dla żywiołu zimna w statystykach postaci.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego magicznego dla żywiołu zimna.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critmval_f</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego magicznego dla żywiołu ognia w statystykach postaci.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego magicznego dla żywiołu ognia.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critmval_l</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego magicznego dla żywiołu błyskawic w statystykach postaci.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego magicznego dla żywiołu błyskawic.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critmval-allies</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego magicznego dla wszystkich członków drużyny.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego magicznego.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Łączy się addytywnie z efektem <code>critmval-enemies</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą oraz sojusznika i zależy od liczby wykonanych przez nich tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>critmval-enemies</code></center></td><td>• Działanie: zmniejsza siłę ciosu krytycznego magicznego dla wszystkich członków przeciwnej drużyny.<br>
• Zmienna: liczba obniżanych punktów w siłę ciosu krytycznego magicznego.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Łączy się addytywnie z efektem <code>critmval-allies</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na przeciwnika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>critpierce_per</code></center></td><td>• Działanie: w przypadku zajścia zarówno ciosu krytycznego jak i przebicia pancerza podczas tury, posiadane przez postać niszczenie pancerza zostaje zwiększone o jego część na 1 turę.<br>
• Zmienna: część o jaką wzrasta niszczenie pancerza postaci.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Łączy się addytywnie z efektem <code>redacdmg_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critpoison_per</code></center></td><td>• Działanie: w przypadku zajścia zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, istnieje 25% na zajście zdarzenia, podczas którego leczenie pochodzące z ekwipunku atakowanego gracza, zostaje zredukowane na 1 najbliższą turę przeciwnika.<br>
• Zmienna: część leczenia, która zostaje obniżona po zajściu zdarzenia.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Zdarzenie zachodzi wyłącznie podczas wykonywania celnego ataku przez posiadacza efektu.<br>
• Efekt zmniejszenia leczenia dotyczy następnego wyzwolenia leczenia przez przeciwnika, które zawsze następuje przed turą postaci.<br>
• Efekt nie ulega kumulacji.<br>
• Zdarzenie redukcji leczenia nie jest losowane podwójnie w przypadku zajścia w trakcie jednej tury zarówno zdarzenie ciosu krytycznego i ciosu krytycznego pomocniczego.<br>
• Łączy się addytywnie z efektami <code>heal_per-allies, heal1_per, heal_per-enemies</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critrage_perw</code></center></td><td>• Działanie: w przypadku, gdy poziom zdrowia postaci spadnie poniżej 25%<br>
• Zmienna: część leczenia, która zostaje obniżona po zajściu zdarzenia.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Zdarzenie redukcji leczenia nie jest losowane podwójnie w przypadku zajścia w trakcie jednej tury zarówno zdarzenie ciosu krytycznego i ciosu krytycznego pomocniczego.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critsa_per</code></center></td><td>• Działanie: w przypadku zajścia zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, istnieje 25% na zajście zdarzenia (Krytyczne przyspieszenie), podczas którego szybkość ataku postaci zostaje zwiększona na 3 tury.<br>
• Zmienna: część szybkości ataku, o którą zostaje przyspieszona postać.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Zdarzenie krytycznego przyspieszenia nie jest losowane podwójnie w przypadku zajścia w trakcie jednej tury zarówno zdarzenie ciosu krytycznego i ciosu krytycznego pomocniczego.<br>
• Przyspieszenie nie ulega kumulacji.<br>
• Przyspieszenie łączy się w sposób addytywny z efektami <code>aura-sa_per, sa_per, sa2_per, adrenalin_sa_per, allslow_per, critslow_per, lightshield_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critslow_per</code></center></td><td>• Działanie: w przypadku zajścia zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, przeciwnik zostaje spowolniony o pewną część jego szybkości ataku na 1 turę.<br>
• Zmienna: część szybkości ataku przeciwnika, o którą zostaje spowolniona jego postać.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Spowolnienie nie ulega kumulacji.<br>
• Przyspieszenie łączy się w sposób addytywny z efektami <code>aura-sa_per, sa_per, sa2_per, adrenalin_sa_per, allslow_per, critslow_per, lightshield_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critval</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego fizycznego w statystykach postaci.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego fizycznego.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>critval-allies</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego fizycznego oraz siły ciosu krytycznego pomocniczego (w przypadku wyekwipowanej broni pomocniczej) dla wszystkich członków drużyny.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego fizycznego.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Łączy się addytywnie z efektem <code>critval-enemies</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na postać rzucającą oraz sojusznika i zależy od liczby wykonanych przez nich tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>critval-enemies</code></center></td><td>• Działanie: zmniejsza siłę ciosu krytycznego fizycznego oraz siły ciosu krytycznego pomocniczego (w przypadku wyekwipowanej broni pomocniczej) dla wszystkich członków przeciwnej drużyny.<br>
• Zmienna: liczba obniżanych punktów w siłę ciosu krytycznego fizycznego.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Łączy się addytywnie z efektem <code>critval-allies</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na przeciwnika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>critwound</code></center></td><td>• Działanie: w przypadku zajścia zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, których wartość obrażeń zadanych w gracza jest większa od zera, istnieje szansa na zajście zdarzenia (Ciężka rana), podczas którego aplikowane są na cel obrażenia od głębokiej rany (jako osobna instancja wyniszczeń) o wartości 10% obrażeń zadanych na 3 tury.<br>
• Zmienna: szansa na zajście zdarzenia ciężkiej rany po zajściu zdarzenia ciosu krytycznego.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Zdarzenie może wystąpić tylko podczas trafionego ataku w przeciwnika.<br>
• Typ obrażeń to głęboka rana i są one redukowane przez efekt <code>woundred</code>.<br>
• Efekt obrażeń nie kumuluje się.<br>
• Efekt obrażeń nadpisuje się najświeższą nałożoną na danego przeciwnika wartością.<br>
• Obliczanie wartości obrażeń następuje przed ich wyzerowaniem przez efekt <code>immunity_to_dmg</code>, a zatem są wciąż aplikowane na przeciwnika.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>crush_dmg_per</code></center></td><td>• Działanie: zadaje dodatkowe obrażenia fizyczne o wartości części obrażeń zadanych w przeciwnika, w przypadku, gdy stosunek obrażeń zadanych do obrażeń wykonanych jest większy niż procentowa wartość podana jako parametr efektu <code>crush_threshold_per</code>.<br>
• Zmienna: część obrażeń zadanych, która zostaje ponownie wykonana w przeciwnika.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt wyłącza się, jeżeli poziom zdrowia postaci ponownie przekroczy wartość podaną w parametrze <code>crush_threshold_per</code>.<br>
• Dodatkowe obrażenia są redukowane przez efekty <code>lowdmg_enemy</code> oraz <code>poison_lowdmg_per-enemies</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>crush_threshold_per</code></center></td><td>• Działanie: ustala stosunek obrażeń zadanych do obrażeń wykonanych, powyżej którego wyzwala się efekt <code>crush_dmg_per</code>.<br>
• Zmienna: liczba punktów procentowych określających stosunek obrażeń zadanych do wykonanych.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>decblock_per</code></center></td><td>• Działanie: zwiększa wartość atrybutu obniżającego blok postaci przeciwnika.<br>
• Zmienna: liczba punktów procentowych obniżania bloku przeciwnika dodawanych do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Szansa na blok nie może spaść poniżej zera.<br>
• Obniżanie bloku obliczane jest w momencie sumowania wszystkich efektów manipulujących blokiem, również tych, których źródłem są przedmioty.<br>
• Łączy się w sposób addytywny z efektami umiejętności: <code>blok_per, decblock_per, active_block_per, active_decblock_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>decevade_per</code></center></td><td>• Działanie: zwiększa wartość atrybutu obniżającego unik postaci przeciwnika.<br>
• Zmienna: liczba punktów procentowych obniżania uniku przeciwnika dodawanych do statystyk postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Szansa na unik nie może spaść poniżej zera.<br>
• Najpierw przebiega wzrost uniku z efektu <code>evade_per</code>, następnie przyrostu z <code>adrenalin_evade_per</code>, następnie zmniejszenie o punkty stałe z <code>lowevade</code>, a na koniec zmniejszenie o punkty procentowe z efektów <code>decevade_per</code> i <code>active_decevade_per</code>.<br>
</td><td><center>pasywny</center><br>
<br>
</td></tr><tr><td><center><code>distract</code></center></td><td>• Działanie: w przypadku zajścia zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, istnieje szansa na zajście zdarzenia (Wytrącenie z równowagi), podczas którego na przeciwnika zostaje nałożony efekt zaniechania następnej wykonanej przez niego tury.<br>
• Zmienna: szansa na zajście zdarzenia Wytrącenia z równowagi po zajściu zdarzenia Ciosu krytycznego.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Efekt może zostać nadpisany przez zdarzenie Klątwy lub Oślepienia do momentu wykonania tury przez gracza, na którego został nałożony.<br>
• Zdarzenie wystąpić może wyłącznie podczas trafionego ataku w przeciwnika.<br>
• Zdarzenie jest jawne, w logu walki przeciwnik zostaje o nim powiadomiony.<br>
• Podczas wyzwolenia efektu zaniechania wykonania tury przez przeciwnika, jego akcja zostaje przerwana.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>disturb</code></center></td><td>• Działanie: w przypadku wykonania ataku, na przeciwnika zostaje nałożony efekt obniżający jego szansę na cios krytyczny, cios krytyczny pomocniczy oraz przebicie pancerza.<br>
• Zmienna: liczba punktów procentowych obniżających szansę na cios krytyczny przeciwnika oraz przebicie pancerza. Przebicie pancerza zostaje obniżone przez podwojoną wartość parametru umiejętności.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
• Zdarzenie nie wymaga trafienia ataku w przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt nie wpływa na szansę zajścia zdarzenia ciosu bardzo krytycznego oraz ciosu bardzo krytycznego pomocniczego.<br>
• Efekt łączy się w sposób addytywny z efektami <code>active_crit, active_crit-allies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>disturb_crit</code></center></td><td>• Działanie: w przypadku wykonania ataku, na przeciwnika zostaje nałożony efekt obniżający jego szansę na cios krytyczny oraz cios krytyczny pomocniczy.<br>
• Zmienna: liczba punktów procentowych obniżających szansę na cios krytyczny przeciwnika.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
• Zdarzenie nie wymaga trafienia ataku w przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt nie wpływa na szansę zajścia zdarzenia ciosu bardzo krytycznego oraz ciosu bardzo krytycznego pomocniczego.<br>
• Efekt łączy się w sposób addytywny z efektami <code>active_crit, active_crit-allies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>disturb_pierce</code></center></td><td>• Działanie: w przypadku wykonania ataku, na przeciwnika zostaje nałożony efekt obniżający jego szansę na przebicie pancerza.<br>
• Zmienna: liczba punktów procentowych obniżających szansę na przebicie pancerza.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
• Zdarzenie nie wymaga trafienia ataku w przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_evade_hpp-target_light</code></center></td><td>• Działanie: w przypadku trafionego ataku, na przeciwnika zostają nałożone obrażenia od błyskawic rozłożone w czasie o wartości części jego puli zdrowia.<br>
• Zmienna: część puli zdrowia przeciwnika, która determinuje obrażenia rozłożone w czasie.<br>
• Aplikacja: warstwa obrażeń.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Obrażenia są redukowane przez odporność na błyskawice.<br>
• Czas trwania efektu może być większy od 1.<br>
• Obrażenia działają tylko na graczy. Potwory nie otrzymują obrażeń.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_evade-target_fire-perw</code></center></td><td>• Działanie: w przypadku trafionego ataku, na przeciwnika zostają nałożone obrażenia od ognia rozłożone w czasie o wartości części posiadanych przez postać obrażeń od ognia.<br>
• Zmienna: część posiadanych przez postać obrażeń od ognia, które są wyzwalane jako obrażenia rozłożone w czasie.<br>
• Aplikacja: warstwa obrażeń.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Obrażenia są redukowane przez odporność na ogień.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_from_npc_per</code></center></td><td>• Działanie: potwory zadają mniejsze obrażenia postaci posiadającej umiejętność z tym efektem.<br>
• Zmienna: liczba punktów procentowych, o którą są redukowane obrażenia od potworów.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Efekt zmniejsza wszelkie obrażenia - również obrażenia od umiejętności specjalnych i ładowanych potworów.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>dmg_from_player_per</code></center></td><td>• Działanie: gracze zadają mniejsze obrażenia postaci posiadającej umiejętność z tym efektem.<br>
• Zmienna: liczba punktów procentowych, o którą są redukowane obrażenia od graczy.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Efekt zmniejsza wszelkie obrażenia - również obrażenia od umiejętności graczy i efekty rozłożone w czasie.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł spośród efektów: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code>.<br>
• Efekt łączy się w sposób addytywny z pozostałymi efektami: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code><br>
• Wzmocnienie łączy się w sposób multiplikatywny z innymi modyfikatorami obrażeń (również z przyrostem obrażeń na skutek ciosu krytycznego).<br>
• Obrażenia widoczne w logu walki są już pomniejszone przez ten efekt.<br>
• Efekt łączy się w sposób multiplikatywny z redukcją przez odporności efektów rozłożonych w czasie.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>dmg_hpp-row_fire</code></center></td><td>• Działanie: zadaje obrażenia od ognia wszystkim postaciom znajdującym się w jednej linii (ta sama pozycja bieżąca) o wartości części posiadanego przez nich zdrowia.<br>
• Zmienna: część puli zdrowia, która determinuje obrażenia od ognia.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Obrażenia mogą być zadane również w postać rzucającą umiejętność oraz w sojuszników o ile postacie znajdują się na tej samej pozycji.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_hpp-target</code></center></td><td>• Działanie: zadaje obrażenia fizyczne rozłożone w czasie o wartości części puli zdrowia przeciwnika.<br>
• Zmienna: część puli zdrowia, która determinuje obrażenia fizyczne.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt nie wymaga trafionego ataku w przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_hpp-target_frost</code></center></td><td>• Działanie: zadane obrażenia od zimna rozłożone w czasie o wartości części puli zdrowia przeciwnika.<br>
• Zmienna: część puli zdrowia, która determinuje obrażenia od zimna.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt nie wymaga trafionego ataku w przeciwnika.<br>
• Obrażenia są redukowane przez odporność na zimno.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_hpp-target_fire</code></center></td><td>• Działanie: zadane obrażenia od ognia rozłożone w czasie o wartości części puli zdrowia przeciwnika.<br>
• Zmienna: część puli zdrowia, która determinuje obrażenia od ognia.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt nie wymaga trafionego ataku w przeciwnika.<br>
• Obrażenia są redukowane przez odporność na ogień.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_hpp-target_light</code></center></td><td>• Działanie: zadane obrażenia od błyskawic rozłożone w czasie o wartości części puli zdrowia przeciwnika.<br>
• Zmienna: część puli zdrowia, która determinuje obrażenia od błyskawic.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt nie wymaga trafionego ataku w przeciwnika.<br>
• Obrażenia są redukowane przez odporność na błyskawice.<br>
• Czas trwania efektu może być większy od 1.<br>
• Obrażenia działają tylko na graczy. Potwory nie otrzymują obrażeń.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg_to_npc_per</code></center></td><td>• Działanie: postać zadaje większe obrażenia w potwory.<br>
• Zmienna: liczba punktów procentowych, o którą wzrastają obrażenia zadawane potworom.<br>
• Wyzwolenie: warstwa obrażeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>dmg_to_player_per</code></center></td><td>• Działanie: postać zadaje większe obrażenia w postacie graczy.<br>
• Zmienna: liczba punktów procentowych, o którą wzrastają obrażenia zadawane w postacie graczy.<br>
• Wyzwolenie: warstwa obrażeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>dmg-force-4_light-perw</code></center></td><td>• Działanie: zadaje obrażenia od błyskawic w cel oraz w losowe trzy, niepowtarzające się postacie, o wartości części posiadanego przez postać bieżącego ataku od błyskawic.<br>
• Zmienna: część ataku od błyskawic, która determinuje obrażenia umiejętności.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>aktywny</center><br>
<br>
</td></tr><tr><td><center><code>dmg-row_fire-perw</code></center></td><td>• Działanie: zadaje obrażenia od ognia wszystkim postaciom znajdującym się w jednej linii (ta sama pozycja bieżąca) o wartości części posiadanego przez postać ataku od ognia.<br>
• Zmienna: część ataku od ognia, który determinuje obrażenia umiejętności.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Obrażenia mogą być zadane również w postać rzucającą umiejętność oraz w sojuszników o ile postacie znajdują się na tej samej pozycji.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg-swing_physical-perw</code></center></td><td>• Działanie: zadaje obrażenia od umiejętności, o wartości części posiadanych obrażeń, maksymalnie trzem losowym i niepowtarzającym się postaciom innym niż cel umiejętności, które postać gracza może obrać za cel ataku bez konieczności zmiany pozycji.<br>
• Zmienna: część posiadanych obrażeń, które determinują obrażenia umiejętności.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg-target_fire-perw</code></center></td><td>• Działanie: na przeciwnika zostają nałożone obrażenia od błyskawic rozłożone w czasie o wartości części posiadanych przez postać obrażeń od ognia.<br>
• Zmienna: część posiadanych przez postać obrażeń od ognia, które są wyzwalane jako obrażenia rozłożone w czasie.<br>
• Aplikacja: warstwa obrażeń.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Obrażenia są redukowane przez odporność na ogień.<br>
• Efekt nie wymaga trafionego ataku.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>dmg-target_physical</code></center></td><td>• Działanie: na przeciwnika zostają nałożone obrażenia od umiejętności o stałej wartości.<br>
• Zmienna: liczba punktów obrażeń zadanych w przeciwnika.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>doublecastcost_per</code></center></td><td>• Działanie: użycie umiejętności z tym efektem sprawi, że koszt (energii lub many) kolejnego użycia tej umiejętności w następnej turze będzie większe o część podaną w parametrze.<br>
• Zmienna: część kosztu umiejętności o jaką rośnie wymóg zasobu i jego zużycie w następnej turze.<br>
• Wyzwolenie: warstwa wymagań.<br>
• Efekt wyłącza się, jeżeli w następnej turze zostanie użyta inna umiejętność.<br>
• Umiejętność nie może zostać użyta, jeżeli bieżąca liczba punktów energii lub many gracza nie jest większa bądź równa wymaganej liczbie zasobów powiększonej na skutek tego efektu umiejętności.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>energy</code></center></td><td>• Działanie: określenie kosztu umiejętności w postaci wymaganych punktów energii, które postać traci po użyciu umiejętności.<br>
• Zmienna: liczba punktów energii wymagana do użycia umiejętności, którą gracz traci po jej użyciu.<br>
• Wyzwolenie: warstwa wymagań.<br>
• Umiejętność nie może zostać użyta, jeżeli bieżąca energia postaci jest mniejsza niż parametr efektu.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>energybon</code></center></td><td>• Działanie: zwiększa pulę energii postaci o liczbę punktów określoną w parametrze.<br>
• Zmienna: liczba punktów energii o jaką rośnie pula energii postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>energygain</code></center></td><td>• Działanie: przywraca liczbę punktów energii po zakończeniu tury postaci.<br>
• Zmienna: liczba przywracanych punktów energii.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Liczba przywróconej energii nie może przekroczyć puli energii, z którą postać rozpoczynała walkę.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>energyout</code></center></td><td>• Działanie: zmniejsza energię przeciwnika o stałą wartość wraz z każdą turą.<br>
• Zmienna: liczba odejmowanych przeciwnikowi punktów energii.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>energyrestore_per</code></center></td><td>• Działanie: przywraca część posiadanej puli punktów energii.<br>
• Zmienna: część przywracanej puli punktów energii.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Liczba przywróconej energii nie może przekroczyć puli energii, z którą postać rozpoczynała walkę.<br>
• Wartość przywróconych zasobów podczas kolejnych użyć umiejętności z tym efektem jest o 10% niższa od wartości początkowej.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>engback</code></center></td><td>• Działanie: w przypadku zajścia zdarzenia ciosu krytycznego lub ciosu krytycznego pomocniczego, przywraca postaci część posiadanej puli punktów energii.<br>
• Zmienna: część przywracanej puli punktów energii w przypadku zajścia zdarzenia ciosu krytycznego.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Liczba przywróconej energii nie może przekroczyć puli energii, z którą postać rozpoczynała walkę.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>en-regen</code></center></td><td>• Działanie: zwiększa liczbę przywracanych punktów energii postaci z każdą wykonaną turą.<br>
• Zmienna: liczba punktów energii o jaką wzrasta przywracanie z każdą turą wykonaną przez postać.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Czas trwania efektu umiejętności jest zależny od liczby tur postaci, na którą została nałożona.<br>
• Czas trwania efektu może być większy od 1.<br>
• Liczba przywróconej energii nie może przekroczyć puli energii, z którą postać rozpoczynała walkę.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>evade_per</code></center></td><td>• Działanie: zwiększa szansę na unik o liczbę punktów procentowych zadaną jako parametr.<br>
• Zmienna: liczba punktów procentowych o jaką jest zwiększana szansa na unik postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Najpierw przebiega wzrost uniku z efektu <code>evade_per</code>, następnie przyrostu z <code>adrenalin_evade_per</code>, następnie zmniejszenie o punkty stałe z <code>lowevade</code>, a na koniec zmniejszenie o punkty procentowe z efektów <code>decevade_per</code> i <code>active_decevade_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>fastarrow</code></center></td><td>• Działanie: ustala szansę na zajście zdarzenia (Szybka strzała), podczas którego czas trwania ataku zostaje skrócony o 75% po uwzględnieniu wszystkich modyfikatorów szybkości ataku.<br>
• Zmienna: szansa na zajście zdarzenia szybkiej strzały.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Łączy się multiplikatywnie z innymi efektami skrócenia czasu trwania ataku.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>firebon</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadany przez postać intelekt i wynik dodaje do średnich obrażeń od ognia postaci (wartość ta bierze udział w obliczaniu rozrzutu).<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń za każdy punkt intelektu.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>freeze</code></center></td><td>• Działanie: wprowadza szansę na zajście zdarzenia (Zamrożenie), które ogłusza przeciwnika wprowadzając efekt zablokowania tury przeciwnika. Podczas zablokowanej tury, gracz nie może wykonać żadnej akcji.<br>
• Zmienna: liczba punktów procentowych określająca szansę na zajście zdarzenia zamrożenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Wymaga posiadania obrażeń od magii zimna.<br>
• Efekt działa analogicznie do efektu ogłuszenia (<code>stun</code>).<br>
• Zdarzenie zamrożenia może zajść wyłącznie podczas trafionego ataku, podczas którego nie zaszło zdarzenie bloku.<br>
• Podczas atakowania zamrożonego przeciwnika, nie mogą zajść zdarzenia bloku, uniku, parowania, bloku strzały, kontry.<br>
• Czas trwania zamrożenia jest redukowany przez efekt <code>redstun</code>.<br>
</td><td><center>aktywny</center><br>
<br>
</td></tr><tr><td><center><code>frostbon</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadany przez postać intelekt i wynik dodaje do obrażeń od zimna postaci.<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń za każdy punkt intelektu.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>heal_per</code></center></td><td>• Działanie: przywraca część puli punktów zdrowia postaci.<br>
• Zmienna: część puli punktów zdrowia, jaka ulega przywróceniu.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt leczenia może zostać zredukowany przez efekt lowheal_per-enemies.<br>
• Każde kolejne użycie umiejętności z tym efektem, zmniejsza część przywracanego zdrowia o 25% wartości bazowej.<br>
• Efekt nie może przywrócić więcej punktów życia niż poziom zdrowia posiadany przez postać na początku walki.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>heal_per-allies</code></center></td><td>• Działanie: zwiększa wartość leczenia z ekwipunków wszystkich członków drużyny o część zadaną jako parametr efektu.<br>
• Zmienna: część leczenia z ekwipunku postaci, o jaką rośnie przywracanie zdrowia z każdą turą.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Łączy się addytywnie z efektami <code>heal1_per, critpoison_per, heal_per-enemies</code>.<br>
• Efekt działa do końca trwania walki.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>heal_per-enemies</code></center></td><td>• Działanie: zmniejsza wartość leczenia z ekwipunków wszystkich członków drużyny przeciwnej o część zadaną jako parametr efektu.<br>
• Zmienna: część leczenia z ekwipunku postaci przeciwnika, o jaką maleje przywracanie zdrowia z każdą turą.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Łączy się addytywnie z efektami <code>heal1_per, heal_per-allies, critpoison_per</code>.<br>
• Efekt działa do końca trwania walki.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>heal1_per</code></center></td><td>• Działanie: zwiększa wartość leczenia z ekwipunku postaci o część zadaną jako parametr efektu.<br>
• Zmienna: część leczenia z ekwipunku postaci, o jaką rośnie przywracanie zdrowia z każdą turą.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Łączy się addytywnie z efektami <code>heal_per-allies, critpoison_per, heal_per-enemies</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>healall_per</code></center></td><td>• Działanie: przywraca część puli punktów zdrowia wszystkich postaci w drużynie.<br>
• Zmienna: część puli punktów zdrowia, jaka ulega przywróceniu.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt umiejętności jest o połowę słabszy, jeżeli postać nie posiada w walce żadnych sojuszników.<br>
• Efekt leczenia może zostać zredukowany przez efekt lowheal_per-enemies.<br>
• Każde kolejne użycie umiejętności z tym efektem, zmniejsza część przywracanego zdrowia o 25% wartości bazowej.<br>
• Efekt nie może przywrócić więcej punktów życia niż poziom zdrowia posiadany przez postać na początku walki.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>healpower</code></center></td><td>• Działanie: zwiększa leczenie pochodzące z przedmiotów konsumpcyjnych podczas rozgrywki swobodnej.<br>
• Zmienna: część wartości przywracanego przez miksturę zdrowia, o jaką wzrasta jej siła leczenia.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>hp</code></center></td><td>• Działanie: zwiększenie puli punktów zdrowia postaci o stałą wartość.<br>
• Zmienna: liczba punktów życia o jaką rośnie pula punktów zdrowia postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>hp_per-allies</code></center></td><td>• Działanie: zwiększa pulę punktów zdrowia wszystkich członków drużyny o część posiadanych punktów zdrowia.<br>
• Zmienna: część posiadanych punktów życia, o jaką rośnie pula punktów zdrowia.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt działa do końca trwania walki.<br>
• Dynamicznie zwiększa pulę zdrowia postaci, sprawiając, że rozpoczyna walkę z innym poziomem zdrowia, niż w chwili przed jej rozpoczęciem.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>hpbon</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadaną przez postać siłę i wynik dodaje do puli punktów zdrowia postaci.<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty życia za każdy punkt siły.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>immunity_to_dmg</code></center></td><td>• Działanie: postać staje się niewrażliwa na otrzymywane obrażenia.<br>
• Zmienna: brak.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, która rzuciła umiejętność.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>injure</code></center></td><td>• Działanie: określa szansę na zajście zdarzenia (Zranienie), podczas którego aplikowane są na cel obrażenia od głębokiej rany (jako osobna instancja wyniszczeń) o wartości 15% obrażeń zadanych na 3 tury.<br>
• Zmienna: szansa na zajście zdarzenia zranienia.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Zdarzenie może wystąpić tylko podczas trafionego ataku w przeciwnika.<br>
• Typ obrażeń to głęboka rana i są one redukowane przez efekt <code>woundred</code>.<br>
• Efekt obrażeń nie kumuluje się.<br>
• Efekt obrażeń nadpisuje się najświeższą nałożoną na danego przeciwnika wartością.<br>
• Obliczanie wartości obrażeń następuje przed ich wyzerowaniem przez efekt <code>immunity_to_dmg</code>, a zatem są wciąż aplikowane na przeciwnika.<br>
</td><td><center>pasywny</center><br>
<br>
</td></tr><tr><td><center><code>lastcrit</code></center></td><td>• Działanie: zwiększa szansę na zajście zdarzenia cios krytyczny oraz cios krytyczny pomocniczy w przypadku, gdy poziom zdrowia przeciwnika jest niższy od 20% jego puli zdrowia.<br>
• Zmienna: liczba punktów procentowych o jaką rośnie szansa na cios krytyczny.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Zwiększa również szansę na wystąpienie zdarzenia cios bardzo krytyczny oraz cios bardzo krytyczny pomocniczy.<br>
• Dodatkowe punkty procentowe w zajście zdarzenia na cios krytyczny nie mogą zostać obniżone przez efekty przeciwnika.<br>
• Łączy się addytywnie z efektem <code>active_crit</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>lightbon</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadany przez postać intelekt i wynik dodaje do maksymalnych obrażeń od błyskawic postaci (oraz 66% tej wartości do obrażeń minimalnych).<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń za każdy punkt intelektu.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center><br>
<br>
</td></tr><tr><td><center><code>lightshield_per</code></center></td><td>• Działanie: nakłada na postać efekt, który podczas przyjmowania przez nią ataku, odbija w przeciwnika losowo od 6% do 14% zadanych przez niego obrażeń oraz spowalnia go na jedną turę.<br>
• Zmienna: część szybkości ataku, o jaką zostaje spowolniony przeciwnik atakujący postać.<br>
• Aplikacji: warstwa inicjacji.<br>
• Wyzwolenie: warstwa finalizacji u przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, na którą została rzucona umiejętność.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy. W przypadku nałożenia podwójnego efektu, obrażenia odbijane w przeciwnika są dwukrotnie, jednak za drugim razem efekt jest 50% słabszy.<br>
• Spowolnienie łączy się w sposób addytywny z efektami <code>adrenalin_sa_per, critsa_per, sa_per, sa2_per, aura-sa_per, allslow_per, critslow_per</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>lowdmg_enemy</code></center></td><td>• Działanie: w przypadku trafionego ciosu, nakłada na przeciwnika efekt, osłabiający wartość jego obrażeń od ataku o część określoną w parametrze efektu.<br>
• Zmienna: część wartości, o jaką maleją obrażenia przeciwnika.<br>
• Aplikacja: warstwa obrażeń.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt zmniejsza też obrażenia odbite w postać, nawet podczas wykonywania umiejętności gdy czas trwania jest równy 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, na którą została rzucona umiejętność.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł spośród efektów: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code>.<br>
• Efekt łączy się w sposób addytywny z pozostałymi efektami: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code><br>
• Wzmocnienie łączy się w sposób multiplikatywny z innymi modyfikatorami obrażeń (również z przyrostem obrażeń na skutek ciosu krytycznego).<br>
• Obrażenia widoczne w logu walki są już pomniejszone przez ten efekt.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>lowdmg_self</code></center></td><td>• Działanie: zmniejsza wartość obrażeń postaci rzucającej czar o część określoną w parametrze efektu na jedną turę.<br>
• Zmienna: część wartości, o jaką maleją obrażenia postaci.<br>
• Aplikacja: warstwa obrażeń.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Efekt łączy się w sposób multiplikatywny z innymi efektami modyfikacji wartości obrażeń (łącznie z ciosem krytycznym).<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>lowheal_per-enemies</code></center></td><td>• Działanie: zmniejsza wartość leczenia z efektów umiejętności aktywnych wszystkich postaci z drużyny przeciwnej.<br>
• Zmienna: część wartości, o jaką maleją efekty przywracania zdrowia z umiejętności.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Redukuje leczenie wywołane przez efekty <code>healall_per, heal_per, combo_heal_per</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>mana</code></center></td><td>• Działanie: określenie kosztu umiejętności w postaci wymaganych punktów many, które postać traci po użyciu umiejętności.<br>
• Zmienna: liczba punktów many wymagana do użycia umiejętności, którą gracz traci po jej użyciu.<br>
• Wyzwolenie: warstwa wymagań.<br>
• Umiejętność nie może zostać użyta, jeżeli bieżąca mana postaci jest mniejsza niż parametr efektu.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>manabon</code></center></td><td>• Działanie: zwiększa pulę many postaci o liczbę punktów określoną w parametrze.<br>
• Zmienna: liczba punktów many o jaką rośnie pula many postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>manaendest</code></center></td><td>• Działanie: zmniejsza bieżącą pulę punktów energii i many przeciwnika o stałą wartość.<br>
• Zmienna: liczba punktów energii i many, o jaką pomniejszone są zasoby przeciwnika. Liczba zniszczonych punktów many jest co do wartości równa podanemu parametrowi, natomiast liczba punktów energii jest trzy razy mniejsza.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Bieżąca liczba punktów energii i many przeciwnika nie może spaść poniżej zera.<br>
• Wartość niszczonych zasobów jest pomniejszana na skutek działania efektu <code>reddest_per</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>managain</code></center></td><td>• Działanie: przywraca liczbę punktów many po zakończeniu tury postaci.<br>
• Zmienna: liczba przywracanych punktów many.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Liczba przywróconej many nie może przekroczyć puli many, z którą postać rozpoczynała walkę.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>manarestore_per</code></center></td><td>• Działanie: przywraca część posiadanej puli punktów many.<br>
• Zmienna: część przywracanej puli punktów many.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Liczba przywróconej many nie może przekroczyć puli many, z którą postać rozpoczynała walkę.<br>
• Wartość przywróconych zasobów podczas kolejnych użyć umiejętności z tym efektem jest o 10% niższa od wartości początkowej.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>manastr</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadany przez postać intelekt i wynik dodaje do puli punktów many postaci.<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty many za każdy punkt intelektu.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>mcurse</code></center></td><td>• Działanie: nakładany jest na przeciwnika efekt, który określa szansę na zajście zdarzenia, podczas którego zostaje zaniechana próba wykonania akcji, o ile postać rzucająca czar wykona w niego atak. W przypadku zajścia zdarzenia (Klątwa), w logu walki widnieje informacja o utracie tury.<br>
• Zmienna: szansa na zaniechanie akcji przeciwnika w bieżącej turze.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa zdarzeń u przeciwnika.<br>
• Aplikacja i wyzwolenie zdarzenia są jawne i sygnalizowane w logu walki.<br>
• Zdarzenie może zajść wyłącznie podczas trafionego ataku w przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, na którą została rzucona umiejętność.<br>
• Efekt łączy się w sposób addytywny z bonusem legendarnym Klątwa.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>of-crit</code></center></td><td>• Działanie: zwiększa szansę na cios krytyczny pomocniczy postaci.<br>
• Zmienna: liczba punktów procentowych o jakie rośnie szansa na cios krytyczny pomocniczy w statystykach postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>of-critval</code></center></td><td>• Działanie: zwiększa siłę ciosu krytycznego pomocniczego w statystykach postaci.<br>
• Zmienna: liczba dodatkowych punktów w siłę ciosu krytycznego fizycznego pomocniczego.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>of-str</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadaną przez postać siłę i wynik dodaje do obrażeń minimalnych pomocniczych oraz maksymalnych pomocniczych postaci. <br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń pomocniczych za każdy punkt siły.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>of-thirdatt</code></center></td><td>• Działanie: określa szansę na zajście zdarzenia (Trzeci cios), podczas którego postać wykonuje dodatkowy atak pomocniczy o wartości losowanej między minimalnymi a maksymalnymi obrażeniami broni głównej powiększonymi o efekt <code>str1h</code>.<br>
• Zmienna: szansa na zajście zdarzenia trzeciego ciosu.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Obrażenia od trzeciego ciosu są redukowane przez te same efekty co obrażenia pomocnicze, jednak nie są poddawane pod redukcję obrażeń ze zdarzenia bloku, parowania oraz uniku.<br>
• Podczas zajścia zdarzenia przebicia pancerza, obrażenia od trzeciego ciosu również ignorują pancerz przeciwnika.<br>
• Obrażenia od trzeciego ciosu nigdy nie są zwiększane na skutek zajścia zdarzenia cios krytyczny.<br>
• Obrażenia od trzeciego ciosu nie są zwiększane na skutek addytywnych modyfikatorów obrażeń.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>of-wounddmgbon_perw</code></center></td><td>• Działanie: zwiększa obrażenia od głębokiej rany broni pomocniczej o część określoną w parametrze efektu.<br>
• Zmienna: część wartości, o jaką rosną obrażenia od głębokiej rany broni pomocniczej.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Dodatkowe obrażenia są uwzględniane do obliczania maksymalnych możliwych do zadania obrażeń od głębokiej rany.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>parry</code></center></td><td>• Działanie: określa szansę na zajście zdarzenia (Parowanie), podczas którego obrażenia od broni białej (klasa przedmiotu: jednoręczne, dwuręczne, półtoraręczne, pomocnicze) zostają zredukowane do zera i następuje efekt <i>chybienia</i>.<br>
• Zmienna: szansa na zajście zdarzenia parowania.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Efekt chybienia wyłącza aplikację efektów z tej broni, takich jak: głęboka rana, przebicie pancerza, klątwa, trucizna, zranienie, ciężka rana, ogłuszenie.<br>
• Zdarzenie może zajść wyłącznie podczas przyjęcia ataku od broni białej przez postać posiadającą umiejętność z tym efektem.<br>
• W przypadku, gdy przeciwnik atakuje bronią pomocniczą, może ona zostać sparowana o ile nie została sparowana broń główna. Następuje wtedy osobne losowanie. W przypadku, gdy sparowana zostanie broń pomocnicza, mogą zajść efekty nakładane przez broń główną (ogłuszenie, klątwa, zranienie, ciężka rana, trucizna broni głównej, głęboka rana broni głównej), ale nie mogą zaaplikować się efekty broni pomocniczej (trucizna broni pomocniczej, głęboka rana broni pomocniczej).<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>pcontra</code></center></td><td>• Działanie: określa szansę na zajście zdarzenia (Kontra), podczas którego, w przypadku zajścia zdarzenia Parowanie, wyzwala dodatkowy automatyczny atak  (opisany w ramach efektu <code>contra</code>).<br>
• Zmienna: szansa na zajście zdarzenia kontry w przypadku zajścia zdarzenia parowania.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Zdarzenie może zajść wyłącznie podczas przyjęcia ataku od broni białej (klasa przedmiotu: jednoręczne, dwuręczne, półtoraręczne, pomocnicze) przez postać posiadającą umiejętność z tym efektem.<br>
• Efekt łączy się w sposób addytywny z efektem <code>contra</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>perdmg</code></center></td><td>• Działanie: zwiększa obrażenia wykonywane przez postać o część określoną w parametrze efektu.<br>
• Zmienna: część wartości, o jaką wzrastają obrażenia postaci.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Wzmocnienie łączy się w sposób multiplikatywny z innymi modyfikatorami obrażeń (również z przyrostem obrażeń na skutek ciosu krytycznego).<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, na którą została rzucona umiejętność.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>perdmg-allies</code></center></td><td>• Działanie: zwiększa obrażenia wykonywane przez wszystkich członków drużyny o część określoną w parametrze efektu.<br>
• Zmienna: część wartości, o jaką wzrastają obrażenia postaci.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Efekt łączy się w sposób addytywny z efektem <code>perdmg</code>.<br>
• Wzmocnienie łączy się w sposób multiplikatywny z innymi modyfikatorami obrażeń (również z przyrostem obrażeń na skutek ciosu krytycznego).<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, na którą została rzucona umiejętność.<br>
• Efekt działa w połowie skutecznie na postać rzucającą umiejętność.<br>
• Efekt kumuluje się do dwóch najwyższych źródeł od różnych graczy.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>pierce</code></center></td><td>• Działanie: ustala szansę na zajście zdarzenia (Przebicie pancerza), podczas którego, w momencie redukowania wykonanych przez postać obrażeń, ignorowany jest pancerz przeciwnika.<br>
• Zmienna: liczba punktów procentowych, o jaką wzrasta szansa na przebicie pancerza.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Efekt zdarzenia może zostać anulowany w przypadku zajścia zdarzenia bloku lub bloku przebicia.<br>
• Zdarzenie może zajść wyłącznie podczas wykonywania ataku w przeciwnika.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>poison_lowdmg_per-enemies</code></center></td><td>• Działanie: zmniejsza obrażenia od ataku i instancji obrażeń (innych niż efekty rozłożone w czasie) przeciwnika w przypadku nałożonych na niego obrażeń od trucizny z dowolnego źródła.<br>
• Zmienna: część redukowanych obrażeń wykonanych przez przeciwnika.<br>
• Aplikacja: warstwa finalizacji.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł spośród efektów: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code>.<br>
• Efekt łączy się w sposób addytywny z pozostałymi efektami: <code>combo_lowdmg_enemy, lowdmg_enemy, poison_lowdmg_per-enemies, dmg_from_player_per</code><br>
• Wzmocnienie łączy się w sposób multiplikatywny z innymi modyfikatorami obrażeń (również z przyrostem obrażeń na skutek ciosu krytycznego).<br>
• Obrażenia widoczne w logu walki są już pomniejszone przez ten efekt.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>poisonbon_poison-perw</code></center></td><td>• Działanie: nakłada na przeciwnika obrażenia od trucizny na 5 tur o wartości zależnej od posiadanych przez postać obrażeń od trucizny, powiększonych o część określoną w parametrze efektu. <br>
• Zmienna: część wartości, o jaką aplikowane są na przeciwnika obrażenia od trucizny.<br>
• Aplikacja: warstwa finalizacji.<br>
• Efekt wymaga trafienia przeciwnika oraz wykonania niezerowych obrażeń zadanych.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Po 5 turach efekt wygasa, wyłączając również obrażenia od trucizny. <br>
• Podczas nakładania efektu na przeciwnika, uwzględniana jest najwyższa działająca na niego wartość, jednak każda dodatkowa aplikacja obrażeń od efektu, przedłuża czas trwania obrażeń.<br>
• Obrażenia od trucizny pochodzącej z broni pomocniczej, są wzmacniane osobno. W przypadku, gdy broń główna chybi, nakładane są wyłącznie obrażenia od trucizny broni pomocniczej. W przypadku, gdy broń pomocnicza chybi (zdarzenie Parowania), nakładane są obrażenia od trucizny z obu źródeł.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>rage</code></center></td><td>• Działanie: po otrzymaniu przez postać ciosu krytycznego, jej obrażenia zostają zwiększone o 10%.<br>
• Zmienna: liczba tur na jaką zostają zwiększone obrażenia po otrzymaniu ciosu krytycznego.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Wzmocnienie łączy się addytywnie z innymi modyfikatorami do obrażeń.<br>
• Wzmocnienie nie łączy się z efektem <code>rage3_turns</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>rage_3turns</code></center></td><td>• Działanie: po otrzymaniu przez postać ciosu krytycznego, jej obrażenia zostają zwiększone o część określoną w parametrze efektu na 3 tury.<br>
• Zmienna: część obrażeń jaka ulega wzmocnieniu po przyjęciu przez postać ciosu krytycznego.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Wzmocnienie łączy się addytywnie z innymi modyfikatorami do obrażeń.<br>
• Wzmocnienie nie łączy się z efektem <code>rage</code>.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>redabdest_per</code></center></td><td>• Działanie: redukuje niszczenie absorpcji, którego źródłem są przedmioty przeciwnika.<br>
• Zmienna: część posiadanego przez przeciwnika niszczenia absorpcji, która ulega zmniejszeniu.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>redacdmg_per</code></center></td><td>• Działanie: redukuje niszczenie pancerza, którego źródłem są przedmioty i umiejętności przeciwnika.<br>
• Zmienna: część posiadanego przez przeciwnika niszczenia pancerza, która ulega zmniejszeniu.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>reddest_per</code></center></td><td>• Działanie: redukuje niszczenie energii i many, którego źródłem są przedmioty i umiejętności przeciwnika.<br>
• Zmienna: część posiadanego przez przeciwnika niszczenia energii oraz many, która ulega zmniejszeniu.<br>
• Wyzwolenie: warstwa obrażeń u przeciwnika.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>red-sa</code></center></td><td>• Działanie: skraca czas trwania ataku o część zadaną w parametrze efektu.<br>
• Zmienna: część czasu trwania ataku, która ulega skróceniu.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Łączy się w sposób multiplikatywny z innymi efektami skracającymi czas trwania ataku.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>redslow</code></center></td><td>• Działanie: zmniejsza wartość spowolnień stałych, którego źródłem są przedmioty przeciwnika.<br>
• Zmienna: część wartości, o jaką są zmniejszane spowolnienia z przedmiotów przeciwnika.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Nie redukuje dodatkowego spowolnienia wynikającego ze wzmocnienia spowolnień od zimna.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>redstun</code></center></td><td>• Działanie: skraca czas trwania tur, podczas których postać podlega efektom ogłuszenia (<code>stun, freeze, stun2</code>).<br>
• Zmienna: część czasu trwania ataku, która ulega skróceniu.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>removeslow-allies</code></center></td><td>• Działanie: usuwa ze wszystkich członków drużyny efekty spowolnienia rozłożone w czasie, których źródłem jest ekwipunek oraz umiejętności przeciwników.<br>
• Zmienna: brak.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• W przypadku trwania na postaci obrażeń od trucizny rozłożonych w czasie, usuwa spowolnienie do momentu aż ponownie nie zostanie przedłużony efekt trucizny.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>removestun-allies</code></center></td><td>• Działanie: usuwa ze wszystkich członków drużyny efekty ogłuszenia (<code>stun, freeze, stun2</code>).<br>
• Zmienna: brak.<br>
• Wyzwolenie: warstwa inicjacji.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>resdmg</code></center></td><td>• Działanie: zwiększa niszczenie odporność przeciwnika w statystykach postaci.<br>
• Zmienna: liczba punktów procentowych, o jaką maleją odporności przeciwnika.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>resfire</code></center></td><td>• Działanie: zwiększa odporność na ogień postaci.<br>
• Zmienna: liczba punktów procentowych, o jaką rosną odporności na ogień postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>resfire_per</code></center></td><td>• Działanie: zwiększa odporność na ogień postaci, na którą rzucona jest umiejętność.<br>
• Zmienna: liczba punktów procentowych, o jaką rosną odporności na ogień postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Może trwać dłużej niż 1 turę.<br>
• Może działać na postać rzucającą umiejętność lub na sojusznika.<br>
• Może przyjmować wartości ujemne.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>resfrost</code></center></td><td>• Działanie: zwiększa odporność na zimno postaci.<br>
• Zmienna: liczba punktów procentowych, o jaką rosną odporności na zimno postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>resfrost_per</code></center></td><td>• Działanie: zwiększa odporność na zimno postaci, na którą rzucona jest umiejętność.<br>
• Zmienna: liczba punktów procentowych, o jaką rosną odporności na zimno postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Może trwać dłużej niż 1 turę.<br>
• Może działać na postać rzucającą umiejętność lub na sojusznika.<br>
• Może przyjmować wartości ujemne.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>reslight</code></center></td><td>• Działanie: zwiększa odporność na błyskawice postaci.<br>
• Zmienna: liczba punktów procentowych, o jaką rosną odporności na błyskawice postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>reslight_per</code></center></td><td>• Działanie: zwiększa odporność na błyskawice postaci, na którą rzucona jest umiejętność.<br>
• Zmienna: liczba punktów procentowych, o jaką rosną odporności na błyskawice postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Może trwać dłużej niż 1 turę.<br>
• Może działać na postać rzucającą umiejętność lub na sojusznika.<br>
• Może przyjmować wartości ujemne.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>reusearrows</code></center></td><td>• Działanie: po zakończeniu walki, gracz otrzymuje część użytych podczas niej strzał.<br>
• Zmienna: część użytych strzał, którą odzyskuje gracz po zakończeniu walki.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>sa_per</code></center></td><td>• Działanie: zwiększa szybkość ataku postaci o pewną jej część.<br>
• Zmienna: część wartości o jaką wzrasta szybkość ataku postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Przyspieszenie łączy się w sposób addytywny z efektami <code>critsa_per, adrenalin_sa_per, sa2_per, aura-sa_per, allslow_per, critslow_per, lightshield_per</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>sa1</code></center></td><td>• Działanie: zwiększa szybkość ataku postaci o stałą liczbę punków.<br>
• Zmienna: liczba punktów, o jaką wzrasta szybkość ataku w statystykach postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>sa2_per</code></center></td><td>• Działanie: zwiększa szybkość ataku postaci o pewną jej część.<br>
• Zmienna: część wartości o jaką wzrasta szybkość ataku postaci.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Przyspieszenie łączy się w sposób addytywny z efektami <code>critsa_per, adrenalin_sa_per, sa_per, aura-sa_per, allslow_per, critslow_per, lightshield_per</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>sa-clothes</code></center></td><td>• Działanie: zwiększa szybkość ataku o część wartości szybkości ataku, która pochodzi z ekwipunku postaci.<br>
• Zmienna: część szybkości ataku pochodzącej z ekwipunku postaci, o którą rosną statystyki postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>shout</code></center></td><td>• Działanie: zmusza postacie, na które nałożony jest efekt, do obierania za cel ataku postaci, która użyła umiejętności z tym efektem. Efekt działa na gracza, będącego celem umiejętności oraz losowo na pozostałą liczbę graczy określoną w parametrze efektu.<br>
• Zmienna: liczba postaci, która zostaje zmuszona do obrania sobie za cel ataku posiadacza efektu.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Czas trwania efektu może być większy od 1.<br>
• Postać objęta działaniem efektu, może wciąż używać akcji rzucanych na samą siebie (również jeśli w konsekwencji efekt używanych przez nich umiejętności działa na całą drużynę).<br>
• Podczas działania efektu, nie może zajść zdarzenie Kontry.<br>
• Jeżeli postać nie jest w zasięgu ataku, wyzwany potwór wykonuje <i>Krok do przodu</i>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>slowfreeze_per</code></center></td><td>• Działanie: zwiększa spowolnienie z broni od zimna o pewną część określoną w parametrze efektu.<br>
• Zmienna: część wartości, o jaką zostaje zwiększone spowolnienie z broni postaci.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Dodatkowe spowolnienie nie jest redukowane przez efekt <code>redslow</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>stealmana_per</code></center></td><td>• Działanie: zabiera przeciwnikowi część posiadanej przez niego many i przekazuje postaci gracza, używającego umiejętności z tym efektem.<br>
• Zmienna: część many, która zostaje odebrana postaci przeciwnika i przekazana postaci gracza.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt nie jest zmniejszany przez żadne efekty redukcji niszczenia many.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>stinkbomb</code></center></td><td>• Działanie: nakłada na przeciwnika efekt obniżający jego szansę na cios krytyczny, cios krytyczny pomocniczy oraz przebicie pancerza.<br>
• Zmienna: liczba punktów procentowych obniżających szansę na cios krytyczny przeciwnika oraz przebicie pancerza. Przebicie pancerza zostaje obniżone przez podwojoną wartość parametru umiejętności.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt nie wpływa na szansę zajścia zdarzenia ciosu bardzo krytycznego oraz ciosu bardzo krytycznego pomocniczego.<br>
• Efekt łączy się w sposób addytywny z efektami <code>active_crit, active_crit-allies, disturb</code>.<br>
• Szansa na cios krytyczny przeciwnika nie może spaść poniżej 1%.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>stinkbomb_crit</code></center></td><td>• Działanie: nakłada na przeciwnika efekt obniżający jego szansę na cios krytyczny oraz cios krytyczny pomocniczy.<br>
• Zmienna: liczba punktów procentowych obniżających szansę na cios krytyczny przeciwnika.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt nie wpływa na szansę zajścia zdarzenia ciosu bardzo krytycznego oraz ciosu bardzo krytycznego pomocniczego.<br>
• Efekt łączy się w sposób addytywny z efektami <code>active_crit, active_crit-allies, disturb</code>.<br>
• Szansa na cios krytyczny przeciwnika nie może spaść poniżej 1%.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>stinkbomb_pierce</code></center></td><td>• Działanie: nakłada na przeciwnika efekt obniżający jego szansę na przebicie pancerza.<br>
• Zmienna: liczba punktów procentowych obniżających szansę na przebicie pancerza.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa inicjacji u przeciwnika.<br>
• Efekt ulega kumulacji do maksymalnie dwóch źródeł od różnych graczy.<br>
• Czas trwania efektu może być większy od 1.<br>
• Szansa na przebicie pancerza przeciwnika nie może spaść poniżej 1%.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>str1h</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadaną przez postać siłę i wynik dodaje do obrażeń minimalnych oraz maksymalnych postaci jeżeli posiada wyekwipowaną broń jednoręczną (lub półtoraręczną noszoną z tarczą).<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń za każdy punkt siły.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>str2h</code></center></td><td>• Działanie: mnoży wartość podaną jako parametr przez posiadaną przez postać siłę i wynik dodaje do obrażeń minimalnych oraz maksymalnych postaci jeżeli posiada wyekwipowaną broń dwuręczną (lub półtoraręczną bez tarczy).<br>
• Zmienna: mnożnik wpływający na otrzymywane punkty obrażeń za każdy punkt siły.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>stun</code></center></td><td>• Działanie: określa szansę na zajście zdarzenia (Ogłuszenie), które ogłusza przeciwnika wprowadzając efekt zablokowania tury przeciwnika. Podczas zablokowanej tury, gracz nie może wykonać żadnej akcji.<br>
• Zmienna: liczba punktów procentowych określająca szansę na zajście zdarzenia ogłuszenia.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Zdarzenie ogłuszenia może zajść wyłącznie podczas trafionego ataku, podczas którego nie zaszło zdarzenie bloku.<br>
• Podczas atakowania ogłuszonego przeciwnika, nie mogą zajść zdarzenia bloku, uniku, parowania, bloku strzały, kontry, bloku przebicia oraz Płomiennego oczyszczenia.<br>
• Czas trwania ogłuszenia jest redukowany przez efekt redstun.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>sunshield_per</code></center></td><td>• Działanie: zwiększa pancerz postaci oraz leczenie pochodzące z przedmiotów o pewną część określoną w parametrze efektu. Dodatkowy pancerz oraz leczenie maleją o 20% przyrostu początkowego wraz z każdą turą postaci.<br>
• Zmienna: część wartości, o jaką rośnie pancerz i leczenie postaci.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest zależny od liczby tur wykonanej przez postać, która rzuciła umiejętność.<br>
• Dodatkowy pancerz nie może zostać zredukowany przez przeciwnika.<br>
• Dodatkowe leczenie może ulec modyfikacji na skutek efektów <code>heal_per-allies, critpoison_per, heal_per-enemies</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>swing</code></center></td><td>• Działanie: określa szansę na zajście zdarzenia (Szeroki zamach), które zadaje dodatkowe obrażenia fizyczne losowane z ataku (fizycznego) broni głównej, maksymalnie trzem losowym niepowtarzającym się przeciwnikom, których postać może obrać za cel ataku bez zmiany pozycji.<br>
• Zmienna: liczba punktów procentowych określająca szansę na zajście zdarzenia szerokiego zamachu.<br>
• Wyzwolenie: warstwa zdarzeń.<br>
• Dodatkowe obrażenia nie ulegają wzmocnieniom od umiejętności i zdarzenia ciosu krytycznego.<br>
• Efekt wymaga posiadania obrażeń fizycznych i nie dotyczy obrażeń dystansowych.<br>
• Dodatkowe obrażenia nie są redukowane przez efekty obniżające obrażenia ataku postaci, efekty bonusów legendarnych i absorpcję.<br>
• Dodatkowe obrażenia są redukowane przez pancerz.<br>
• Efekt nie zachodzi podczas ataku będącego ciosem śmiertelnym.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>taken_dmg_per</code></center></td><td>• Działanie: nakłada na przeciwnika efekt, zwiększający wymierzone w niego obrażenia o pewną część.<br>
• Zmienna: część obrażeń zadanych, która ulega zwiększeniu.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt umiejętności oblicza dodatkowe obrażenia względem obrażeń wykonanych przez postać atakującą przed wszelkimi efektami redukcji obrażeń.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na przeciwnika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt kumuluje się do dwóch najwyższych źródeł od różnych graczy.<br>
• W przypadku wielu instancji obrażeń (np: obrażenia fizyczne i magiczne), każda z nich obliczana jest osobno, a dopiero na sam koniec są ze sobą sumowane.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>taken_dmg_per-all</code></center></td><td>• Działanie: nakłada na przeciwnika efekt, zwiększający wymierzone w niego obrażenia o pewną część.<br>
• Zmienna: część obrażeń zadanych, która ulega zwiększeniu.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt umiejętności oblicza dodatkowe obrażenia względem obrażeń wykonanych przez postać atakującą przed wszelkimi efektami redukcji obrażeń.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na przeciwnika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt kumuluje się do dwóch najwyższych źródeł od różnych graczy.<br>
• W przypadku wielu instancji obrażeń (np: obrażenia fizyczne i magiczne), każda z nich obliczana jest osobno, a dopiero na sam koniec są ze sobą sumowane.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>taken_dmg_per-row</code></center></td><td>• Działanie: nakłada na wszystkich przeciwników stojących w tej samej linii efekt, zwiększający wymierzone w nich obrażenia o pewną część.<br>
• Zmienna: część obrażeń zadanych, która ulega zwiększeniu.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt umiejętności oblicza dodatkowe obrażenia względem obrażeń wykonanych przez postać atakującą przed wszelkimi efektami redukcji obrażeń.<br>
• Czas trwania efektu może być większy od 1.<br>
• Efekt jest nakładany na przeciwnika i zależy od liczby wykonanych przez niego tur.<br>
• Efekt kumuluje się do dwóch najwyższych źródeł od różnych graczy.<br>
• W przypadku wielu instancji obrażeń (np: obrażenia fizyczne i magiczne), każda z nich obliczana jest osobno, a dopiero na sam koniec są ze sobą sumowane.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>vamp</code></center></td><td>• Działanie: zadaje stałe obrażenia od umiejętności oraz przywraca postaci punkty zdrowia o tę samą wartość.<br>
• Zmienna: liczba punktów obrażeń oraz leczenia.<br>
• Wyzwolenie: warstwa inicjacji.<br>
• Efekt leczenia jest obniżany przez efekt <code>lowheal_per-enemies</code>.<br>
• Obrażenia są obniżane przez efekt <code>dmg_from_player_per</code>.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>vamp_time_per</code></center></td><td>• Działanie: nakłada na postać efekt, przywracający zdrowie postaci o wartości części obrażeń zadanych w przeciwnika.<br>
• Zmienna: część obrażeń zadanych, która determinuje przywracane punkty zdrowia postaci.<br>
• Aplikacja: warstwa inicjacji.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt leczenia jest obniżany przez efekt <code>lowheal_per-enemies</code>.<br>
• Czas trwania efektu może być większy od 1.<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>vulture_perw</code></center></td><td>• Działanie: w przypadku, gdy cel ataku ma poziom zdrowia niższy niż 20%, obrażenia zadane zostają zwiększone o część obrażeń wykonanych.<br>
• Zmienna: część obrażeń wykonanych, o którą zostają zwiększane obrażenia zadane.<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa finalizacji.<br>
• Efekt zwiększa tylko zadane obrażenia fizyczne lub dystansowe.<br>
• Dodatkowe obrażenia są dodawane na samym końcu procesu po uwzględnieniu wszelkich efektów redukcji - są więc redukowane wyłącznie przez efekty umiejętności osłabiające źródła obrażeń (<code>dmg_from_player_per, poison_lowdmg_per-enemies</code>).<br>
</td><td><center>aktywny</center></td></tr><tr><td><center><code>woundchance</code></center></td><td>• Działanie: zwiększa szansę na zajście zdarzenia (Głęboka rana, Głęboka rana pomocnicza), podczas którego na cel zostają nałożone obrażenia od głębokiej rany rozłożone w czasie 5 tur.<br>
• Zmienna: liczba punktów procentowych, o jakie rośnie szansa na zdarzenie głębokiej rany i głębokiej rany pomocniczej (w przypadku posiadania broni pomocniczej z obrażeniami głębokiej rany).<br>
• Aplikacja: warstwa zdarzeń.<br>
• Wyzwolenie: warstwa obrażeń.<br>
• Efekt wymaga posiadania broni głównej z obrażeniami od głębokiej rany (w przypadku zajścia zdarzenia Głęboka rana) lub broni pomocniczej z obrażeniami od głębokiej rany (w przypadku zajścia zdarzenia Głęboka rana pomocnicza).<br>
• Obrażenia aplikują się wyłącznie podczas trafionego ataku w przeciwnika.<br>
• Zdarzenie dla broni pomocniczej oraz głównej obliczane jest osobno.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>wounddmgbon_perw</code></center></td><td>• Działanie: zwiększa obrażenia od głębokiej rany z broni głównej o część określoną w parametrze efektu.<br>
• Zmienna: część wartości, o jaką rosną obrażenia od głębokiej rany w statystykach postaci.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
</td><td><center>pasywny</center></td></tr><tr><td><center><code>woundred</code></center></td><td>• Działanie: określa odporność postaci na obrażenia od głębokiej rany.<br>
• Zmienna: część wartości, o jaką są pomniejszone wszelkie obrażenia od głębokiej rany.<br>
• Wyzwolenie: statystyki bazowe postaci.<br>
• Odporności nie mogą zostać obniżone.<br>
• Maksymalna wartość redukcji obrażeń od głębokiej rany wynosi 90%.<br>
</td><td><center>pasywny</center></td></tr></tbody></table><br><br><br>
<br>
<hr><a name="k4"></a><h2><b>4. Atrakcje oparte na walce</b></h2><a name="k41"></a><b><h3>4.1. Otchłań</h3></b>Otchłań jest atrakcją bazującą na solowych pojedynkach między graczami. Pojawia się niecyklicznie, a termin wydarzenia (okres trwania, dni oraz godziny) jest podawany wraz z jego zapowiedzią.<br>
<br><br>
<h3><span class="color-blue">Warunki uczestnictwa</span></h3>W celu wzięcia udziału w atrakcji w momencie rozpoczęcia wydarzenia, należy skorzystać z modułu <i>Otchłań</i>. Dostęp do modułu wymaga posiadania poziomu większego lub równego 40. Zarówno w Starym Interfejsie jak i Nowym Interfejsie znajduje się specjalny przycisk uruchamiający moduł Otchłani, który z kolei jest podzielony na sekcje:<br>
• Postęp - gdzie gracz może odebrać na postaci nagrody za udział w Otchłani, przejrzeć <i>Sklep Czempionów</i> oraz nagrody za koniec sezonu, sprawdzić swoją historię walk, wyniki postaci czy stosunek wygranych walk z konkretną profesją.<br>
• Szukaj walki - przycisk zapisujący postać do kolejki, w której trwa wyszukiwanie przeciwnika. Za wyszukiwanie partnera do walki odpowiada system <i>matchmakingu</i>, odpowiednio przeszukując kandydata wśród zapisanych do kolejki postaci, uwzględniając takie czynniki jak:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ czas oczekiwania w kolejce<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ poziom postaci<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ ekwipunek postaci<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ pozycja w rankingu<br>
Po odnalezieniu przeciwnika, następuje uruchomienie pojedynku. Postać gracza chwilowo znika z mapy, przeprowadzana jest walka, a następnie postać wraca na miejsce sprzed znalezienia przeciwnika.<br>
• Ranking - zestawienie pozycji w rankingu graczy w obrębie serwera, listy znajomych postaci lub klanowiczy.<br>
<br>
Warunki zapisu do kolejki:<br>
• Postać nie znajduje się na mapie typu Arena ani nie uczestniczy w Krwawej Łaźni.<br>
• Postać nie ma blokady zapisu do kolejki wynikającej z przekroczenia pewnego progu Punktów ostrzeżenia.<br>
<br><br>
<h3><span class="color-blue">Wyszukiwanie przeciwnika</span></h3>• Maksymalny poziom gracza, z którym można stoczyć walkę, wynosi 110% poziomu postaci, ale różnica między poziomami (widełki) nie jest mniejsza niż 5 poziomów oraz nie przekracza 15 poziomów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<i>Przykłady:</i> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dla gracza z poziomem 40 maksymalny poziom dobranego przeciwnika wynosi 45.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dla gracza z poziomem 75 maksymalny poziom dobranego przeciwnika wynosi 83.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dla gracza z poziomem 100 maksymalny poziom dobranego przeciwnika wynosi 110.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dla gracza z poziomem 250 maksymalny poziom dobranego przeciwnika wynosi 265.<br>
• Wszystkie postacie z poziomem przewyższającym 300, są traktowane, jakby miały poziom 300.<br>
• Im dłużej gracz oczekuje w kolejce, tym bardziej rosną jego szanse na wylosowanie przeciwnika z wyższym poziomem oraz zwiększa się jego priorytet na odnalezienie przeciwnika.<br>
• Maksymalna różnica Punktów Rankingowych, między mogącymi siebie znaleźć postaciami, wynosi 400.<br>
• Gracze należący do 10% najlepszych pod względem liczby Punktów Rankingowych (Grupa Śmierci), mogą znaleźć przeciwnika o różnicy punktowej większej niż 400, ale pod warunkiem, że oczekują na walkę co najmniej 40 sekund.<br>
• Gracze należący do 10% najsłabszych pod względem liczby Punktów Rankingowych (Grupa Przegranych), mogą znaleźć przeciwnika o różnicy punktowej większej niż 400, ale pod warunkiem, że oczekują na walkę co najmniej 40 sekund.<br>
• Postać musi móc znaleźć co najmniej 2 aktywnych przeciwników żeby walka mogła zostać uruchomiona.<br>
• Minimalny czas oczekiwania na walkę wynosi 20 sekund.<br>
• Odrzucenie walki z przeciwnikiem prowadzi do przyznania Punktów ostrzeżenia, skutkujących blokadą wejścia do kolejki:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 3 Punkty ostrzeżenia – blokada na 3 minuty<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 6 Punktów ostrzeżenia – blokada na 15 minut<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 9 Punktów ostrzeżenia – blokada na 60 minut<br>
<br>
<br><br>
<h3><span class="color-blue">Przeprowadzanie pojedynku</span></h3>• Postać gracza rozpoczyna walkę zawsze z pełnym poziomem zdrowia.<br>
• Bonus za przewagę poziomową jest wyłączony.<br>
• Przedmioty (również błogosławieństwo) gracza z niższym poziomem otrzymują wzmocnienie. Każdy przedmiot z osobna otrzymuje wzmocnienie - ich statystyki są zwiększone w taki sposób, jakby ich poziom został zwiększony o najmniejszą wartość z poniższych:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 100% różnicy poziomowej między przedmiotami, które są umieszczone w tych samych miejscach ekwipunku. Rękawice są porównywane z rękawicami, pierścienie z pierścieniami, bronie z broniami, bronie pomocnicze z broniami pomocniczymi (lub z bronią dwuręczną jeżeli przeciwnik ją posiada).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 100% różnicy poziomowej między postaciami - przedmiot nie może otrzymać wzrostu poziomu pozornego większego niż różnica poziomowa między walczącymi ze sobą postaciami.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<i>Przykład:</i><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Gracz A z poziomem 76 posiada rękawice na poziom 63, buty z poziomem 76 i naszyjnik z poziomem 76.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Gracz B z poziomem 83 posiada rękawice z poziomem 82, buty z poziomem 70 i naszyjnik z poziomem 80.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rękawice gracza A zostaną zwiększone o 7 poziomów do poziomu 70 (różnica w poziomach między graczami - górna granica wzmocnienia).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Buty gracza A nie zostaną zwiększone. Buty gracza B również nie zostaną zwiększone (ponieważ ma wyższy poziom).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Naszyjnik gracza A zostanie zwiększony o 4 poziomy do poziomu 80 (różnica w poziomach między przedmiotami).<br>
• Najpierw obliczany jest poziom przedmiotów wynikający z różnicy poziomowej (między graczami lub przedmiotami), a dopiero następnie względem niego obliczane jest ulepszenie przedmiotu.<br>
<i>Przykład:</i> Gracz z poziomem 80, posiadający zbroję na poziom 80 ulepszoną na +5 i walcząc z graczem na poziomie 90 posiadającym zbroję na poziomie 88, najpierw otrzymuje wzmocnienie do zbroi wynikające z różnicy poziomowej między zbrojami o 8 poziomów (tak jakby była na poziom 88), a następnie po obliczeniu statystyk po ulepszeniu (pojedyncze ulepszenie przedmiotu posiadającego poziom 88 zwiększa jego poziom pozorny o 3), jej statystyki zwiększane są względem poziomu 88 do poziomu 103.<br>
• Bonusy legendarne postaci, której poziom przewyższa 300, są obliczane w taki sposób, jakby poziom postaci wynosił 300. Włączone do tej zasady są również błogosławieństwa.<br>
• Czas oczekiwania na akcję gracza wynosi 5 sekund.<br>
• Podczas pojedynków, postać gracza występująca na mapie w grze jest chroniona przed wszelkimi interakcjami.<br>
• Podczas pojedynków nie można używać przedmiotów przerywających walkę.<br>
• Podczas pojedynków nie można używać przedmiotów leczących w trakcie walki.<br>
• Śmierć postaci w walce na Otchłani nie powoduje przejścia w stan nieprzytomności ani przeniesienia do najbliższej lokacji z ustawionym miejscem odrodzenia.<br>
• Śmierć postaci w walce na Otchłani na świecie Berufs nie powoduje utraty poziomu.<br>
<br>
<br><br>
<h3><span class="color-blue">Punktacja</span></h3>• Atrakcja Otchłani przewiduje dwa rodzaje punktacji:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Punkty Rankingowe, ustalające pozycję w rankingu oraz nagrody za koniec sezonu.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Punkty Progresu, których zbieranie umożliwi odblokowanie kolejnej Skrzyni oraz etapu w ramach dziennego postępu postaci.<br>
• Każda postać rozpoczyna sezon Otchłań z liczbą 1400 Punktów Rankingowych.<br>
• Przed umieszczeniem postaci w rankingu, musi ona stoczyć 10 meczy klasyfikacyjnych, podczas których odpowiednio modyfikowane są jej Punkty Rankingowe.<br>
• Zwycięstwo w walce powoduje odebranie przeciwnikowi Punktów Rankingowych, natomiast przegrana powoduje ich przekazanie przeciwnikowi. Remis nie powoduje żadnych zmian w punktacji.<br>
• Postać za zakończoną walkę może zyskać lub stracić:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 28 Punktów Rankingowych, gdy osiągnięto maksymalną różnicę w kryteriach: różnica Punktów Rankingowych, różnica poziomów postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 Punktów Rankingowych, gdy osiągnięto bardzo niewielką różnicę w kryteriach: różnica Punktów Rankingowych, różnica poziomów postaci.<br>
• Liczba uzyskanych lub straconych Punktów Rankingowych zależy od:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Pozycji przeciwnika w rankingu (100% wagi).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dawniej zależała również od poziomu przeciwnika - obecnie zależność ta jest wyłączona.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dawniej zależała również od różnicy w jakości ekwipunku między postaciami - obecnie zależność ta jest wyłączona.<br>
• Punktacja za walkę z postacią, której poziom przekracza 300, jest obliczana tak, jakby postać miała poziom 300.<br>
• Za wygraną walkę gracz otrzymuje 2 Punkty Progresu, za przegraną walkę otrzymuje 1 Punkt Progresu, natomiast za remis - 0.<br>
• Wynik remisu powoduje przyznanie Punktów ostrzeżenia obu postaciom toczącym walkę.<br>
• Poddanie walki powoduje natychmiastowe przegranie pojedynku, oddanie Punktów Rankingowych przeciwnikowi oraz brak otrzymania Punktów Progresu.<br>
• Pula nagród za zakończenie sezonu zwiększana jest o 1 za każdy remis w tabeli rankingowej podczas finalizacji rankingu Otchłani.<br>
<i>Przykład I</i>: Jeżeli dwóch graczy zasiada na pozycji #1, to obaj dostają tę samą nagrodą za ukończenie sezonu na pierwszym miejscu.<br>
<i>Przykład II</i>: Jeżeli na serwerze dostępnych jest 10 strojów po zakończeniu sezonu, ale liczba postaci na pozycjach 1-10 wynosi 12 na skutek remisów, to 12 postaci otrzymuje strój.<br>
• Gracze współdzielą pozycję w rankingu (na przykład dwóch graczy zajmuje pozycję #1) w przypadku gdy zostają spełniono kolejno następujące warunki:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Gracze posiadają tyle samo punktów rankingowych - gracz z większą liczbą punktów jest uznawany jako lepszy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Gracze posiadają tyle samo stoczonych walk (suma wygranych, przegranych i remisów) - gracz z większą liczbą walk uznawany jest jako lepszy.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. Gracze posiadają taki sam stosunek zwycięstw - gracz z wyższym stosunkiem zwycięstw jest uznawany jako lepszy.<br>
<i>Przykład I</i>: Gracz A ma 1400 punktów, 20 zwycięstw i 10 porażek. Gracz B ma 1400 punktów 20 zwycięstw i 5 porażek. Gracz A ma wyższą pozycję od gracza B, ponieważ ma więcej stoczonych walk.<br>
<i>Przykład II</i>: Gracz A ma 1400 punktów, 20 zwycięstw i 10 porażek. Gracz B ma 1400 punktów 10 zwycięstw i 20 porażek. Gracz A ma wyższą pozycję od gracza B, ponieważ ma większy stosunek zwycięstw mimo tej samej liczby stoczonych walk.<br>
<br>
<br>
<br>
<br><br>
<h3><span class="color-blue">Nagrody</span></h3>• Każda postać ma swój własny Progres składający się z czterech etapów, podczas którego ma możliwość odbierania skrzyń w zamian za skumulowane Punkty Progresu. Progres wraz ze wszystkimi etapami resetuje się każdego dnia o 5:25. Reset powoduje przywrócenie Progresu do stanu początkowego, a zatem zostaje utracona możliwość odebrania odblokowanych wcześniej Skrzyń.<br>
• Progres podzielony jest na 4 etapy. Każde zebrane 3 Punkty Progresu umożliwiają odebranie Skrzyni w ramach określonego etapu. Ukończenie etapu umożliwia odebranie unikatowej Skrzyni, a zakończenie wszystkich etapów umożliwia odebranie heroicznej Skrzyni.<br>
• Zawartość Skrzyń jest zależna od profesji i poziomu postaci. Skrzyń z Otchłani nie można przekładać przez depozyt ani nimi handlować. Po otworzeniu Skrzyni następuje przyznanie postaci jednego losowego przedmiotu, który jest związany na stałe, ale można go przenosić przez depozyt.<br>
• Skrzynie z Otchłani można wymieniać między profesjami u Materialisty Gverkosza znajdującego się w Gildii Teologów w mieście Thuzal. <b><a href="https://youtube.com/shorts/H3wu3bJMuik">Krótki film</a></b> omawiający proces wymiany Skrzyń z Otchłani.<br>
• Zawartość Skrzynki z Otchłani (możliwa do przejrzenia poprzez Podgląd przedmiotu):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 7 pospolitych przedmiotów: 75% szans<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 13 unikatowych przedmiotów: 25% szans<br>
• Zawartość Zdobionej skrzynki z Otchłani (możliwa do przejrzenia poprzez Podgląd przedmiotu):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 13 unikatowych przedmiotów: 75% szans<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 12 heroicznych przedmiotów: 24% szans<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 legendarne przedmioty (3 podczas Sezonu finałowego): 1% szans<br>
• Zawartość Krwawej skrzynki z Otchłani (możliwa do przejrzenia poprzez Podgląd przedmiotu):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 12 heroicznych przedmiotów: 96% szans<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 legendarne przedmioty (3 podczas Sezonu finałowego): 4% szans<br>
• Postacie, znajdujące się w pierwszych 10 pozycjach aktualnego rankingu Otchłani, są oznaczane specjalnymi elementami kosmetycznymi do momentu startu kolejnego sezonu:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ikona pucharu w dymku postaci na nowym interfejsie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Złote obramowanie dymku postaci na nowym interfejsie (postacie posiadające list gończy są wyłączone z tej mechaniki).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Tytuł <b>Czempion</b> na starym interfejsie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Złoty neon pod postacią (postacie posiadające list gończy są wyłączone z tej mechaniki).<br>
• Po zakończeniu sezonu Otchłani następuje finalizacja rankingu, czyli przyznawanie nagród zwycięzcom:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsce 1: 100 (150 podczas Sezonu finałowego) Kryształów Czempionów, Kufer arcymistrza, Legendarna pamiątka (Kamień teleportacyjny lub Maskotka)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 2-3: 100 (130 podczas Sezonu finałowego) Kryształów Czempionów, Kufer arcymistrza<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 4-10: 80 (100 podczas Sezonu finałowego) Kryształów Czempionów, Kufer mistrza<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 11-20: 50 (65 podczas Sezonu finałowego) Kryształów Czempionów, Kufer pretendenta<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 21-50: 25 (35 podczas Sezonu finałowego) Kryształów Czempionów<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 51-100: 15 (20 podczas Sezonu finałowego) Kryształów Czempionów<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 101-180: 10 (15 podczas Sezonu finałowego) Kryształów Czempionów<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Miejsca 181-300: 0 (10 podczas Sezonu finałowego) Kryształów Czempionów<br>
• Kryształy Czempionów służą do zakupu nagród z oferty Sklepu Czempionów dostępnego poprzez moduł Otchłani.<br>
• Kryształy Czempionów nie mają limitu przydatności - można je wykorzystać podczas kolejnych sezonów Otchłani.<br>
• Podczas sezonu finałowego, do puli nagród trafiają legendarne stroje za każde 50 postaci biorących udział w Otchłani. Liczba strojów minimalnie wynosi 1, a maksymalnie 10. Stroje są przyznawane kolejnych pozycji w Otchłani - w przypadku remisów, otrzymują go wszyscy gracze na tej samej pozycji.<br>
<i>Przykład</i>: W Otchłani bierze udział 201 postaci, zatem dostępnych w puli jest 5 strojów. Pierwsze 5 postaci w rankingu otrzymuje przedmiot podczas finalizowania rankingu, niezależnie od liczby remisów na pozycjach.<br>
<br>
<br><br>
<a name="k42"></a><b><h3>4.2. Krwawa Łaźnia</h3></b><br>
Krwawa łaźnia jest cykliczną atrakcją, polegającą na wprowadzaniu na zamkniętą lokację z wymuszonym włączonym trybem PvP (na każdym serwerze niezależnie od ustawień). Gracz ma tylko jedną możliwość wkroczenia na mapę - wyteleportowanie się z niej lub śmierć, powoduje powrót do najbliższego miasta. Atrakcja kończy się w momencie, gdy na mapie pozostanie tylko jeden gracz oraz zakończy się czas wprowadzania graczy na mapę - w tym przypadku gracz powinien porozmawiać z NPC wypuszczającym z mapy i odebrać u niego nagrodę za pokonanie przeciwników. Odebranie nagrody możliwe jest najwcześniej 6 minut po zakończeniu wprowadzania graczy na mapę.<br>
<br>
<h3><span class="color-blue">Parametry mapy</span></h3>• Grupowanie między graczami jest wyłączone.<br>
• Bezwarunkowe PvP jest włączone (również na światach non-PvP).<br>
• Bonus za przewagę poziomową jest wyłączony.<br>
<b><a href="https://youtube.com/shorts/m3skFJ1I8j0">Krótki film</a></b> przedstawiający miejsca, w których można szukać informacji o parametrach mapy.<br>
<br>
<h3><span class="color-blue">Spis Krwawych Łaźni</span></h3><b>Werbin</b><br>
• Zakres poziomowy: 30-40<br>
• NPC wprowadzający na mapę: Harib (5,63)<br>
• Termin walk: środa, 20:00-20:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 500 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 500k złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Werbin)<br>
<br>
<b>Torneg</b><br>
• Zakres poziomowy: 41-59<br>
• NPC wprowadzający na mapę: Badur (93,23)<br>
• Termin walk: wtorek, 20:00-20:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 700 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 700k złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Torneg)<br>
<br>
<b>Thuzal</b><br>
• Zakres poziomowy: 70-85<br>
• NPC wprowadzający na mapę: Zekos (26,20)<br>
• Termin walk: piątek, 21:00-21:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1000 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Thuzal)<br>
<br>
<b>Mythar</b><br>
• Zakres poziomowy: 100-120<br>
• NPC wprowadzający na mapę: Tristen (34,38)<br>
• Termin walk: sobota, 19:00-19:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1300 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Mythar)<br>
<br>
<b>Eder</b><br>
• Zakres poziomowy: 130-150<br>
• NPC wprowadzający na mapę: Silvius (1,60)<br>
• Termin walk: poniedziałek, 19:00-19:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1600 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 3m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Eder)<br>
<br>
<b>Karka-han</b><br>
• Zakres poziomowy: 160-180<br>
• NPC wprowadzający na mapę: Evril (71,53)<br>
• Termin walk: czwartek, 18:00-18:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1900 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 4m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Karka-han)<br>
<br>
<b>Nithal</b><br>
• Zakres poziomowy: 190-210<br>
• NPC wprowadzający na mapę: Korim (52,9)<br>
• Termin walk: wtorek, 18:00-18:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2400 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 5m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Nithal)<br>
<br>
<b>Tuzmer</b><br>
• Zakres poziomowy: 215-245<br>
• NPC wprowadzający na mapę: Nivelan (73,30)<br>
• Termin walk: sobota, 20:00-20:30<br>
• Nagrody:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2800 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 6m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Tuzmer)<br>
<br>
<b>Port Tuzmer</b><br>
• Zakres poziomowy: 250-280<br>
• NPC wprowadzający na mapę: Zlatko (6,43)<br>
• Termin walk: niedziela, 18:00-18:30<br>
• Nagrody: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 3200 Punktów Honoru<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 7m złota<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ błogosławieństwo (Błogosławieństwo rzeźnika)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ trofeum (Rzeźnik z Portu Tuzmer)<br>
<br>
<br><br>
<a name="k43"></a><b><h3>4.3. Krwawa Kopalnia</h3></b><br>
Krwawa Kopalnia jest cykliczną atrakcją, polegającą na wprowadzaniu na zamkniętą lokację z wymuszonym włączonym trybem PvP (na każdym serwerze niezależnie od ustawień). Gracz ma wiele możliwości wkroczenia na mapę. Atrakcja rozpoczyna się i kończy w określonych porach - tylko w tym czasie odpowiedni NPC może wprowadzić gracza na mapę. Po zakończeniu wydarzenia, gracz zostaje wyteleportowany z mapy. Podczas wydarzenia, gracz może wydobywać złoża, z których tworzy się w odpowiednim barterze przedmioty.<br>
<br>
<h3><span class="color-blue">Opis atrakcji</span></h3>Na zamkniętej mapie z bezwarunkowym PvP znajdują się złoża, które gracz może wydobywać przy użyciu specjalnego przedmiotu odnawiającego się na mapie (na przykład kilofa). Rudy złóż posłużą do tworzenia ekskluzywnych przedmiotów w barterze postaci niezależnej wprowadzającej na mapę. Kilof po użyciu ulega zniszczeniu. Postacie eksplorujące mapę mogą być poddane losowym zdarzeniom, które wpływają na ich stan. Ponadto na lokacji występuje elita III - potwór z silnymi statystykami, z którego można zdobyć ekskluzywne przedmioty.<br>
<br>
<h3><span class="color-blue">Parametry mapy</span></h3>• Grupowanie między graczami jest wyłączone.<br>
• Resetowanie poziomu na świecie Berufs jest wyłączone.<br>
• Bezwarunkowe PvP jest włączone (również na światach non-PvP).<br>
• Czas oczekiwania na turę gracza jest skrócony do 3 sekund (1 sekunda na mapie-pułapce).<br>
• Gracze zostają wyteleportowani z mapy przy pierwszym kontakcie z obiektami poza godzinami funkcjonowania atrakcji lub w momencie gdy ich postać nie posiada odpowiedniego poziomu.<br>
• Czas na wykonanie wszystkich tur wynosi 60 sekund (zamiast 120 sekund).<br>
• Minimalny czas trwania tury w trybie przyspieszonym wynosi 0 sekund (zamiast 2 sekund).<br>
• Czas odrodzenia obiektów jest zależny od ustawień serwera.<br>
<b><a href="https://youtube.com/shorts/m3skFJ1I8j0">Krótki film</a></b> przedstawiający miejsca, w których można szukać informacji o parametrach mapy.<br>
<br>
<h3><span class="color-blue">Dodatkowe uwagi</span></h3>• Krwawe Kopalnie mogą być nieczynne podczas wydarzenia Otchłani. Przez okres równy czasowi nieaktywności Krwawej Kopalni, szansa na przedmiot unikatowy, heroiczny i legendarny jest dwukrotnie większa (kosztem szansy na przedmiot pospolity) po zakończeniu sezonu Otchłani.<br>
• Po wprowadzeniu Krwawej Kopalni do gry, ma ona zwiększoną szansę na przedmioty unikatowe, heroiczne i legendarne dwukrotnie przez 2 tygodnie (2 wystąpienia wydarzenia).<br>
• Przedmioty specjalne - klucze, skrzynie i kilofy, są usuwane podczas pierwszego wejścia na Kopalnię w danym tygodniu.<br>
<br>
<h3><span class="color-blue">Spis Krwawych Kopalni</span></h3><a name="kk43"></a><br>
<b>Kopalnia Krwawej Zemsty</b><br>
• <b><a href="https://www.youtube.com/watch?v=ixAwimxjpnA">Film</a></b> prezentujący atrakcję.<br>
• Wejście na mapę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać: Przemytnik Wilgrim (Wilcza Nora p.1 18,4).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Godziny wstępu: 20:00 - 21:00.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dzień tygodnia: sobota.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymagany poziom doświadczenia postaci: 36-43.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czas oczekiwania przed ponownym wejściem na mapę: 10 minut.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba losowych miejsc wprowadzenia postaci na mapę: 20.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba kilofów ustawiania w ekwipunku postaci po pierwszym wejściu na mapę: 5.<br>
• Obiekty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 3 miejscach złóż o czasie odrodzenia 1.5min - 4.5min. Typ: elita.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 2 miejscach kilofów o czasie odrodzenia 1.5min - 4.5min. Typ: odnawialne.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 11 obiektów wyzwalających w promieniu 12 kratek zdarzenia (teleportacja, unieruchomienie, zranienie, klucz, informacja o mapie) losowo co 3 minuty. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 obiekt wyzwalający w promieniu całej mapy zdarzenie raz na 4 minuty, wprowadzający parę graczy do mapy-pułapki (w przypadku, gdy na mapie jest więcej niż 5 graczy). Samotny gracz wewnątrz pułapki może odebrać przedmiot oferujący 5 losowań szablonu zdobyczy złóż. Wewnątrz pułapki brak aktywności przez 138 sekund kończy się śmiercią postaci. Wewnątrz pułapki czas oczekiwania na turę gracza wynosi 1 sekundę i wyłączona jest możliwość teleportacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 losowo odradzające się w 3 miejscach skrzynie o czasie odrodzenia 2min - 6min. Skrzynie otwierać można kluczem pozyskanym ze zdarzeń. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 losowo odradzający się w 6 miejscach kamień blokujący drogę, ginący automatycznie po 30 sekundach. Typ: obiekt statyczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 9 potworów ze standarowym szablonem przedmiotów. Typ: potwór.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Tarmus Wuden z poziomem 43 losowo odradzająca się w 10 miejscach o czasie odrodzenia 6min - 18min. Typ: elita III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 7 indywidualnych dla gracza par tuneli teleportujących między sobą co 3 minuty każda. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Tunel losowo teleportujący w centralną część mapy lub unieruchamiający postać gracza. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wyjście z mapy umieszczone w jej centralnej części (34,19). Typ: postać niezależna.<br>
• Przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wydobyte surowce nie są związane z właścicielem, można nimi handlować, wystawiać na aukcję i przechowywać w depozycie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kilofy są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Klucze są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Duża torba z narzędziami jest permanentnie związane z właścicielem. Oferuje ona od 6 do 8 losowań: kilofy, pospolite odłamki, unikatowe odłamki i heroiczne odłamki. Nie można jej przechowywać w depozycie. Jest zabierana postaci przed pierwszym wejściem do lokacji danego dnia. Po 5 dniach skrzynia traci moc i nie można jej otworzyć.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Pokaźnego Złoża zawiera: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ pusty łup: 15%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 pospolity surowiec: 49.5%, <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 unikatowy surowiec: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 heroiczny surowiec: 10%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 legendarny surowiec: 0.5%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Barter Przemytnika Wilgrima zawiera: 1 pospolity teleport, 6 unikatowych zbroi, 6 heroicznych broni, 4 legendarne naszyjniki.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Tarmusa Wudena zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 4 przedmioty unikatowe: 70%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3 przedmioty heroiczne: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 2 przedmioty legendarne: 5%.<br>
• Informacje dodatkowe:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Bonus za przewagę poziomową jest włączony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po przegranej walce gracz odradza się w Eder.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szmugler Beniamin (Eder 13,55) przenosi postacie o dozwolonym poziomie w godzinach od 19:50 do 21:00 na mapę Wilcza Nora p.1.<br>
<br>
<a name="kk64"></a><br>
<b>Kopalnia Krwawego Szaleństwa</b><br>
• <b><a href="https://www.youtube.com/watch?v=LYUAsjj6L1A">Film</a></b> prezentujący atrakcję.<br>
• Wejście na mapę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać: Dirakos (Mroczna Pieczara p.0 10,4).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Godziny wstępu: 20:00 - 21:00.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dzień tygodnia: piątek.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymagany poziom doświadczenia postaci: 57-64.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czas oczekiwania przed ponownym wejściem na mapę: 10 minut.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba losowych miejsc wprowadzenia postaci na mapę: 20.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba kilofów ustawiania w ekwipunku postaci po pierwszym wejściu na mapę: 5.<br>
• Obiekty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 3 miejscach złóż o czasie odrodzenia 1.5min - 4.5min. Typ: elita.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 2 miejscach kilofów o czasie odrodzenia 1.5min - 4.5min. Typ: odnawialne.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 obiektów wyzwalających w promieniu 12 kratek zdarzenia (teleportacja, unieruchomienie, zranienie, klucz, informacja o mapie) losowo co 1-2 minuty. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 obiekt wyzwalający w promieniu całej mapy zdarzenie raz na 4 minuty, wprowadzający parę graczy do mapy-pułapki (w przypadku, gdy na mapie jest więcej niż 5 graczy). Samotny gracz wewnątrz pułapki może odebrać przedmiot oferujący 5 losowań szablonu zdobyczy złóż. Wewnątrz pułapki brak aktywności przez 138 sekund kończy się śmiercią postaci. Wewnątrz pułapki czas oczekiwania na turę gracza wynosi 1 sekundę i wyłączona jest możliwość teleportacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 losowo odradzające się w 3 miejscach skrzynie o czasie odrodzenia 2min - 6min. Skrzynie otwierać można kluczem pozyskanym ze zdarzeń losowych. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 losowo odradzający się w 6 miejscach kamień blokujący drogę, ginący automatycznie po 30 sekundach. Typ: obiekt statyczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 potworów z niestandardowym szablonem przedmiotów. Typ: potwór.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Vonaros z poziomem 64 losowo odradzający się w 10 miejscach o czasie odrodzenia 6min - 18min. Typ: elita III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 6 indywidualnych dla gracza par tuneli teleportujących między sobą co 3 minuty każda. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Tunel losowo teleportujący na 3 koordynaty ze wspólnym czasem odnowienia dla wszystkich graczy wynoszącym 15 sekund. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wyjście z mapy umieszczone w jej środkowej części (37,26). Typ: postać niezależna.<br>
• Przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wydobyte surowce nie są związane z właścicielem, można nimi handlować, wystawiać na aukcję i przechowywać w depozycie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kilofy są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Klucze są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zdradliwa skrzynia jest permanentnie związana z właścicielem. Oferuje ona od 6 do 8 losowań: kilofy, pospolite odłamki, unikatowe odłamki i heroiczne odłamki. Nie można jej przechowywać w depozycie. Jest zabierana postaci przed pierwszym wejściem do lokacji danego dnia. Po 5 dniach skrzynia traci moc i nie można jej otworzyć.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Naładowanego kryształu zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ pusty łup: 15%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 pospolity surowiec: 49.5%, <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 unikatowy surowiec: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 heroiczny surowiec: 10%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 legendarny surowiec: 0.5%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Barter Dirakosa zawiera: 1 pospolity teleport, 6 unikatowych naszyjników, 6 heroicznych broni pomocniczych, 1 heroiczny pierścień, 6 legendarnych par butów, 1 legendarny naszyjnik.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Vonarosa zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 5 przedmiotów unikatowych: 70%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 5 przedmiotów heroicznych: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 2 przedmioty legendarne: 5%.<br>
• Informacje dodatkowe:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Bonus za przewagę poziomową jest wyłączony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po przegranej walce gracz odradza się w Ithan<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ciosy Naładowanych grzechotników zawsze zabijają postać.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przesiadywanie wewnątrz mapy-pułapki przez dłuższy czas powoduje zabicie postaci.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Istnieje szansa, że tylko jeden gracz zostanie umieszczony w mapie-pułapce.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Adept Ceranir (Ithan 54,55) przenosi postacie o dozwolonym poziomie w godzinach od 19:50 do 21:00 na mapę Mroczna Pieczara p.0.<br>
<br>
<a name="kk83"></a><br>
<b>Kopalnia Krwawego Opętania</b><br>
• Wejście na mapę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać wprowadzająca na przedsionek: Poprzewracane Książki (Biblioteka Andarum 21,3).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać teleportująca na przedsionek oraz oferująca barter: Mnich Damien (Ithan -&gt; Pod Rozbrykanym Niziołkiem 7,7).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Godziny wstępu: 20:00 - 21:00.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dzień tygodnia: środa.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymagany poziom doświadczenia postaci: 76-83.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czas oczekiwania przed ponownym wejściem na mapę: 10 minut.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba losowych miejsc wprowadzenia postaci na mapę: 20.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba kilofów ustawiania w ekwipunku postaci po pierwszym wejściu na mapę: 5.<br>
• Obiekty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 3 miejscach złóż o czasie odrodzenia 1.5min - 4.5min. Typ: elita.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 2 miejscach kilofów o czasie odrodzenia 1.5min - 4.5min. Typ: odnawialne.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 obiektów wyzwalających w promieniu 12 kratek zdarzenia (teleportacja, unieruchomienie, zranienie, klucz, informacja o mapie) losowo co 1-2 minuty. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 obiekt wyzwalający w promieniu całej mapy zdarzenie raz na 4 minuty, wprowadzający parę graczy do mapy-pułapki (w przypadku, gdy na mapie jest więcej niż 5 graczy). Samotny gracz wewnątrz pułapki może odebrać przedmiot oferujący 5 losowań szablonu zdobyczy złóż. Wewnątrz pułapki brak aktywności przez 138 sekund kończy się śmiercią postaci. Wewnątrz pułapki czas oczekiwania na turę gracza wynosi 1 sekundę i wyłączona jest możliwość teleportacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 losowo odradzające się w 3 miejscach skrzynie o czasie odrodzenia 2min - 6min. Skrzynie otwierać można kluczem pozyskanym ze zdarzeń. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 losowo odradzający się w 6 miejscach kamień blokujący drogę, ginący automatycznie po 30 sekundach. Typ: obiekt statyczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 potworów z niestandardowym szablonem przedmiotów. Typ: potwór.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wyznawca Ciemnych Mocy z poziomem 83 losowo odradzająca się w 10 miejscach o czasie odrodzenia 6min - 18min. Typ: elita III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 7 indywidualnych dla gracza par tuneli teleportujących między sobą co 3 minuty każda. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wyjście z mapy umieszczone w jej centralnej części (34,21). Typ: postać niezależna.<br>
• Przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wydobyte surowce nie są związane z właścicielem, można nimi handlować, wystawiać na aukcję i przechowywać w depozycie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kilofy są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Klucze są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Świątynna skrzynia jest permanentnie związana z właścicielem. Oferuje on od 6 do 8 losowań: kilofy, pospolite odłamki, unikatowe odłamki i heroiczne odłamki. Nie można go przechowywać w depozycie. Jest zabierana postaci przed pierwszym wejściem do lokacji danego dnia. Po 5 dniach skrzynia traci moc i nie można jej otworzyć.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Błękitnego złoża zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ pusty łup: 15%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 pospolity surowiec: 49.5%, <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 unikatowy surowiec: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 heroiczny surowiec: 10%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 legendarny surowiec: 0.5%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Barter Mnicha Damiena zawiera: 1 pospolity teleport, 6 unikatowych broni, 6 heroicznych broni pomocniczych, 1 heroiczny pierścień, 6 legendarnych par rękawic.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Wyznawcy Ciemnych Mocy zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 4 przedmioty unikatowe: 70%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3 przedmioty heroiczne: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3 przedmioty legendarne: 5%.<br>
• Informacje dodatkowe:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Bonus za przewagę poziomową jest wyłączony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po przegranej walce gracz odradza się w Ithan.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ciosy Opętanych mnichów zawsze zabijają postać.<br>
<br>
<a name="kk114"></a><br>
<b>Kopalnia Krwawej Arogancji</b><br>
• Wejście na mapę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać wprowadzająca na przedsionek: Grobowiec Zapomnianych (Płaskowyż Arpan 83,48).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać teleportująca na przedsionek oraz oferująca barter: Archeolog Bunar (Tuzmer 67,3).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Godziny wstępu: 20:00 - 21:00.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dzień tygodnia: czwartek.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymagany poziom doświadczenia postaci: 107-114.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czas oczekiwania przed ponownym wejściem na mapę: 10 minut.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba losowych miejsc wprowadzenia postaci na mapę: 20.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba kilofów ustawiania w ekwipunku postaci po pierwszym wejściu na mapę: 5.<br>
• Obiekty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 3 miejscach złóż o czasie odrodzenia 1.5min - 4.5min. Typ: elita.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 15 losowo odradzających się w 2 miejscach kilofów o czasie odrodzenia 1.5min - 4.5min. Typ: odnawialne.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 obiektów wyzwalających w promieniu 12 kratek zdarzenia (teleportacja, unieruchomienie, zranienie, klucz, informacja o mapie) losowo co 1-2 minuty. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 obiekt wyzwalający w promieniu całej mapy zdarzenie raz na 4 minuty, wprowadzający parę graczy do mapy-pułapki (w przypadku, gdy na mapie jest więcej niż 5 graczy). Samotny gracz wewnątrz pułapki może odebrać przedmiot oferujący 5 losowań szablonu zdobyczy złóż. Wewnątrz pułapki brak aktywności przez 138 sekund kończy się śmiercią postaci. Wewnątrz pułapki czas oczekiwania na turę gracza wynosi 1 sekundę i wyłączona jest możliwość teleportacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 losowo odradzające się w 3 miejscach skrzynie o czasie odrodzenia 2min - 6min. Skrzynie otwierać można kluczem pozyskanym ze zdarzeń. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 losowo odradzający się w 6 miejscach kamień blokujący drogę, ginący automatycznie po 30 sekundach. Typ: obiekt statyczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 potworów z niestandardowym szablonem przedmiotów. Typ: potwór.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szkielet Władcy Żywiołów z poziomem 83 losowo odradzająca się w 10 miejscach o czasie odrodzenia 6min - 18min. Typ: elita III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 8 współdzielonych między graczami par tuneli teleportujących między sobą co 30 sekund każda. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Tunel losowo teleportujący w centralną część mapy lub unieruchamiający postać gracza. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wyjście z mapy umieszczone w jej zachodniej części (17,25). Typ: postać niezależna.<br>
• Przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wydobyte surowce nie są związane z właścicielem, można nimi handlować, wystawiać na aukcję i przechowywać w depozycie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kilofy są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Klucze są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Świątynna skrzynia jest permanentnie związana z właścicielem. Oferuje on od 6 do 8 losowań: kilofy, pospolite odłamki, unikatowe odłamki i heroiczne odłamki. Nie można go przechowywać w depozycie. Jest zabierana postaci przed pierwszym wejściem do lokacji danego dnia. Po 5 dniach skrzynia traci moc i nie można jej otworzyć.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablony Niewydobytego minerału oraz Sterty kości zawierają:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ pusty łup: 15%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 pospolity surowiec: 49.5%, <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 unikatowy surowiec: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 heroiczny surowiec: 10%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 legendarny surowiec: 0.5%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Barter Archeologa Bunara zawiera: 1 pospolity teleport, 6 unikatowych broni, 6 heroicznych broni pomocniczych, 1 heroiczna para butów, 6 legendarnych hełmów.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Szkieletu Władcy Żywiołów zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 5 przedmiotów unikatowych: 70%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 5 przedmiotów heroicznych: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3 przedmioty legendarne: 5%.<br>
• Informacje dodatkowe:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Bonus za przewagę poziomową jest wyłączony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po przegranej walce gracz odradza się w Tuzmer.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ciosy Zakopanych żołnierzy zawsze zabijają postać.<br>
<br>
<a name="kk300"></a><br>
<b>Kopalnia Krwawej Pychy</b><br>
• <b><a href="https://www.youtube.com/watch?v=81EJyTEPyvI">Film</a></b> prezentujący atrakcję.<br>
• Wejście na mapę:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Postać: Desa Florentyna (Thuzal 88,7).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Godziny wstępu: 20:00 - 21:00.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Dzień tygodnia: niedziela.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wymagany poziom doświadczenia postaci: 300-500.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czas oczekiwania przed ponownym wejściem na mapę: 10 minut.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba losowych miejsc wprowadzenia postaci na mapę: 20.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Liczba kilofów ustawiania w ekwipunku postaci po pierwszym wejściu na mapę: 5.<br>
• Obiekty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 12 losowo odradzających się w 3 miejscach złóż o czasie odrodzenia 1.5min - 4.5min. Typ: elita.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 12 losowo odradzających się w 2 miejscach kilofów o czasie odrodzenia 1.5min - 4.5min. Typ: odnawialne.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 10 obiektów wyzwalających w promieniu 12 kratek zdarzenia (teleportacja, unieruchomienie, zranienie, klucz, informacja o mapie) losowo co 1-2 minuty. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 obiekt wyzwalający w promieniu całej mapy zdarzenie raz na 4 minuty, wprowadzający parę graczy do mapy-pułapki (w przypadku, gdy na mapie jest więcej niż 5 graczy). Samotny gracz wewnątrz pułapki może odebrać przedmiot oferujący 5 losowań szablonu zdobyczy złóż. Wewnątrz pułapki brak aktywności przez 138 sekund kończy się śmiercią postaci. Wewnątrz pułapki czas oczekiwania na turę gracza wynosi 1 sekundę i wyłączona jest możliwość teleportacji.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 2 losowo odradzające się w 3 miejscach skrzynie o czasie odrodzenia 2min - 6min. Skrzynie otwierać można kluczem pozyskanym ze zdarzeń. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 1 losowo odradzający się w 6 miejscach kamień blokujący drogę, ginący automatycznie po 30 sekundach. Typ: obiekt statyczny.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 11 potworów z niestandardowym szablonem przedmiotów. Typ: potwór.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Erktos z poziomem 300 losowo odradzająca się w 10 miejscach o czasie odrodzenia 6min - 18min. Typ: elita III.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ 7 indywidualnych dla gracza par tuneli teleportujących między sobą co 3 minuty każda. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Tunel losowo teleportujący w centralną część mapy lub unieruchamiający postać gracza. Typ: postać niezależna.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wyjście z mapy umieszczone w jej górnej części (32,15). Typ: postać niezależna.<br>
• Przedmioty:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Wydobyte surowce nie są związane z właścicielem, można nimi handlować, wystawiać na aukcję i przechowywać w depozycie.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kilofy są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Klucze są permanentnie związane z właścicielem i nie można ich przechowywać w depozycie. Są odbierane postaci przed pierwszym wejściem do lokacji danego dnia.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Drżący kuferek jest permanentnie związany z właścicielem. Oferuje on od 6 do 8 losowań: kilofy, pospolite odłamki, unikatowe odłamki i heroiczne odłamki. Nie można go przechowywać w depozycie. Jest zabierana postaci przed pierwszym wejściem do lokacji danego dnia. Po 5 dniach skrzynia traci moc i nie można jej otworzyć.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Zamrożonego czarodzieja zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ pusty łup: 15%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 pospolity surowiec: 49.6%, <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 unikatowy surowiec: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 heroiczny surowiec: 10%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1 legendarny surowiec: 0.4%.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Barter Desy Florentyny zawiera: 1 pospolity teleport, 6 unikatowych zbroi, 6 heroicznych broni, 6 legendarnych broni pomocniczych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Szablon Erktosa zawiera:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 4 przedmioty unikatowe: 70%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 4 przedmioty heroiczne: 25%,<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3 przedmioty legendarne: 5%.<br>
• Informacje dodatkowe:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Bonus za przewagę poziomową jest wyłączony.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po przegranej walce gracz odradza się w Thuzal.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Ciosy Mrożących mykonidów zawsze zabijają postać.<br>
<br>
<br><br>
<a name="k44"></a><b><h3>4.4. Walki przeciw potworom</h3></b><br>
Część potworów jest specjalnie przygotowywana w celu stawiania wyzwań graczom. Do takich atrakcji należą:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Kolosi - potężne potwory, znajdujące się na mapie typu Próba Sił, przeznaczene do walk grupowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Tytani - najsilniejsze potwory, posiadające najdłuższy czas odrodzenia oraz najsilniejsze przedmioty, przeznaczone do walk grupowych.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Elity III - silne potwory występujące na specjalnych atrakcjach (instancja lub Krwawa kopalnia), przeznaczone do walki w pojedynkę.<br>
<br>
Każda profesja posiada umiejętności dedykowane walkom grupowym, które odpowiadają za wzmacnianie sojuszników lub osłabianie przeciwników. Stosuje się je zarówno do walk grupowych przeciw silnym potworom, jak i dużych walk grupowych między pełnymi drużynami graczy.<br>
• <b><a href="https://youtube.com/shorts/4irfJn4Ok9g">Krótki film</a></b> opisujący umiejętności do walk grupowych <b>Maga</b>.<br>
• <b><a href="https://youtube.com/shorts/6QVxAtTNIdI">Krótki film</a></b> opisujący umiejętności do walk grupowych <b>Paladyna</b>.<br>
• <b><a href="https://youtube.com/shorts/PVb8iyo0cmo">Krótki film</a></b> opisujący umiejętności do walk grupowych <b>Wojownika</b>.<br>
• <b><a href="https://youtube.com/shorts/1ZoD2kUglCg">Krótki film</a></b> opisujący umiejętności do walk grupowych <b>Tropiciela</b>.<br>
• <b><a href="https://youtube.com/shorts/Gz8g8bqeHxs">Krótki film</a></b> opisujący umiejętności do walk grupowych <b>Łowcy</b>.<br>
• <b><a href="https://youtube.com/shorts/0MP6mrmwgWY">Krótki film</a></b> opisujący umiejętności do walk grupowych <b>Tancerza ostrzy</b>.<br>
<br>
<br>
Dodatkowym specjalnym typem potwora jest elita II zamknięta na mapie, na której niemożliwe jest grupowanie się z innymi graczami. Pojedynki przeprowadzane na tej lokacji zawsze przebiegają między samotnie walczącymi graczami.<br>
<b><a href="https://youtube.com/shorts/ZpqloRHMYu4">Krótki film</a></b> omawiający działanie elit II na mapie z wyłączonym grupowaniem.<br>
<br>
<h3><span class="color-blue">Elity III</span></h3>Elity III są wzmocnionymi potworami przeznaczonymi do walk w pojedynkę. Atrakcja ta posiada następujące właściwości:<br>
• Z Elity III nigdy nie może wylosować się więcej niż jedna zdobycz.<br>
• Podczas niektórych wydarzeń (eventów), istnieje możliwość uczestnictwa w walkach z elitami III, posiadającymi jeden z trzech poziomów trudności - normalny, trudny, mistrzowski. Poziom takiej Elity III jest dopasowany do poziomu gracza.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Elita III z poziomem trudnym posiada szablon zdobyczy z szansą o 50% wyższą na zdobycie przedmiotu heroicznego oraz legendarnego względem elity z poziomem normalnym.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Elita III z poziomem mistrzowskim posiada szablon zdobyczy z szansą o 100% wyższą na zdobycie przedmiotu heroicznego oraz legendarnego względem elity z poziomem normalnym.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Elity III występujące w nieregularnej treści gry, zawsze posiadają personalne rozdzielanie łupu.<br>
<br>
<h3><span class="color-blue">Kolosi</span></h3>Kolosi są potworami tym silniejszymi im mniejsza jest grupa graczy biorących udział w walce. Dostępni są na mapie o typie <i>Próba Sił</i>. Atrakcja ta posiada następujące właściwości:<br>
• Mapa jest instancją przypisaną do dowódcy drużyny.<br>
• Pokonanie kolosa uniemożliwia dalsze wzięcie udziału w instancji (dowolnego innego kolosa z treści regularnej gry) w trakcie danego dnia. Można jednak zdobyć specjalne przedmioty, które umożliwiają ponowne stoczenie Próby Sił (zresetowanie instancji).<br>
• Reset instancji następuje o 5:25 każdego dnia.<br>
• Po rozwiązaniu drużyny wszyscy gracze będący w jej składzie opuszczają mapę.<br>
• Każdy gracz, którego poziom mieści się w granicach uczestnictwa w atrakcji, może wygenerować własnego kolosa lub wziąć udział we wspólnej Próbie sił, dołączając do drużyny innego gracza.<br>
• Z kolosa obowiązuje personalne rozdzielenie łupu.<br>
• Przedsionki przed mapami kolosów mają wyłączony tryb PvP.<br>
• Ustawienia mapy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Możliwość wejścia przez postacie posiadające co najwyżej 14 poziomów mniej od kolosa oraz co najwyżej 25 poziomów więcej od kolosa.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zablokowana walka PvP.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Zablokowana teleportacja.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po śmierci postaci odradza się ona w przedsionku przed mapą kolosa.<br>
• Podczas niektórych wydarzeń (eventów), istnieje możliwość uczestnictwa w walkach z kolosami, posiadającymi jeden z trzech poziomów trudności - normalny, trudny, mistrzowski. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kolos z poziomem trudnym posiada szablon zdobyczy z szansą o 50% wyższą na zdobycie przedmiotu heroicznego oraz legendarnego względem kolosa z poziomem normalnym.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Kolos z poziomem mistrzowskim posiada szablon zdobyczy z szansą o 100% wyższą na zdobycie przedmiotu heroicznego oraz legendarnego względem kolosa z poziomem normalnym.<br>
• Pierwsze wejście na kolosa w przeciągu dnia (doby zaczynającej się o 5:25) powoduje przeteleportowanie się tuż pod pozycję kolosa. <b><a href="https://youtube.com/shorts/djzJJXCiyNM">Krótki film</a></b> omawiający działanie Mechanizmu wprowadzania na mapę.<br>
• <b><a href="https://youtube.com/shorts/cjgFpbCrpAc">Krótki film</a></b> omawiający wymianę zwojów teleportacyjnych z kolosów.<br>
<br>
<h3><span class="color-blue">Tytani</span></h3>Tytani są wzmocnionymi potworami przeznaczonymi do walk w pełnej drużynie. Atrakcja ta posiada następujące właściwości:<br>
• Czas odrodzenia tytana zależy od jego poziomu i jest dłuższy od doby na serwerach bez skróconego czasu odrodzenia NPC.<br>
• Przedmioty dostępne z tytana mają dodatkowy bonus typu nagroda.<br>
• Tytani zawsze mają włączone wiele losowań łupów niezależnie od różnicy poziomów członków drużyny. Oznacza to, że po pokonaniu potwora liczba zdobytych przedmiotów może wynosić nawet 6, mimo bardzo dużej różnicy poziomów graczy.<br>
• Ustawienia mapy:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Możliwość wejścia przez postacie posiadające co najwyżej 13 poziomów mniej od tytana (dotyczy wszystkich tytanów) oraz co najwyżej 13 poziomów więcej od tytana (dotyczy tylko tytanów z poziomem niższym od 285).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Bezwarunkowa walka PvP.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Po śmierci postaci odradza się ona w przedsionku przed mapą tytana.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Czas na wykonanie wszystkich tur wynosi 100 sekund (zamiast 120).<br>
• Przed mapami tytanów znajdują się przedsionki ze specjalnymi ustawieniami mapy. <b><a href="https://youtube.com/shorts/mPbkHRFPEMM">Krótki film</a></b> omawiający zasady działania przedsionków przed mapami z tytanami.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przedsionki przed mapami tytanów, którzy posiadają poziom niższy od 285, są zablokowane poziomowo do poziomu o 13 wyższego od poziomu tytana.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Przedsionki przed mapami tytanów, którzy posiadają poziom niższy od 150, mają wyłączony tryb PvP.<br>
<br>
<br><br>
<a name="k45"></a><b><h3>4.5. Niuanse związane z elitami II</h3></b><br>
Poniżej zestawiony został zbiór mechanik, jakimi charakteryzuje się potwór - elita II.<br>
• Elity II zawsze posiadają rozrzut koordynatów wynoszący od 2 do 10 kratek od miejsca ich domyślnego położenia. Rozrzut jest ograniczony przez kolizje mapy i nigdy nie powinien wylosować miejsca, które jest odseparowane ścianą od koordynatów początkowych.<br>
• W przypadku, gdy w otoczeniu elity II (odległość mniejsza od 8 kratek) występują więcej niż dwie grupy graczy (samotni gracze liczeni są jako grupa o liczności 1), następuje losowanie potwora. W przeciwieństwie do herosa lub tytana, pozycja postaci graczy nie musi sąsiadować z pozycją potwora.<br>
• Elity II nie można zaatakować jak ma się poziom umożliwiający zniszczenie z niej łupu.<br>
• Postacie posiadające poziom umożliwiający zniszczenie łupu z elity II, mogą przez nią przechodzić w taki sposób, jakby nie stanowiła kolizji.<br>
• Jeżeli w drużynie znajduje się gracz, którego poziom umożliwiłby zniszczenie łupu z elity II, nie bierze on udziału w walce. Podczas próby ataku elity II wyświetli się komunikat informujący o tej mechanice.<br>
• Elity II mogą występować na mapie "zamkniętej", co oznacza, że posiada górny limit poziomu postaci, która może na nią wejść za pomocą drzwi lub teleportu. Przykładem takiej elity II jest Furruk Kozug (66lvl).<br>
• Elity II mogą występować na mapie z wyłączoną możliwością grupowania się postaci. Na tej mapie gracze zawsze walczą ze sobą samotnie, a szansa na przedmioty unikatowe, heroiczne oraz legendarne z potwora jest zwiększona o 25% kosztem szansy na przedmiot pospolity (szansa na pusty łup pozostaje bez zmian). Przykładem takiej elity jest Morthen (89lvl).<br>
• Podobnie jak w przypadku innych potworów - elity II posiadające poziom większy od 249 mogą być zawsze atakowane, niezależnie od poziomu postaci. Powyżej poziomu 249, elity II (które nie są umieszczone w zamkniętych lokacjach) dzielą się na rotacyjne grupy - parametry map, na których się znajdują, ulegają zmianie trzy razy w ciągu roku:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Grupy parametrów map:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1: Mechanika przewagi poziomowej: włączona, mechanika karania punktami do listu gończego: włączona.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 2: Mechanika przewagi poziomowej: włączona, mechanika karania punktami do listu gończego: wyłączona.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3: Mechanika przewagi poziomowej: wyłączona, mechanika karania punktami do listu gończego: wyłączona.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;○ Grupy elit:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 1: Cuaitl Citlalin (250 lvl), Chopesz (267 lvl), Vaenra Charkhaam (280 lvl), Zorin (300 lvl).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 2: Pogardliwa Sybilla (255 lvl), Neferkar Set (274 lvl), Chaegd Agnrakh (280 lvl), Furion (300 lvl).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;▪ 3: Quetzalcoatl (260 lvl), Terrozaur (280 lvl, otwarty), Nymphemonia (287 lvl), Artenius (300 lvl).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Powyższe ustawienia można sprawdzić w zakładce "Parametry lokacji" modułu "Świat" wewnątrz gry.<br>
</tabgdzie:<br></lu>