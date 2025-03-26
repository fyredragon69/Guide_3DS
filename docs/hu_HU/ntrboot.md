# ntrboot

::: tip

Ha a flashkártyád gyárilag flashelve van az ntrboot-tal (vagy már magad ráflashelted), ugorhatsz a [boot9strap telepítése (ntrboot)](installing-boot9strap-\(ntrboot\)) című útmutatóra, amiben megtudhatod, hogyan kell használni.

:::

## Kötelező olvasmány

Ahhoz, hogy ntrboot segítségével telepíthesd a boot9strap-et, szükséged lesz egy azt támogató NDS / DSi flashkártyára, amire ráflashelheted az ntrbootot. Megjegyzendő, hogy néhány ilyen flashkártyát már gyárilag ntrboot-tal flashelve árulnak.

Míg az ntrboot exploit működése nem függ a rendszerverziótól, az ntrboot flashelő (ami az exploitot a kártyára telepíti) igen. Ez azt jelenti, hogy attól függően, hogy a flashkártyád milyen verziókat és konzolokat támogat, csak bizonyos módszerek lehetnek elérhetőek számodra.

Vedd figyelembe, hogy a "Time Bomb"-bal rendelkező kártyák nem lesznek képesek `.nds` fájlok futtatására, ha észlelik, hogy a rendszeridő meghaladja a flashkártya firmware-je által meghatározott értéket. Ennek megkerülésére az egyik módszer a rendszeridő korábbi dátumra állítása.

