# LibreLMS — предрелизная страница

Временная landing-страница веб-портала ИТ-экосистемы LibreLMS. Показывает экран «скоро откроется» до запуска полноценного портала.

## Технологии

- [Astro](https://astro.build/) — статическая генерация
- TypeScript
- CSS (без UI-библиотек)

## Установка

```bash
npm install
```

## Разработка

```bash
npm run dev
```

Сайт будет доступен по адресу `http://localhost:4321`.

## Сборка

```bash
npm run build
```

Результат сборки — папка `dist/`, готовая к статическому хостингу.

## Предпросмотр production-сборки

```bash
npm run preview
```

## Деплой

Проект рассчитан на **статический хостинг** через [Onreza](https://onreza.com/):

1. Выполните `npm run build`.
2. Загрузите содержимое папки `dist/` на хостинг.
3. Укажите корневую директорию сайта как `dist` (или загрузите файлы из `dist` в корень).

Серверные функции не используются — только статические HTML/CSS/JS.

## Структура

```
src/
  components/ComingSoonHero.astro  — hero-секция «скоро откроется»
  layouts/BaseLayout.astro       — базовый layout с meta и шрифтами
  pages/index.astro              — главная страница
  styles/global.css              — глобальные стили и CSS-переменные
public/
  logo/                          — актуальные логотипы LibreStudium (SVG)
  favicon.svg
```

## Бренд

Цвета и типографика соответствуют брендбуку LibreStudium:

- Deep Blue `#1E3A8A`, Bright Blue `#3B82F6`, Light Blue `#93C5FD`
- Шрифты: Jost (заголовки), Manrope (текст)
