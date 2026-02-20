# 🚀 БЫСТРАЯ ИНСТРУКЦИЯ — 5 МИНУТ ДО ДЕПЛОЯ

## ✅ ШАГ 1: Скачайте изображения (В CHROME!)

**⚠️ СДЕЛАЙТЕ ЭТО ПЕРВЫМ!**

1. Откройте Figma Make в **Chrome**
2. Нажмите **⌘ + ⌥ + J** (Console)
3. Найдите файл `COPY_THIS_SCRIPT.txt` в Figma Make
4. Скопируйте длинную строку (от `const` до `;`)
5. Вставьте в Console: **⌘ + V**
6. Нажмите **Enter**
7. Подождите 20 секунд
8. ✅ Все 29 PNG скачаются в Downloads

---

## ✅ ШАГ 2: Создайте проект в Cursor

```bash
mkdir fastmine-landing
cd fastmine-landing
```

Откройте Cursor: **File → Open Folder** → `fastmine-landing`

---

## ✅ ШАГ 3: Скопируйте базовые файлы

Из Figma Make скопируйте файлы из папки `/CURSOR_READY/`:

### Корневые файлы:
- ✅ `package.json`
- ✅ `vite.config.ts`
- ✅ `tsconfig.json`
- ✅ `tsconfig.node.json`
- ✅ `postcss.config.mjs`
- ✅ `index.html`
- ✅ `.gitignore`

### Папка src/:
- ✅ `src/main.tsx`
- ✅ `src/app/App.tsx`
- ✅ `src/styles/index.css`
- ✅ `src/styles/tailwind.css`
- ✅ `src/styles/theme.css`
- ✅ `src/styles/fonts.css`

---

## ✅ ШАГ 4: Скопируйте FormatsImproved.tsx

**В Figma Make:**

1. Найдите файл `/FormatsImproved.production.tsx`
2. Откройте его
3. Выделите всё: **⌘ + A**
4. Скопируйте: **⌘ + C**

**В Cursor:**

5. Создайте файл: `src/app/components/FormatsImproved.tsx`
6. Вставьте: **⌘ + V**
7. Сохраните: **⌘ + S**

📖 Подробнее: см. файл `HOW_TO_COPY_FORMATS.md`

---

## ✅ ШАГ 5: Добавьте изображения

```bash
mkdir -p public/assets
mv ~/Downloads/*.png public/assets/
```

**Или перетащите** 29 PNG из Downloads в `public/assets/`

---

## ✅ ШАГ 6: Установите зависимости

```bash
npm install
```

---

## ✅ ШАГ 7: Проверьте

```bash
npm run dev
```

Откройте http://localhost:5173 🎉

---

## ✅ ШАГ 8: GitHub

```bash
git init
git add .
git commit -m "Initial commit: FastMine landing"

# Создайте repo на https://github.com/new
# Затем:
git remote add origin https://github.com/ваш-username/fastmine-landing.git
git branch -M main
git push -u origin main
```

---

## ✅ ШАГ 9: Vercel

1. Откройте https://vercel.com
2. Войдите через GitHub
3. **New Project**
4. Выберите `fastmine-landing`
5. **Deploy**

🎉 **ГОТОВО! САЙТ ОНЛАЙН!**

---

## 📋 Чеклист:

- [ ] Скачаны 29 изображений
- [ ] Скопированы все файлы из `/CURSOR_READY/`
- [ ] Скопирован `FormatsImproved.tsx`
- [ ] Изображения в `public/assets/`
- [ ] `npm install` выполнен
- [ ] `npm run dev` работает
- [ ] Код в GitHub
- [ ] Деплой на Vercel

---

## 🆘 Проблемы?

- **Изображения не грузятся** → Проверьте что все PNG в `public/assets/`
- **Module not found** → Проверьте что `FormatsImproved.tsx` на месте
- **Tailwind не работает** → Перезапустите `npm run dev`

Подробнее: см. `README.md`
