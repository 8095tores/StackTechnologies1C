# Стек технологий для 1С
- [Стек технологий для 1С](#стек-технологий-для-1с)
- [Разработка](#разработка)
  - [Языки программирования](#языки-программирования)
    - [Встроенный язык программирования 1С:Предприятия](#встроенный-язык-программирования-1спредприятия)
    - [Язык запросов](#язык-запросов)
    - [Платформа для мобильных устройств](#платформа-для-мобильных-устройств)
    - [1С:Исполнитель](#1сисполнитель)
    - [1С:Предприятие.Элемент](#1спредприятиеэлемент)
    - [OneScript](#onescript)
  - [IDE](#ide)
    - [Конфигуратор](#конфигуратор)
    - [EDT](#edt)
    - [VSCode](#vscode)
  - [Плагины](#плагины)
    - [Снегопат](#снегопат)
    - [BSL Plagin](#bsl-plagin)
    - [Подсистема разработчика](#подсистема-разработчика)
  - [Базы данных](#базы-данных)
    - [Файловая](#файловая)
    - [MS SQL](#ms-sql)
    - [Postgres](#postgres)
- [Системы хранения версий](#системы-хранения-версий)
  - [Хранилище](#хранилище)
  - [git](#git)
- [Прототипирование](#прототипирование)
  - [MockPlus](#mockplus)
  - [mock1c](#mock1c)
- [Повышение качества продуктов](#повышение-качества-продуктов)
  - [Автоматизированное тестирование](#автоматизированное-тестирование)
  - [1С:Сценарное тестирование](#1ссценарное-тестирование)
  - [1С:Тестировщик](#1стестировщик)
  - [Vanessa Behavior](#vanessa-behavior)
  - [xUnitFor1C](#xunitfor1c)
  - [Статический анализ текста](#статический-анализ-текста)
    - [Синтаксическая проверка конфигурации](#синтаксическая-проверка-конфигурации)
    - [1С:Автоматизированная проверка конфигураций](#1савтоматизированная-проверка-конфигураций)
    - [Плагин для SonarQube](#плагин-для-sonarqube)
  - [Прочее](#прочее)
    - [Code-review](#code-review)
    - [Стандарты разработки](#стандарты-разработки)
    - [Allure](#allure)
- [CI/CD](#cicd)
    - [Gitlab CI](#gitlab-ci)
    - [Travis](#travis)
    - [Github CI](#github-ci)
    - [Jenkins](#jenkins)
    - [Docker](#docker)
- [Интеграции](#интеграции)
    - [1С:Аналитика](#1саналитика)
    - [Телеграмм бот](#телеграмм-бот)
    - [Rabbit MQ](#rabbit-mq)
    - [Kafka](#kafka)
    - [Power BI](#power-bi)
- [Продуктивность](#продуктивность)
  - [Трекеры задач](#трекеры-задач)
    - [Jira](#jira)
    - [Bitrix24](#bitrix24)
    - [Todoist](#todoist)
    - [Wunderlinst](#wunderlinst)
  - [Базы знаний](#базы-знаний)
    - [Notion](#notion)
    - [Confluence](#confluence)
    - [Wiki](#wiki)
- [Благодарность](#благодарность)


# Разработка
## Языки программирования
### Встроенный язык программирования 1С:Предприятия

Встроенный язык системы 1С:Предприятия. На стадии разработки конфигурации предназначен для описания алгоритмов функционирования прикладной задачи. Основной язык разработчика 1С.

![alt text](img/ВстроенныйЯзыкПрограммирования1С.png "Встроенный язык программирования 1С")​

**На что обратить внимание**

Новые возможности языка программирования обычно добавляют при выпуске новых версий платформы.
Поэтому имеет смысл отслеживать изменения в версиях, чтобы использовать новые технологии.

**С чего начать:**

Книги:
1. М.Г. Радченко. - 1С:Програмирование для начинающих - https://buh.ru/books/detail.php?ID=51780

Курсы:
1. Учебный центр 1С - https://uc1.1c.ru
2. Хорошие курсы на сайте https://курсы-по-1с.рф

**Подробнее:**
1. Официальный сайт: https://v8.1c.ru/platforma/  
2. Документация к платформе: https://its.1c.ru/db/v8320doc

[В начало](#стек-технологий-для-1с)
### Язык запросов
Язык запросов основан на [SQL](https://ru.wikipedia.org/wiki/SQL), при этом содержит как ограничения так и расширения, ориентированные на отражение специфики финансово-экономических задач.

![alt text](img/КонструкторЗапросов.png "Конструктор запросов")​

**На что обратить внимание:**

1. Статья - [Типичные причины неоптимальной работы запросов и методы оптимизации](https://its.1c.ru/db/metod8dev/content/5842/hdoc). 
Следуя этим рекомендациям можно избежать большинство проблем с производительностью запросов.
2. Для отладки запросов можно использовать Консоль запросов. Этот инструмент позволяет выполнять и отлаживать запросы в режиме 1С:Предприятие.
Разработок на эту тему много, можно поискать по запросу [Консоль запросов](https://infostart.ru/public/all/?st=t&sort=postsd&public-filter%5Bsearch%5D=%CA%EE%ED%F1%EE%EB%FC+%E7%E0%EF%F0%EE%F1%EE%E2)

**С чего начать:**

Статьи:

1. Особенности языка запросов 1С - https://infostart.ru/1c/articles/204054/
2. Полезные сведения о языке запросов 1С 8.2 - https://infostart.ru/1c/articles/165456/

Книги:
1. Е. Ю. Хрусталева - Язык запросов 1С:Предприятия 8 - https://its.1c.ru/db/pubqlang

**Подробнее**
1. Официальный сайт: https://v8.1c.ru/platforma/mehanizm-zaprosov/

[В начало](#стек-технологий-для-1с)
### Платформа для мобильных устройств
По факту используется тот же язык программирования, но есть ограничения.
С помощью этой платформы можно полностью создать приложение для мобильных устройств.

![alt text](img/МобильнаяПлатформа.png "Мобильная платформа")​

**На что обратить внимание**

Есть много хороших программ, созданных с помощью мобильной платформы как вендора, так и сторонних разработчиков.
Кажется, что сейчас это тренд и требуется во многих вакансиях.

**С чего начать:**

Статьи: 

Книги:
1. Е. Ю. Хрусталева - Знакомство с разработкой мобильных приложений на платформе 1С:Предприятие 8 - https://v8.1c.ru/metod/books/42725.htm

**Подробнее:**

Официальный сайт: https://v8.1c.ru/platforma/mobilnaya-platforma-1s-predpriyatiya/


### 1С:Исполнитель
Это кроссплатформенный язык сценариев. Язык базируется на встроенном языке разработки 1С:Предприятие, но имеет ряд отличий от него.
1С:Исполнитель - это инструмент для автоматизиации и администрирования информационных систем, созданных на платформе 1С:Предприятие.

![alt text](img/Исполнитель.png "1С:Исполнитель")​

**На что обратить внимание**
Кажется, что этот язык - это "проба пера" для нового языка и новых технологий фирмы 1С.
Имеет смысл ознакомиться с новыми возможностями, но глубоко изучать язык, кажется, не обязательным.
Так как сфера применения его довольно специфичная.

**С чего начать:**
1. Статья на зазеркалье - https://wonderland.v8.1c.ru/blog/1c-ispolnitel/

### 1С:Предприятие.Элемент
Новая разработка фирмы 1С. Информации пока не много. Сообщается, что это тот же язык, что используется в 1С:Исполнитель.

В качестве основных компонентов технологии обозначены:
- новый пользовательский интерфейс, ориентированный в первую очередь на работу в веб;
- динамично развивающийся встроенный язык;
- поддержка модульности разработки;
- среда разработки, развернутая в облаке и доступная через браузер;
- ориентация на работу решений в облаке, но будет поддержка и локальной установки (on-premise);
- мобильность, что подразумевает возможность работы приложения на мобильных устройствах и в мобильных браузерах сразу «из коробки».

![alt text](img/1СПредприятиеЭлемент.png "1С:Предприятие. Элемент")​

**На что обратить внимание**
Решения, уже использующие эту технологию:
- [«1С:Кабинет сотрудника»](https://portal.1c.ru/applications/94)
- [1С:Шина](https://wonderland.v8.1c.ru/blog/integratsionnaya-shina/)
- Сервис [mag1C](https://mag1c.ru)
- [1С:Аналитика](https://wonderland.v8.1c.ru/blog/1s-analitika/)
- Сайт [developer.1c.ru](https://developer.1c.ru) создан с помощью этой технологии

**С чего начать:**
1. Статья на зазеркалье - https://wonderland.v8.1c.ru/blog/novaya-tekhnologiya-razrabotki-prilozheniy/

### OneScript

## IDE

### Конфигуратор

### EDT

### VSCode

## Плагины
Плагины, которые помогают в разработке на языках 1С

### Снегопат

### BSL Plagin

### Подсистема разработчика


## Базы данных
Для 1С могут использоваться разные базы данных. Для каждой могут быть свои особенности.

### Файловая

### MS SQL

### Postgres

# Системы хранения версий
Нужны для того, чтобы отслеживать версии кода и можно было легче возвращаться.
Широко используются при командной разработке, но и при индивидуальной тоже дают свои плюсы.

## Хранилище
Нативная система хранения версий для 1С. Работает только с конфигуратором.

## git

Удаленные репозитории:
GitHub
GitLab
Bitbucket 

# Прототипирование
Система программ для быстрого создания прототипов. Позволяет без конфигурирования сделать макет формы.

## MockPlus 
Про него рассказывали на партнерском семинаре

## mock1c
Энтузиасты сделали отдельный механизм

# Повышение качества продуктов
Автоматизированное тестирование для 1С

## Автоматизированное тестирование
## 1С:Сценарное тестирование
Инструмент от вендора, который позволяет строить автотесты

## 1С:Тестировщик
Легкая версия 1С:Сценарное тестирование
## Vanessa Behavior 
Инструмент от разработчиков, который тоже позволяет строить автотесты

## xUnitFor1C
Юнит тесты для 1С. Сторонний механизм

## Статический анализ текста
### Синтаксическая проверка конфигурации

### 1С:Автоматизированная проверка конфигураций

### Плагин для SonarQube

## Прочее

### Code-review
Проведение обзора кода, чтобы исключить ошибки или типа того

### Стандарты разработки
1С публикует стандарты разработки, чтобы решения были качественные

### Allure
Инструмент для красивого отображения результатов тестирования

# CI/CD

### Gitlab CI

### Travis

### Github CI

### Jenkins

### Docker

# Интеграции


### 1С:Аналитика

### Телеграмм бот

### Rabbit MQ

### Kafka

### Power BI

# Продуктивность

## Трекеры задач
### Jira

### Bitrix24

### Todoist

### Wunderlinst

## Базы знаний

### Notion

### Confluence

### Wiki


# Благодарность
Если статья была полезная или просто хотите поддержать автора,
то можете купить мне кофе - https://yoomoney.ru/to/410011910320096
