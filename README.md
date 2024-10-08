# Тестовое задание для фронтенд-разработчика

#### Используя официальную документацию Telegram API, разработать небольшое приложение Miniapp. 
#### Суть приложения проста – отображать ежедневный гороскоп для каждого из 12 знаков зодиака с возможностью автоматического определения языка и его ручного переключения.

<br>

#### Это задание позволит нам:
- Оценить ваши навыки работы с React или Vue.js
- Увидеть ваше умение работы с документацией Telegram miniapps
- Проверить понимание работы со сторонними API других сервисов
- Понять уровень верстки и компетентность в разработке адаптивных интерфейсов

<br>

_* Если вы считаете, что какие-то части задания можно улучшить или добавить, не стесняйтесь предложить свои идеи. Мы ценим инициативу и креативный подход к решению задач._

<br>

После успешного выполнения тестового задания, вам необходимо прислать ссылку на свой репозиторий + ссылку на miniapp для проверки


***

### Функциональные требования:

<br>

#### 1. Автоматическое определение языка:
- Приложение должно автоматически определять язык интерфейса на основе языка, установленного в Telegram
- Если язык Telegram установлен на русский, интерфейс приложения должен быть на русском. Во всех остальных случаях интерфейс должен быть на английском

<br>

#### 2. Страница с блоками зодиаков:
- После открытия приложения пользователь должен видеть страницу с 12 блоками, каждый из которых представляет один знак зодиака
- Дизайн блоков должен быть удобным и интуитивно понятным
- В каждом из контейнеров кликабельного элемента должно находиться Название зодиака + Период дат для него + Иконка

<br>

#### 3. Получение данных с API:
- Для получения описания каждого знака зодиака необходимо сделать POST запрос [по предоставленному API](https://poker247tech.ru/get_horoscope/)
- Описание должно загружаться динамически при нажатии на соответствующий блок зодиака

```json Параметры:

Вариант 1 (ru)
{
    "sign": "aries",
    "language": "original",
    "period": "today"
}
Вариант 2 (en)
{
    "sign": "taurus",
    "language": "translated",
    "period": "today"
}

Если не указываем параметр sign, то получаем в ответе описания всех знаков
```




<br>

#### 4. Отображение и скрытие описания зодиака:
- При нажатии на кнопку с соответствующим зодиаком должно появляться описание для выбранного знака
- В окне описания должна быть кнопка “Назад” из официальной документации Telegram miniapps для закрытия описания и возврата к основному списку
- Также описание должно закрываться при свайпе вправо (для мобильных устройств)

<br>

#### 5. Переключение языка вручную:
- В интерфейсе должна быть возможность вручную переключать язык между русским и английским, независимо от настроек Telegram.
- Переключение языка должно обновлять все тексты в приложении, включая описания знаков зодиака.

<br>

#### 6. Адаптивный дизайн:
- Приложение должно быть адаптивным и корректно отображаться на всех устройствах, поддерживаемых Telegram mini apps.

<br>

#### 7. Развертывание и предоставление доступа:
- Проект должен быть загружен на GitHub. В репозитории должны быть инструкции по сборке и запуску проекта.
- Приложение должно быть развернуто и доступно через ссылку на Telegram mini app, чтобы можно было оценить его работу в реальных условиях.

***

### Дополнительные требования:

- Приложение должно быть выполнено с использованием React или Vue.js
- Используйте современные технологии и подходы (например, React Hooks, Composition API в Vue)
- Обратите внимание на производительность приложения, особенно на мобильных устройствах
- В приложении должен быть качественный и аккуратный дизайн с учетом лучших практик UX/UI

#### Что нужно предоставить:

 1. Ссылку на репозиторий GitHub с исходным кодом проекта.
 2. Ссылку на развернутое mini app для Telegram, чтобы оценить его работу.


