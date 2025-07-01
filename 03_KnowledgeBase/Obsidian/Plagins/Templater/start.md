# 🧩 Templater — шаблони в Obsidian

## 🔧 Що таке Templater
Templater — це плагін для Obsidian, який дозволяє створювати динамічні шаблони з автоматичною датою, логікою, вставкою даних.

---

## ✅ Що я вже зробив:
- Встановив плагін через Community Plugins
- Увімкнув `Turn on community plugins`
- Створив шаблон `daily.md` у папці `Templates`
- Додав до шаблону динамічну дату:  
  `<% tp.date.now("YYYY-MM-DD") %>`

---

## ⚙️ Налаштування Templater:
1. **Template folder location** = `Templates`
2. Увімкнено:
   - ✅ `Trigger Templater on new file creation`
   - ✅ `Trigger Templater command on file creation`

---

## 💡 Команди, які використовую:
- `Templater: Insert template` — вставити шаблон у файл
- `Templater: Replace templates in active file` — виконати код
- Гаряча клавіша: `Ctrl + Alt + T` — для швидкої вставки

---

## 🛠 Типові проблеми:
| Проблема                                     | Рішення                                             |
|---------------------------------------------|------------------------------------------------------|
| Код `<% tp.date.now(...) %>` не виконується | Натиснути `Templater: Replace templates...` вручну  |
| Шаблон не вставляється                      | Перевірити назву папки `Templates` і налаштування   |

---

## 📌 Приклад шаблону `daily.md`:
```markdown
# <% tp.date.now("YYYY-MM-DD") %>

## 🔧 Що зроблено:
- [ ]

## 📅 План на завтра:
- [ ]

## 💡 Ідеї / думки:
- ...
## 💡 Команди, які використовую:

- `Ctrl + P` — викликає **Command Palette** — панель команд
  > Тут можна знайти будь-яку команду плагіна чи Obsidian, наприклад:
  > - `Templater: Insert template`
  > - `Templater: Replace templates in active file`
  > - `Create new note`
  > - `Toggle reading view`

- `Templater: Insert template` — вставити шаблон у файл  
- `Templater: Replace templates in active file` — виконати `<% %>` код  
- Гаряча клавіша: `Ctrl + Alt + T` — для миттєвої вставки шаблону

# ⌨️ Гарячі клавіші Obsidian — Стартовий список

Цей список містить найкорисніші гарячі клавіші для ефективної роботи в Obsidian — включно з шаблонами, командною панеллю, посиланнями та структуруванням.

---
## **Налаштування Templater в Obsidian**

### 📌 1. Створи папку для шаблонів (якщо ще немає)

- У File Explorer правою кнопкою → `New folder`
    
- Назви її, наприклад: `Templates`
    

(У тебе вже є така — добре 👍)

---

### ⚙️ 2. Увімкни Templater

- Перейди в **Settings → Plugin Options → Templater**
    
- Налаштуй:
    
    - **Template folder location** → вибери `Templates`
        
    - **Trigger Templater on new file creation** → `ON` (якщо хочеш авто-шаблон)
        

---

### 📝 3. Створи перший шаблон

1. У папці `Templates` → `New note` → назви наприклад: `daily.md`
    
2. Встав туди ось такий код:
    

markdown

КопіюватиРедагувати

`<% tp.file.rename(tp.date.now("YYYY-MM-DD")) %>  # 📅 <% tp.date.now("dddd, MMMM Do YYYY") %>  ## 🔧 Що зроблено: - [ ]  ## 📆 План на завтра: - [ ]  ## 💡 Ідеї / Думки: - ...`

Збережи.

---

### ⚡ 4. Як застосовувати шаблон вручну?

- Відкрий нову нотатку (будь-де)
    
- Відкрий **Command Palette (Ctrl + P)** → `Templater: Insert template`
    
- Вибери `daily.md`
    

💡 Якщо хочеш, щоб він вставлявся **автоматично при створенні нової нотатки**, скажи — налаштуємо через **QuickAdd**.%%  *add link for QuickAdd.* %%

