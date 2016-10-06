# Az intercepció hatása a növényzet számára hasznosítható csapadék mértékének alakulására

Az erdei fák számára felvehető csapadék mértékét jelentősen befolyásolja az a vízmennyiség, amit a lombfelület megköt és újra elpárologtat anélkül, hogy az elérhetné a talajfelszínt. Hazai környezetben fenyő esetén a talajfelszínen található vastag száraz tűavar ezt a hatás még jelentősen fokozhatja. Az élő lomb és a száraz avar együttes hatásaként visszatartott csapadékmennyiség eseményenként elérheti az 5-10 mm mértéket, ami sok esetben a teljes csapadékesemény 30-50%-át is jelentheti.

<img src="https://github.com/jsheperd/forest_water/blob/master/img/csapadek.png?raw=true" width="300" height="300" />

### Hipotézis

A növényzet számára felvehető csapadék alakulását nem csak az éves csapadékösszeg befolyásolja, de az eloszlási mintázat is meghatározó. A modellezhetőség szempontjából a legfontosabb tényezők a lombfelület aktuális nagysága, valamint az adott csapadékesemény mértéke mm-ben. A növényzet felhasználható vízellátottságának modellezéséhez további forrásokat és nyelőket is érdemes figyelembe, mint a felszíni elfolyást és a mélybeszivárgást, azonban az első vizsgálatainkban ezeket figyelemen kívül hagyjuk.

### Intercepció számítása

Az intercepció modellezésére a gyakorlatban több módszer is elterjedt.
A legegyszerűbb esetben az intercepciót mint egy szivacsot lehet szemléltetni, amely a telítési állapotig minden csapadékot magába szív, a telítés után pedig már nem köt meg több vizet. A számítások során a csapadékot az intercepció értékével csökkentjük és 0-val maximáljuk. Fejlettebb modellekben az intercepció mértékét a csapadék adott arányában határozzuk meg, így a telítési állapotig lineárisan nő az inercepció értéke, majd onnantól kezdve konstans marad. Az általunk használt modellben egy telítési görbével jellemeztük az intercepció alakulását. A modellhez Dr. Führer Ernő 1994-ben fafajfüggő paramétereket határozott meg gyakorlati mérési eredmények alapján.


<img src="https://github.com/jsheperd/forest_water/blob/master/img/merriam.png?raw=true"/>
[Részletes leírás](https://github.com/jsheperd/forest_water/blob/master/interception.ipynb)

### Elemzések

1. [Szombathely csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/szombathely.ipynb)
2. [Szeged csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/masx0ter/szeged.ipynb)
3. [Debrecen csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/debrecen.ipynb)
4. [Pécs csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/pecs.ipynb)
5. [Budapest csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/budapest.ipynb)

### Felhasznált adatok

Az [Országos meteorológia Szolgálat 1901-2010 éghajalati adasorai](http://www.met.hu/eghajlat/magyarorszag_eghajlata/eghajlati_adatsorok/) napi csapdékeseményeket is tartalmaznak, ami alkalmas arra, hogy becsléseket tegyünk az aktuális csapadékesemény intercepciós veszteségére 110 éves időszakra vonatkozóan.