| Flashcart neve                                                                                                              |            Aktuális ár |                                "Időbomba"?                                |                                  3DS verziók?                                 |                            DSi verziók?                           | Megjegyzések                                                                                                                                                                                                                                                                                                                    |
| --------------------------------------------------------------------------------------------------------------------------- | ---------------------: | :-----------------------------------------------------------------------: | :---------------------------------------------------------------------------: | :---------------------------------------------------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [**Ace3DS X**](https://www.nds-card.com/ProShow.asp?ProID=575)                                                              | $17.99 |                                    Nem                                    |                                      MIND                                     |                                MIND                               | **ntrboot-tal gyárilag flashelve** (külső kapcsolóval váltogatható az ntrboot ("3DS") és az NDS mód); ne flasheld kézileg ntrboot-tal. Ez a kártya egy SD kártyát igényel behelyezve, hogy egyaránt működjön ntrboot-tal és hagyományos NDS firmware-rel. |
| [**R4i-SDHC B9S** (r4i-sdhc.com)](http://www.nds-card.com/ProShow.asp?ProID=574)         | $16.99 |                     2024 szeptember 3.                    |                                      MIND                                     |                                MIND                               | **Előflashelt ntrboot-tal érkezik**; visszaflashelhető NDS flashkártyára.                                                                                                                                                                                                                                       |
| [**DSTT** (ndstt.com)](http://www.nds-card.com/ProShow.asp?ProID=157)                    | $11.99 |                                    Nem                                    |                                     Nincs                                     |                               Nincs                               | Csak [bizonyos flash chipek](https://gist.github.com/aspargas2/fa2a70aed3a7fe33f1f10bc264d9fab6) kompatibilisek az ntrboot-tal.                                                                                                                                                                                 |
| [**R4i-SDHC 3DS RTS** (r4i-sdhc.com)](http://www.nds-card.com/ProShow.asp?ProID=146)     | $15.99 | 1.85b: 2024 szeptember 3. |                                      MIND                                     |                                MIND                               |                                                                                                                                                                                                                                                                                                                                 |
| [**R4iSDHC GOLD Pro 20XX** (r4isdhc.com)](http://www.nds-card.com/ProShow.asp?ProID=490) | $17.99 |  4.0b: 2024 szeptember 3. |                                      MIND                                     |                                MIND                               | Csak a 2014 vagy későbbi r4isdhc **.com** kártyák, amik kompatibilisek.                                                                                                                                                                                                                         |
| **Ace3DS Plus**                                                                                                             |                        |                                    Nem                                    |                                      MIND                                     |                                MIND                               | Ez a kártya egy SD kártyát igényel behelyezve, hogy egyaránt működjön ntrboot-tal és hagyományos NDS firmware-rel.                                                                                                                                                                                              |
| **Acekard 2i**                                                                                                              |                        |                                    Nem                                    |       <= 4.3.0       | <= 1.4.4 |                                                                                                                                                                                                                                                                                                                                 |
| **Gateway Blue**                                                                                                            |                        |                                    Nem                                    | 4.1.0 - 4.5.0 |                                MIND                               |                                                                                                                                                                                                                                                                                                                                 |
| **Infinity 3 R4i** (r4infinity.com)                                                      |                        |                                    Nem                                    |                                      MIND                                     |                                MIND                               |                                                                                                                                                                                                                                                                                                                                 |
| **R4 3D Revolution**                                                                                                        |                        |                                    Nem                                    |                                     Nincs                                     |                               Nincs                               |                                                                                                                                                                                                                                                                                                                                 |
| **R4i Gold 3DS Plus** (r4ids.cn)                                                         |                        |                                    Nem                                    |                                      MIND                                     |                                MIND                               | **ntrboot-tal előre flashelve** ([belső kapcsolóval váltogatható az ntrboot és az NDS mód](/images/screenshots/r4i-gold-3ds-plus.png)); ne flasheld kézileg ntrboot-tal.                                                                                                                     |
| **R4i Gold 3DS** (r4ids.cn)                                                              |                        |                                    Nem                                    |                                      MIND                                     |                                MIND                               | Minden kártya kompatiblis.                                                                                                                                                                                                                                                                                      |
| **R4i Ultra** (r4ultra.com)                                                              |                        |                                    Nem                                    |       <= 4.3.0       |                                MIND                               |                                                                                                                                                                                                                                                                                                                                 |
| **R4i-SDHC 3DS RTS Deluxe Edition**                                                                                         |                        |                                 Ismeretlen                                |                                      MIND                                     |                                MIND                               | Csak a kék cimkés Deluxe Edition kompatibilis.                                                                                                                                                                                                                                                                  |
| **R4iSDHC RTS LITE 20XX** (r4isdhc.com)                                                  |                        |  4.0b: 2024 szeptember 3. |                                      MIND                                     |                                MIND                               | Csak a 2014 vagy későbbi r4isdhc **.com** kártyák, amik kompatibilisek.                                                                                                                                                                                                                         |
| **R4iSDHC Dual-Core 20XX** (r4isdhc.com)                                                 |                        |  4.0b: 2024 szeptember 3. |                                      MIND                                     |                                MIND                               | Csak a 2014 vagy későbbi r4isdhc **.com** kártyák, amik kompatibilisek.                                                                                                                                                                                                                         |

::: info

![](/images/screenshots/ntrboot-flashcarts.png)

:::

Bizonyosodj meg róla, hogy a flashkártyád képes az `.nds` fájlok futtatására a konzolodon, mielőtt továbbmész. Néhány flashkártya esetében szükség lehet a firmware, vagy "kernel" fájlok SD kártyára másolására. Részletekért lásd az adott flashkártya használati útmutatóját.

Megjegyzendő, hogy a konkrét módszerek további információval szolgálhatnak kompatibilitás terén.

A flashelés módjától függetlenül, ezen exploit használatakor szükséged lesz egy apró mágnesre, ha a cél konzol összecsukható kivitelű (a 3DS családba tartozó összes készülék ilyen, kivéve az Old 2DS-t, ami rendelkezik alvó mód kapcsolóval). Ennek az az oka, hogy az exploithoz alvó módba kell lépni, azonban a gombokra továbbra is szükség van.

::: info

Kipróbálhatod, hogy működik-e a mágnes úgy, hogy az (A), (B), (X), (Y) gombok környékére teszed, miközben a konzol be van kapcsolva, így látod, hogy előidézi-e az alvó állapotot. Ha sikerült, mindkét képernyő elsötétül, és úgy is marad, amíg a mágnest a helyén tartod.

:::

Vedd figyelembe, hogy a flashkártya nem lesz használható az eredeti rendeltetése szerint addig, amíg az ntrboot exploit telepítve van rá. (Kivételt képez az Acekard 2i, ami működőképes marad _kizárólag NDS-eken, és azokon a 3DS-eken, melyekre egyedi firmware van telepítve_.) Ez azt jelenti, hogy a legtöbb flashkártya még csak a HOME Menüben sem jelenik majd meg. Az ntrboot flashelési útmutatójának végén van néhány opcionális lépés arról, hogyan töröld azt a flashkártyádról, ha már végeztél.

::: danger

Vedd figyelembe, hogy néhány ritka esetben lehetséges, hogy a flashelési folyamat során **brickelődjön** néhány hamisított flashkártya és végleg használhatatlanná váljon. Ez elég valószínűtlen, azonban éppen emiatt csak eredeti flashkártyákat támogatunk. Hogy csökkentsd a kockázatát a hamisított kártya megvásárlásának, javasoljuk, hogy egy megbízható oldalról vásárold azt (mint például az [NDS Card](https://www.nds-card.com/)).

:::

___

## Módszerek

___

### Ntrboot flashelése (egy 3DS rendszer)

Ehhez a módszerhez mindössze egy gyári állapotú 3DS-re és egy kompatibilis flashkártyára van szükséged. Ez a módszer a flashkártyát használja, hogy futtassa az ntrboot flashelő `.nds` fájlt a 3DS-eden. Ez azt jelenti, hogy a flashkártyádnak támogatnia kell `.nds` fájlok futtatását a 3DS-ed verzióján. További információkért lásd a flashkártyák táblázatát.

::: tip

Tovább az [ntrboot flashelése (egy 3DS)](flashing-ntrboot-\(3ds-single-system\)) oldalra

:::

___

### Ntrboot flashelése (több 3DS rendszer)

Ehhez a módszerhez szükséged lesz átmenetileg egy második 3DS-családból származó konzolra, amin már telepítve van a boot9strap. Viszont egyik 3DS verziójának sem szükséges támogatnia a flashkártyádat.

::: tip

Tovább az [ntrboot flashelése (több 3DS)](flashing-ntrboot-\(3ds-multi-system\)) oldalra

:::

___

### Ntrboot flashelése (NDS)

Ehhez a módszerhez szükséged lesz átmenetileg egy Nintendo DS vagy egy Nintendo DS Lite készülékre, ami kompatibilis a flashkártyáddal. Ez a módszer a flashkártyát használja, hogy futtassa az ntrboot flashelő `.nds` fájlt az NDS-eden.

::: tip

Tovább az [ntrboot flashelése (NDS)](flashing-ntrboot-\(nds\)) oldalra

:::

___

### Ntrboot flashelése (DSi)

Ehhez a módszerhez szükséged lesz átmenetileg egy Nintendo DSi készülékre, ami kompatibilis a flashkártyáddal. Ez a módszer a flashkártyát használja, hogy futtassa az ntrboot flashelő `.nds` fájlt a DSi-den. Ez azt jelenti, hogy a flashkártyádnak támogatnia kell `.nds` fájlok futtatását azon a verzión, amin a DSi-d áll. További információkért lásd a flashkártyák táblázatát.

::: tip

Tovább az [ntrboot flashelése (DSi)](flashing-ntrboot-\(dsi\)) oldalra

:::
