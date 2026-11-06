# Cita Por Favor (EN / RU)
<img width="376" height="707" alt="image" src="https://github.com/user-attachments/assets/b3c4982b-28d2-4dce-92d8-c977ab9bf475" />

A local browser assistant for checking appointment (`cita previa`) availability in **Barcelona province** for:
- **TIE Fingerprints (`Toma de Huellas`)** — initial card or renewal after *Resolución Favorable*
- **Card Issuance (`Expedición de Tarjetas / Gestión Migratoria`)**
- **TIE Pickup (`Recogida de Tarjeta / Lote`)**
- **NIE Assignment (`Asignación de NIE`)**

It runs 100% locally in Chrome via **Tampermonkey**, checks for available appointments on a customizable human-like schedule, and alerts you with sound/voice when slots open. Final confirmation (SMS OTP / captcha) is always completed by you.

> **🌐 Multi-Language UI (`EN` / `RU`)**: The panel defaults to **English (`EN`)** and includes a built-in language switcher (`🌐 Language / Язык`) at the top of the panel to toggle between **English** and **Russian** at any time.

---

## Credits & Attribution

- **Original Creator & Maintainer**: **Katya Levina** — [katilevina/cita-por-favor](https://github.com/katilevina/cita-por-favor)
- **Fork Enhancements**: Bilingual `EN` / `RU` UI picker (English default) and streamlined English documentation by [@cherkuni](https://github.com/cherkuni).

---

## Quick Start (Windows, macOS & Linux)

### 1. Install Tampermonkey & Enable User Scripts
1. Install [Tampermonkey for Chrome](https://chromewebstore.google.com/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo).
2. Open `chrome://extensions`, click **Details** on Tampermonkey, and turn **ON** **`Allow User Scripts`** *(required by Chrome)*.

### 2. Install the Script
1. Open [`cita-autofill.user.js`](cita-autofill.user.js) and click **Copy raw file**.
2. Click the Tampermonkey icon in Chrome → **Create a new script...**
3. Select all (`Ctrl+A` / `Cmd+A`), paste the script (`Ctrl+V` / `Cmd+V`), and save (`Ctrl+S` / `Cmd+S`).

### 3. Open the Appointment Page & Configure
1. Open the Barcelona Extranjería page:
   [https://icp.administracionelectronica.gob.es/icpplustieb/citar?p=8](https://icp.administracionelectronica.gob.es/icpplustieb/citar?p=8)
2. The dark **Cita Por Favor** panel will appear in the top-right corner (in **English** by default).
3. Click **`⚙️ Settings`**:
   - **`👤 Edit My Personal Details`**: Enter your NIE/Passport, Full Name, Birth Year, Nationality, Phone, and Email → click **Save My Personal Details**. *(Stored only locally inside Tampermonkey on your computer).*
   - **`🔍 Search Settings`**: Select your procedure (e.g. *Fingerprints / Toma de Huellas*) and login method (e.g. **Via Cl@ve** → **With Digital Certificate in Chrome (eIdentifier)**) → click **Save Search Settings**.
   - **`📍 Offices to Check`**: Leave unchecked to search all of Barcelona province, or select specific police stations.
4. Click **`🔍 Check Once Now`** to test a single run, or **`▶ Start Checking`** to run on the configured schedule.

---

## Privacy & Safety

- **100% Local**: Your personal details (`NIE`, name, phone, email) never leave your browser except to fill the official Spanish government form (`*.administracionelectronica.gob.es`).
- **One Tab Only**: Run checks in a single tab on one computer at a time to avoid rate-limiting or IP blocks.
- Detailed docs (in Russian): [SETUP.md](SETUP.md) · [PRIVACY.md](PRIVACY.md) · [SAFE_USE.md](SAFE_USE.md) · [CHANGELOG.md](CHANGELOG.md)

---

## На русском (Кратко)

Локальный помощник для проверки доступности *cita previa* (`toma de huellas`, `expedición de tarjetas`, `recogida de tarjeta`, `asignación de NIE`) в провинции Барселона через Chrome и Tampermonkey. Панель поддерживает переключение языка **EN / RU** в верхней строке.

1. Установите [Tampermonkey](https://www.tampermonkey.net/) в Chrome и включите переключатель **«Разрешить пользовательские скрипты» (`Allow User Scripts`)** в `chrome://extensions`.
2. Создайте новый скрипт в Tampermonkey, вставьте содержимое [`cita-autofill.user.js`](cita-autofill.user.js) и сохраните (`Ctrl+S` / `Cmd+S`).
3. Откройте [страницу записи Барселоны](https://icp.administracionelectronica.gob.es/icpplustieb/citar?p=8), при необходимости переключите язык панели (`🌐 Language / Язык: RU · Русский`), заполните данные и запустите проверку.

Подробная документация оригинала ([katilevina/cita-por-favor](https://github.com/katilevina/cita-por-favor)): [SETUP.md](SETUP.md) · [PRIVACY.md](PRIVACY.md) · [SAFE_USE.md](SAFE_USE.md) · [CHANGELOG.md](CHANGELOG.md).

## License

Available for personal and non-commercial use under [PolyForm Noncommercial 1.0.0](LICENSE.md). Original copyright by Katya Levina.
