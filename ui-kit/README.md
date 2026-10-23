# Ниже представлен список реализованных блоков с их элементами и модификаторами.

1. header
   Шапка сайта с логотипом и навигацией.
   Элементы: header**logo, header**nav
2. menu
   Список навигационных ссылок.
   Элементы: menu**item, menu**link
   Модификаторы: menu\_\_link--current
3. showcase
   Базовый раздел витрины для группировки контента.
   Элементы: showcase**title, showcase**text
4. swatch
   Образец цвета из палитры.
   Элементы: swatch\_\_name
   Модификаторы: swatch--primary, swatch--secondary, swatch--success, swatch--danger, swatch--warning, swatch--info, swatch--light, swatch--dark
5. button
   Интерактивная кнопка.
   Модификаторы: button--primary (по умолчанию), button--secondary, button--danger, button--small
   Состояния: :hover, :focus-visible, :active, :disabled
6. badge
   Статусный ярлык (бейдж).
   Модификаторы: badge--new, badge--sale (или badge--success, badge--warning, badge--danger в зависимости от реализации статусов)
7. field
   Обертка для поля ввода с подписью и подсказкой.
   Элементы: field**label, field**control, field\_\_hint
   Модификаторы: field--error
   Состояния: :disabled (для вложенного input)
8. check
   Кастомный чекбокс или радиокнопка.
   Элементы: check**input, check**label
9. form / form-list
   Контейнер для формы или списка полей.
10. card
    Карточка товара или контента.
    Элементы: card**image, card**title, card**text, card**link
11. card-list
    Сетка карточек (адаптивная).
12. alert
    Блок системного уведомления.
    Элементы: alert**title, alert**text
    Модификаторы: alert--success, alert--danger

Результаты проверок:
Заголовок на три строки не ломает карточку
Кнопка прижата к низу благодаря Flexbox (margin-top: auto).
Карточка без картинки выглядит аккуратно
Отступы сохранены, визуальной дыры нет.
На ширине 360 px нет горизонтальной прокрутки
Использован overflow-x: hidden и адаптивные единицы измерения.
Навигация клавишей Tab (доступность)
Фокус виден на всех интерактивных элементах (:focus-visible).
Валидация W3C (validator.w3.org)
Ошибок валидации нет.
Смена --color-primary
Акцентные элементы (кнопки, ссылки, фокус) меняют цвет глобально.

Технические требования
БЭМ: Все классы написаны по методологии БЭМ.
Селекторы: Селекторы по тегам используются только в base.css. Селекторы по ID отсутствуют (ID используются только для якорей и связи label[for] с input[id]).
Inline-стили: В HTML отсутствуют атрибуты style.
Переменные: Все цвета и отступы вынесены в variables.css.
