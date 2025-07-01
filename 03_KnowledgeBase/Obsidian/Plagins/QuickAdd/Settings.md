Наступний плагін — **QuickAdd**: натисканням 1 клавіші створюєш:
- Нотатку з шаблону
- Новий курс
- Новий день у щоденнику
- Нову задачу
- ## 🔧 Налаштування QuickAdd (покроково)

### 1. Відкрий:

mathematica

КопіюватиРедагувати

`Settings → Plugin Options → QuickAdd`

### 2. Натисни `Manage Macros → + Add Choice`

Назви вибір, наприклад:

КопіюватиРедагувати

`➕ Новий курс`

---

### 3. Вибери тип:

🔘 `Template`

Далі налаштуй:

- **Template Path:** `Templates/learning.md`
    
- **File Name Format:** `01_Learning/<% tp.system.prompt("Назва курсу") %>`
    
- **Folder:** `01_Learning`
    
- Увімкни:
    
    - ✅ "Open file after creation"
        
    - ✅ "Insert template"
        

---

### 4. Створи другий шаблон, наприклад:

КопіюватиРедагувати

`➕ Новий проєкт`

З параметрами:

- **Template Path:** `Templates/project.md`
    
- **File Name Format:** `02_Projects/<% tp.system.prompt("Назва проєкту") %>`
    
- **Folder:** `02_Projects`
    

---

### 🧪 Як запускати?

- `Ctrl + P` → `QuickAdd: Run QuickAdd`
    
- Обери: ➕ Новий курс / ➕ Новий проєкт
    
- Введи назву — і нотатка створиться зі вставленим шаблоном
    

---

### ⚡ Порада: прив’язати до клавіш

1. `Settings → Hotkeys`
    
2. Знайди: `QuickAdd: Run QuickAdd Choice: Новий курс`
    
3. Признач гарячу клавішу, наприклад:
    
    mathematica
    
    КопіюватиРедагувати
    
    `Ctrl + Alt + C`