## 🧱 **I. Створи репозиторій на GitHub**

1. Перейди на [https://github.com](https://github.com)
    
2. Натисни ➕ `New repository`
    
3. Назви його:
    
    nginx
    
    КопіюватиРедагувати
    
    `KostiantynVault`
    
4. **Do not initialize with README** (важливо)
    
5. Створи (Create repository)
    

---

## 💻 **II. Підключи свій Vault до GitHub**

### 🔧 Відкрий термінал у папці Vault

1. Перейди в ту папку, де знаходиться твій Vault (`KostiantynVault`)
    
2. Відкрий термінал/PowerShell/WSL в цій папці
    

### 🔁 Ініціалізуй Git:

bash

КопіюватиРедагувати

`git init git remote add origin https://github.com/your-username/KostiantynVault.git`

⚠️ **Замінити `your-username` на свій логін GitHub!**

---

## 📄 **III. Створи `.gitignore` файл**

1. Створи в корені Vault файл `.gitignore`
    

### Вміст `.gitignore`:

bash

КопіюватиРедагувати

`.obsidian/plugins/*/data.json .obsidian/workspace .trash .DS_Store Thumbs.db node_modules`

> Це допоможе уникнути конфліктів у плагінах, кешах, тимчасових файлах.

---

## 💾 **IV. Додай і відправ перший коміт**

bash

КопіюватиРедагувати

`git add . git commit -m "initial commit" git branch -M main git push -u origin main`

Якщо Git попросить логін/пароль:

- Рекомендується використовувати **GitHub Personal Access Token** замість пароля  
    (Якщо треба — допоможу створити)
    

---

## 📱 **V. Мобільна синхронізація (iOS/Android)**

### iOS:

- Встанови **Working Copy** (App Store)
    
- Підключи репозиторій GitHub
    
- Увімкни **Obsidian Sync Folder** з iCloud → Working Copy
    
- Кожен раз після змін:
    
    - `Pull` → отримати нове з GitHub
        
    - `Commit + Push` → відправити свої зміни