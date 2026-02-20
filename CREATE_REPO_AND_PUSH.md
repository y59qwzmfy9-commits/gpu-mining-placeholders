# Создать репозиторий и запушить код

1. **Создай новый репозиторий на GitHub**
   - Зайди на https://github.com/new
   - Repository name: `gpu-mining-placeholders` (или любое имя)
   - **Не** добавляй README, .gitignore, license — репо должен быть пустым
   - Create repository

2. **Подключи remote и запушь** (если имя репо другое — замени в URL):
   ```bash
   cd "/Users/danil/Downloads/GPU Mining Landing Page-11-8/gpu-mining-no-photos"
   git remote remove origin 2>/dev/null
   git remote add origin https://github.com/y59qwzmfy9-commits/gpu-mining-placeholders.git
   git push -u origin main
   ```

3. **Подключи проект к Vercel**
   - Vercel → Add New Project → Import Git Repository → выбери `gpu-mining-placeholders`
   - Deploy

После этого можно по одному заменять файлы в `src/assets/` на свои фото и пушить — см. ASSETS_README.md.
