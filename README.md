# Time-Series-Analysis---Dunnhumby---hw

# Adatelemzés Kiskereskedelmi Promóciós Adatokon
## Leírás
Ez a projekt egy valós idejű adatbázison végzett elemzést tartalmaz, ami az értékesítési trendeket, a szezonális mintákat és a különböző típusú promóciók (akciók, bolti kiemelések) hatékonyságát vizsgálja. A célja, hogy betekintést nyújtson a marketingkampányok optimalizálásához és az erőforrások hatékony elosztásához.

A projekt segítséget nyújt az alábbi üzleti kérdések megválaszolásában:
- Mely promóciós típusok növelik leginkább az eladási mennyiségeket?
- Hogyan alakítsuk ki a marketingstratégiát a szezonális hatások figyelembevételével?
- Hogyan lehet pontosan megjósolni az eladási trendeket, és ezek alapján tervezni az árképzést és készletezést?

## Források
A projekt az alábbi forrást használja:
- [Dunnhumby Adatbázis](https://www.dunnhumby.com/source-files/)

## Telepítés

A szükséges Python csomagok telepítése:

```bash
pip install openpyxl pandas numpy matplotlib seaborn scipy
```

## Adatok Betöltése
A projekt adatai az Excel fájlban találhatók. A fájl különböző munkalapokat tartalmaz, például:
- **dh Store Lookup**: Üzletek adatai
- **dh Products Lookup**: Termékek adatai
- **dh Transaction Data**: Tranzakciós adatok

A kód segítségével az adatokat beolvashatjuk és előkészíthetjük az elemzéshez.

```python
import pandas as pd

# Adatok betöltése
file_path = 'file.xlsx'
breakfast = pd.ExcelFile(file_path)

# Munkalapok ellenőrzése
print("Munkalapok nevei:", breakfast.sheet_names)
```

## Elemzés
Az adatok előkészítése után következő lépéseket jönnek:
1. **Adattisztítás és előkészítés**: Az adatok előkészítése és a szükséges oszlopok létrehozása.
2. **Exploratory Data Analysis (EDA)**: Az adatok vizualizálása és a promóciók hatékonyságának összehasonlítása.
3. **Szezonális Mintázatok Elemzése**: Az értékesítési trendek és szezonális hatások elemzése.
4. **Ár-Érzékenységi Elemzés**: Az árak és az eladások közötti kapcsolat vizsgálata.
5. **Promóciós Típusok Hatékonysága**: A különböző promóciós típusok hatékonyságának elemzése kategóriák szerint.

## Kód
A kód Python-ban íródott és a következő könyvtárakat használom:
- `pandas`: Adatok kezelésére és elemzésére.
- `matplotlib`, `seaborn`: Az adatok vizualizálására.
- `scipy`: Statisztikai tesztekhez.

## Eredmények
A projekt eredményei közé tartoznak a következő megfigyelések:
- A promóciós termékek eladása ingadozó, míg a nem promóciós termékek stabil kereslettel rendelkeznek.
- Az árak jelentős hatással vannak az eladások számának alakulására.
- A promóciók különösen jól működnek az alacsony árkategóriában.

