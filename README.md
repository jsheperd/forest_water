# Az intercepció hatása a növényzet számára hasznosítható csapadék mértékének alakulására

Az erdei fák számára felvehető csapadék mértékét jelentősen befolyásolja az a vízmennyiség, amit a lombfelület megköt és újra elpárologtat anélkül, hogy az elérhetné a talajfelszínt. Hazai környezetben fenyő esetén a talajfelszínen található vastag száraz tűavar ezt a hatást  még jelentősen fokozza. Hazai fenyveseinkben az élő lomb és a száraz avar együttes hatásaként visszatartott csapadékmennyiség esetenként elérheti az 5-10 mm értéket, ami sok esetben a teljes csapadékesemény 30-50%-át is jelentheti. A fásszárú vegetáció számára az intercepció hatása nem hagygató figyelmen kívül.

<img src="https://github.com/jsheperd/forest_water/blob/master/img/csapadek.png?raw=true" width="300" height="300" />

### Intercepció számítása

A növényzet számára felvehető csapadék alakulását nem csak az éves csapadékösszeg befolyásolja, de az eloszlási mintázat is meghatározó. A modellezhetőség szempontjából a legfontosabb tényezők a lombfelület aktuális nagysága, valamint az adott csapadékesemény mértéke mm-ben. A növényzet felhasználható vízellátottságának pontos modellezéséhez további forrásokat és nyelőket is érdemes figyelembe, mint a felszíni elfolyást és a mélybeszivárgást, vagy a talaj víztározó képességét, azonban az első vizsgálatainkban ezeket még figyelemen kívül hagytuk.

Az intercepció modellezésére a gyakorlatban több módszer is elterjedt. A legegyszerűbb esetben a benedvesedési kapacitás eléréséig az intercepció a csapadékot teljesen visszatartja a talajtól. Ennél finomabb közelítés amikor a csapadéknak csak adott hányadát engedi keresztül a lombozat mindaddig amíg nem telítődik teljesen. Az itt használt modellben a lombozat csapadékvisszatartási képssége az átnedvesedés során folyamatosan egy telítési függvénnyel csökken. Dr. Führer Ernő 1994-ben fafajfüggő paramétereket határozott meg gyakorlati mérési eredmények alapján.


<img src="https://github.com/jsheperd/forest_water/blob/master/img/merriam.png?raw=true"/>
[Részletes leírás](https://github.com/jsheperd/forest_water/blob/master/interception.ipynb)

### Elemzések

1. [Szombathely csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/notebook/szombathely.ipynb)
2. [Szeged csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/notebook/szeged.ipynb)
3. [Debrecen csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/notebook/debrecen.ipynb)
4. [Pécs csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/notebook/pecs.ipynb)
5. [Budapest csapadékeloszlása 1901 - 2010 időszakban](https://github.com/jsheperd/forest_water/blob/master/notebook/budapest.ipynb)

### Felhasznált adatok

Az [Országos meteorológia Szolgálat 1901-2010 éghajalati adasorai](http://www.met.hu/eghajlat/magyarorszag_eghajlata/eghajlati_adatsorok/) napi csapdékeseményeket is tartalmaznak, ami alkalmas arra, hogy becsléseket tegyünk az aktuális csapadékesemény intercepciós veszteségére 110 éves időszakra vonatkozóan.
