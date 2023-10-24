# О проекте Spomeet

| Команда | Должность | Фото |
| ------------- | ------------- | ------------- |
| Малик| Старший Frontend |  |
| Дмитрий | Старший Backend|  |
| Гриша | Backend |  |
| Никита | Backend |  |
| Андрей | Backend |  |
| Илья | Backend | width = "100px"![a04dabc4-57b1-4644-88ab-4c3532bdffac](https://github.com/spomeet/info-spomeet/assets/126795153/2114ad93-56c2-4660-a155-c49e7f6cc176) |

| Алексей | Product-менеджер |  |



## Документация ПО

1) Эксплуатация информационной системы  
В упрощенном варианте системы, установка дополнительного ПО не требуется, достаточно наличия браузера, действующего телефона и/или почты. В расширенном варианте – дополнительное приложение или его мобильная версия, с возможностью обновления.  
Эксплуатация предполагает  
А) создание базы данных игроков с указанием основных параметров, способов связи. Данные вносятся после модерации администратором.  
Б) создание личного кабинета игрока на форуме. 
В) форма заявки команды (указание адреса и времени домашнего зала, если необходим для мероприятия). Список заявленных команд. (на модерации\после)  
Г) формирование таблиц мероприятий по выбранной форме или свободной (турниры и регулярный чемпионат).  
С) лента новостей, с возможностью поиска.  
Таким образом основным сопровождением системы будет являться поддержание системы работоспособной, модерация выбранных разделов команд, архивация данных и резервное восстановление.  
Срок ответа на обращение по возникшей проблеме 3 часа в рабочее время с 9 до 21 по Московскому времени. Резервное копирование и исправление ошибок – с 21 часа пятницы до 9 часов субботы, на основании копий сделанных заказчиком (п.2.12 договора).  
Если количество обращений превышает 15 в месяц, оплачиваются как консультации дополнительно.  
2) Внесение изменений в информационную систему.  
Внесение изменений возможно на основе как пожеланий сообщества конечных пользователей, организаторов, так и аудита\консультирования.  
Дополнительные форматы команд, дополнительные поля информации – модули, индикаторы статуса игроков (в составе команды, в активном поиске и т.д.) Архивация результатов мероприятий с возможностью внесения рейтинга. Создание разделов на форуме в соответствии с активными мероприятиями. Возможность использования гео-локации. Создание модуля-раздела болельщика – показывающего на карте гео-локации мероприятий из регулярного чемпионата и турниров. Возможно автоматическое  
формирование групп на основе локации домашних залов и удобного времени аренды. Возможность заполнять результаты некоторых мероприятий самостоятельно, отправляя на модерацию.  
Расширение возможностей приложения в виде уведомлений о приглашениях в команду, начале регистрации на мероприятия, проведении мероприятий поблизости, на основании выбора интересов.

<hr>

## Инструкция по GIT

