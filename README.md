### 📊 **Time-Series-Analysis-Dunnhumby-hw**  
🛒 **Adatelemzés Kiskereskedelmi Promóciós Adatokon**  
---

## 📖 **Leírás**  
Ez a projekt egy valós idejű adatbázison végzett elemzést tartalmaz, ami az értékesítési trendeket, szezonális mintákat és különböző promóciós típusok (akciók, bolti kiemelések) hatékonyságát vizsgálja.  
🎯 **Célja:** betekintést nyújtani a marketingkampányok optimalizálásához és az erőforrások hatékony elosztásához.  

🔍 A projekt választ ad az alábbi üzleti kérdésekre:  
✅ **Mely promóciók növelik leginkább az eladási mennyiségeket?**  
✅ **Hogyan építsük fel a marketingstratégiát a szezonális hatások figyelembevételével?**  
✅ **Hogyan lehet pontosan megjósolni az eladási trendeket, és ezek alapján tervezni az árképzést és készletezést?**  

---

## 📂 **Források**  
🔹 **Adatbázis:** Dunnhumby Dataset  

---

## ⚙️ **Telepítés**  
A szükséges Python csomagok telepítéséhez futtasd az alábbi parancsot:  
```
pip install openpyxl pandas numpy matplotlib seaborn scipy
```

---

## 📥 **Adatok Betöltése**  
Az adatok egy Excel fájlban találhatók (sajnos mérete miatt itt nem elérhető), amely több munkalapot tartalmaz:  
 **dh Store Lookup** – Üzletek adatai  
 **dh Products Lookup** – Termékek adatai  
 **dh Transaction Data** – Tranzakciós adatok  

🔽 **Betöltés és ellenőrzés:**  
```python
import pandas as pd

# Adatok betöltése
file_path = 'file.xlsx'
excel_data = pd.ExcelFile(file_path)

# Munkalapok listázása
print("Munkalapok nevei:", excel_data.sheet_names)
```

---

## 🔍 **Elemzés Folyamata**  
🔹 ** Adattisztítás és előkészítés** – Hibás vagy hiányzó adatok kezelése, oszlopok létrehozása  
🔹 ** Exploratory Data Analysis (EDA)** – Adatok vizualizálása 📊  
🔹 ** Szezonális Mintázatok Elemzése** – 📆 Értékesítési trendek vizsgálata  
🔹 ** Ár-Érzékenységi Elemzés** – 💰 Az ár és kereslet közötti kapcsolat elemzése  
🔹 ** Promóciós Típusok Hatékonysága** – 📢 Különböző promóciók sikerességének vizsgálata  

---

## 💻 **Kód és Felhasznált Könyvtárak**  
 **Használt Python könyvtárak:**  
 **pandas** – Adatok kezelésére és elemzésére  
 **matplotlib, seaborn** – Grafikonok és vizualizáció  
 **scipy** – Statisztikai tesztek  

---

## 📈 **Eredmények**  
**Főbb megfigyelések:**  
A promóciós termékek eladása 📉 ingadozó, míg a nem promóciós termékek kereslete stabil.  
Az árak **jelentősen befolyásolják** az eladási mennyiséget.  
Az akciók **kiemelkedően hatékonyak** az alacsony árkategóriás termékek esetén.  


