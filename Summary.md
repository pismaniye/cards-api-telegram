# Разработка приложения для изучения карточек (Telegram Mini App)

## Текущая реализация

### Структура проекта
- `index.html` (или `CARDS.html`): Основной HTML файл
- `styles/main.css`: Стили приложения
- `scripts/main.js`: Основной JavaScript файл с объектом `app`
- `scripts/components/`:
  - `mainPage.js`: Компонент главной страницы
  - `listPage.js`: Компонент страницы списка
  - `wordPage.js`: Компонент страницы слова
  - `repeatPage.js`: Компонент страницы повторения

### Функциональность
1. Навигация между страницами
2. Отображение списков на главной странице
3. Отображение слов внутри списка
4. Добавление и редактирование слов
5. Режим повторения с настройками
6. Сохранение данных в локальное хранилище браузера

### Основные методы в `app`
- `renderPage()`: Отрисовка текущей страницы
- `startRepeat()`: Запуск режима повторения
- `showAnswer()`: Показ ответа в режиме повторения
- `nextWord()`: Переход к следующему слову в режиме повторения
- `saveData()`: Сохранение данных в локальное хранилище
- `loadData()`: Загрузка данных из локального хранилища
- `addList()`, `updateList()`, `deleteList()`: Управление списками
- `addWord()`, `updateWord()`, `deleteWord()`: Управление словами

## Нереализованные функции
1. Возможность выбрать несколько элементов (списков или слов)
2. Удаление списков и слов (свайп или кнопка удаления)
3. Переименование списков (свайп слева направо)
4. Изменение порядка элементов в списке (перетаскивание)
5. Добавление слов, на которых был нажат "Ответ", в очередь на повторение
6. Всплывающее окно с поздравлением после завершения всех карточек
7. Подтверждение удаления элементов

## Следующие шаги
1. Реализация оставшихся функций
2. Улучшение дизайна и пользовательского интерфейса
3. Обработка ошибок и пустых состояний
4. Оптимизация производительности для больших списков
5. Интеграция с Telegram Mini App API

## Примечания
- Приложение разработано с учетом требований для Telegram Mini App
- Текущая версия работает локально без необходимости загрузки на сервер
- Для запуска локально используется Python HTTP сервер