- [Правила работы с Git на проекте](#Правила-работы-с-Git-на-проекте)\
    1.<u>Основные команды</u>\
       1.1 [git init](#правила-работы-с-git-на-проекте)\
       1.2. [git clone](#правила-работы-с-git-на-проекте)\
       1.3. [git add](#правила-работы-с-git-на-проекте)\
       1.4. [git commit](#правила-работы-с-git-на-проекте)\
       1.5. [git status](#правила-работы-с-git-на-проекте)\
       1.6. [git fetch](#правила-работы-с-git-на-проекте)\
       1.7. [git push](#правила-работы-с-git-на-проекте)\
       1.8. [git pull](#правила-работы-с-git-на-проекте)\
       1.9. [git branch](#правила-работы-с-git-на-проекте)\
       1.10. [git checkout](#правила-работы-с-git-на-проекте)\
       1.11. [git merge](#правила-работы-с-git-на-проекте)\
       1.12. [git log](#правила-работы-с-git-на-проекте)\
       1.13. [git diff](#правила-работы-с-git-на-проекте)

   2.<u>Ветки Git</u>\
    2.1 [Ветка `Main`](#ветки-git)\
    2.2 [Ветка `Dev`](#ветки-git)\
    2.3 [Ветка `<Название вашей ветки>`](#ветки-git)

   3.<u>Стадии работы с Git в проекте</u>\
    3.1 [Выкачиваем последние изменения из ветки `Dev`](#стадии-работы-с-git-в-проекте)\
    3.2 [Порядок внесения изменений](#стадии-работы-с-git-в-проекте)

- [Сноски](#сноски)


## Правила работы с Git на проекте

#### <u>**Git**</u> - это распределенная система контроля версий, которая используется для управления и отслеживания изменений в исходном коде проекта. Вот некоторые основные команды Git:

1. ### <u>Основные команды</u>

    1.1 `git init`: Создает новый репозиторий Git в текущем каталоге.

    1.2 `git clone <url>`: Клонирует удаленный репозиторий на локальную машину.

    1.3 `git add <файл>`: Добавляет файлы в индекс (staging area) для последующего коммита.

    1.4 `git commit -m "<сообщение>"`: Создает коммит с сохранением изменений, добавленных в индекс, и присваивает ему сообщение.

    1.5 `git status`: Показывает текущее состояние репозитория, включая измененные, добавленные или удаленные файлы.

    1.7 `git fetch`: Получает последние изменения из удаленного репозитория, но не объединяет их с текущей веткой.

    1.8 `git push`: Загружает локальные коммиты в удаленный репозиторий.

    1.9 `git pull`: Получает и объединяет изменения из удаленного репозитория в локальный репозиторий.

    1.10 `git branch`: Показывает список существующих веток в репозитории.

    1.11 `git checkout <ветка>`: Переключается на указанную ветку.

    1.12 `git merge <ветка>`: Объединяет указанную ветку с текущей веткой.

    1.13 `git log`: Показывает историю коммитов в репозитории.

    1.14 `git diff`: Показывает различия между рабочей директорией и индексом или между коммитами.

2. ## <u>Ветки Git</u>

    2.1 Ветка `Main`: Главная ветка проекта, в неё попадают [Stable версии](#stable-версия) приложения, прошедшие [Code review](#code-review)

    2.2 Ветка `Dev`: Ветка, в которую попадают [unstable версии](#unstable-версия) проекта

    2.3 Ветка `<Название вашей ветки>`: Это ваша собственная ветка, в которой вы работаете большую часть времени. После внесения изменений вы создаете [pull request](#запрос-на-рецензию-разработчик-создает-запрос-на-рецензию-pull-request-в-системе-контроля-версий-указывая-изменения-которые-он-внес-и-ветку-которую-он-хочет-слить-с-основной-кодовой-базой) в ветку `Dev`

    ```
    <Название вашей ветки> --> (Code Review) --> Dev --> Main 
    ``` 

3. ## <u>Стадии работы с Git в проекте</u>
   
   1)Выкачиваем последние изменения из ветки `Dev`

   ```bash
   git branch dev  # переходим на ветку Dev
   git fetch --all # проверяем обновления со всех веток
   git status      # получаем текущее состояние репозитория
   git pull        # выкачиваем принятые изменения из удаленной ветки Dev на локальную
   ```

   2)Порядок внесения изменений

   ````bash
   --(Изменения)--> <ваша_ветка> --> (pull request из <ваша_ветка> в ветку Dev) --> Code review --> Внесение изменений в ветку Dev
   ````

   Когда ветка `Dev` становится достаточно стабильной, мы производим её слияние с веткой `Main`, тем самым, выпуская новый релиз проекта

   ```bash
   --(Dev: стабильный релиз)--> Main --> Production Server
   ```



## Сноски

- ### Stable версия

    **Stable версия** - это стаблильная версия проекта

- ### Unstable версия

    **Unstable версия** - это нестаблильная версия проекта, нуждающаяся в отладке и [рефакторинге](#рефакторинг)

- ### Рефакторинг

    **Рефакторинг** - Рефакторинг, или перепроектирование кода, переработка кода, равносильное преобразование алгоритмов — процесс изменения внутренней структуры программы, не затрагивающий её внешнего поведения и имеющий целью облегчить понимание её работы


- ### Code review

    **Code review (рецензирование кода)** - это процесс, в ходе которого другой разработчик проверяет и анализирует написанный код с целью обеспечения качества, выявления потенциальных проблем и улучшения его структуры.

    Вот общий процесс проведения code review:

    **Подготовка для рецензии**: Разработчик завершает свою работу над новым кодом или внесением изменений в существующий код и готовит его для рецензии. Он коммитит свои изменения и пушит их в удаленный репозиторий.

    #### **Запрос на рецензию**: Разработчик создает запрос на рецензию (pull request) в системе контроля версий, указывая изменения, которые он внес и ветку, которую он хочет слить с основной кодовой базой.

    **Рецензия**: Другой разработчик (или несколько разработчиков) берут на себя задачу рецензии кода. Они просматривают код, анализируют его структуру, логику, читаемость, соответствие стандартам кодирования и т.д. Они также могут проверять наличие потенциальных ошибок, уязвимостей или неэффективного кода.

    **Обсуждение и комментарии**: Рецензенты оставляют комментарии, предлагают улучшения, задают вопросы и выражают свои замечания по коду. Разработчик, чья работа проходит рецензию, получает уведомления о комментариях и может отвечать на них, обсуждать изменения и предлагать свои объяснения или альтернативные решения.

    **Внесение изменений**: Разработчик, чья работа проходит рецензию, вносит изменения в код на основе комментариев и предложений рецензентов. Он обсуждает их с коллегами, если это необходимо, и выполняет необходимые правки.

    **Завершение рецензии**: Когда все комментарии удовлетворены и код соответствует требованиям, рецензенты подтверждают успешное прохождение рецензии. Разработчик может продолжить процесс слияния кода с основной веткой проекта.

    > Code review способствует повышению качества кода, обмену знаниями и улучшению согласованности кодовой базы. Он также помогает выявлять и исправлять проблемы на ранних стадиях разработки, что может сэкономить время и усилия в будущем.
