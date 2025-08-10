# 🚀 Развертывание веб-сайта Open Deep Water на GitHub Pages

Это руководство поможет вам создать красивый веб-сайт для проекта **Open Deep Water** на GitHub Pages.

## 📋 Пошаговая инструкция

### Шаг 1: Создание GitHub репозитория

1. Войдите в свой аккаунт на [GitHub](https://github.com)
2. Нажмите кнопку **"New repository"** (зеленая кнопка справа)
3. Заполните форму:
   - **Repository name**: `Open_Deep_Water`
   - **Description**: `OEM WetEnd Integration Program - Open Science Platform Concept`
   - **Public** (чтобы GitHub Pages работали бесплатно)
   - ✅ **Add a README file**
   - **License**: Creative Commons Zero v1.0 Universal

4. Нажмите **"Create repository"**

### Шаг 2: Загрузка файлов

1. В новом репозитории нажмите **"uploading an existing file"**
2. Загрузите все файлы из папки `/home/andrew/Open_Deep_Water/`:
   - `index.html` (английская версия - основная)
   - `index_ru.html` (русская версия)
   - `README.md`
   - `_config.yml`
   - `Open_Deep_Water_RU.pdf`
   - `Open_Deep_Water_EN.pdf`
   - `Open_Deep_Water.md`
   - Папка `assets/` с файлом `style.css`

3. Добавьте commit message: `Initial website setup`
4. Нажмите **"Commit changes"**

### Шаг 3: Настройка GitHub Pages

1. В репозитории перейдите в **Settings** (вкладка справа)
2. Прокрутите вниз до раздела **"Pages"**
3. В разделе **"Source"** выберите:
   - **Deploy from a branch**
   - **Branch**: `main` (или `master`)
   - **Folder**: `/ (root)`
4. Нажмите **"Save"**

### Шаг 4: Обновление ссылок

1. Файлы уже настроены для репозитория `ipmgroup/Open_Deep_Water`
2. Если вы используете другой username, обновите в файлах:
   - В `README.md`
   - В `index.html`
   - В `index_ru.html`
   - В `_config.yml`

3. Для репозитория ipmgroup файл `_config.yml` содержит:
```yaml
url: "https://ipmgroup.github.io"
baseurl: "/Open_Deep_Water"
github_username: ipmgroup
```

### Шаг 5: Проверка развертывания

1. GitHub обработает файлы (это займет 5-10 минут)
2. Ваш сайт будет доступен по адресу: `https://ipmgroup.github.io/Open_Deep_Water/`
3. Проверьте работу обеих языковых версий

## 🎨 Дополнительные возможности

### Добавление иконки (favicon)
1. Создайте файл `favicon.ico` размером 16x16 или 32x32 пикселя
2. Поместите в папку `assets/`
3. Файлы HTML уже содержат ссылку на `assets/favicon.ico`

### Добавление изображения для социальных сетей
1. Создайте изображение `preview.png` размером 1200x630 пикселей
2. Поместите в папку `assets/`
3. Обновите meta-теги Open Graph в HTML файлах

### Настройка Google Analytics
1. Получите код отслеживания GA4
2. Добавьте его в `_config.yml`:
```yaml
google_analytics: G-XXXXXXXXXX
```

### Добавление контактной формы
Можно использовать сервисы как:
- [Formspree](https://formspree.io/)
- [Netlify Forms](https://www.netlify.com/products/forms/)
- [Google Forms](https://forms.google.com/)

## 📱 Мобильная оптимизация

Сайт уже оптимизирован для мобильных устройств:
- ✅ Респонсивный дизайн
- ✅ Viewport meta-тег
- ✅ Адаптивная сетка
- ✅ Мобильное меню

## 🔧 Технические детали

### Используемые технологии:
- **HTML5** с семантической разметкой
- **CSS3** с современными функциями (Grid, Flexbox, Backdrop-filter)
- **JavaScript** для плавной прокрутки
- **GitHub Pages** с Jekyll поддержкой
- **Responsive Design** для всех устройств

### Особенности дизайна:
- 🎨 Современный градиентный дизайн
- 🌟 Анимации и переходы
- 📱 Мобильная адаптивность
- 🌍 Двуязычная поддержка
- ♿ Доступность (accessibility)

## 🚀 Запуск локально (для разработки)

Если хотите тестировать сайт локально:

```bash
# Установите Jekyll
gem install jekyll bundler

# Клонируйте репозиторий
git clone https://github.com/your-username/Open_Deep_Water.git
cd Open_Deep_Water

# Создайте Gemfile
echo 'source "https://rubygems.org"' > Gemfile
echo 'gem "github-pages", group: :jekyll_plugins' >> Gemfile

# Установите зависимости
bundle install

# Запустите локальный сервер
bundle exec jekyll serve

# Откройте http://localhost:4000 в браузере
```

## 📧 Поддержка

Если возникли вопросы по развертыванию:
- 📖 [Документация GitHub Pages](https://docs.github.com/en/pages)
- 💬 [Jekyll документация](https://jekyllrb.com/docs/)
- 🆘 [GitHub Community](https://github.community/)

---

🌊 **Open Deep Water** — Opening the depths of scientific collaboration!

© 2025 Andrew Buckin. Distributed under Creative Commons CC-BY 4.0 license.
