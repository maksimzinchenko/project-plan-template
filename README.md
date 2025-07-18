# project-plan-template

Agile project plan template.

```
/project-plan
│
├── 0-PROJECT_OVERVIEW.md
├── 1-DELIVERABLES.md
├── 2-TIMELINE.md
├── 3-SCOPE.md
├── 4-TEAM_ROLES.md
├── 5-RISKS.md
├── 6-COMMUNICATION_PLAN.md
├── 7-BUDGET.md
├── 8-APPROVALS.md
└── 9-CHANGELOG.md

```

## File Descriptions

- **0-PROJECT_OVERVIEW.md** — Обзор проекта: цели, видение, целевая аудитория, критерии успеха
- **1-DELIVERABLES.md** — Поставляемые результаты (deliverables) по этапам и версиям
- **2-TIMELINE.md** — Таймлайн проекта и ключевые даты (milestones)
- **3-SCOPE.md** — Границы проекта: что входит и что исключено
- **4-TEAM_ROLES.md** — Команда проекта и распределение ролей
- **5-RISKS.md** — Реестр рисков проекта и планы их минимизации
- **6-COMMUNICATION_PLAN.md** — План коммуникаций: форматы, каналы, частота взаимодействий
- **7-BUDGET.md** — Бюджет проекта и распределение затрат
- **8-APPROVALS.md** — История всех утверждений и согласований по проекту
- **9-CHANGELOG.md** — История всех изменений проектной документации
```

Так структура отображается корректно, а описания к файлам — аккуратно вынесены ниже.




### ✅ **Что должно быть в `PROJECT_OVERVIEW.md`** и кто его ведет.


# Пояснение

| Раздел           | Зачем нужен                            |
| ---------------- | -------------------------------------- |
| Project Summary  | Быстрое понимание проекта новичками    |
| Business Goals   | Видно, зачем бизнесу этот проект       |
| Product Vision   | Долгосрочная ориентация                |
| Stakeholders     | Контакты всех, кто влияет на проект    |
| Project Owner    | Кто представляет бизнес в команде      |
| Key Dates        | Вехи проекта                           |
| Scope Summary    | Границы проекта                        |
| Success Criteria | Чёткие метрики успеха                  |
| Constraints      | Что ограничивает проект                |
| Assumptions      | Что считаем верным, но не подтверждено |
| References       | Быстрый доступ к связанным файлам      |

### ✅ **Кто ведёт `0-PROJECT_OVERVIEW.md`**

`PROJECT_OVERVIEW.md` ведёт и обновляет в первую очередь:

| Роль                              | Ответственность                                                                                                                     |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**            | Основной владелец файла. Составляет начальную версию, фиксирует цели, визию, границы проекта, критерии успеха                       |
| **Project Manager** *(если есть)* | Может дополнять информацию по срокам, ограничениям, коммуникационным каналам                                                        |
| **Stakeholders / Заказчик**       | Предоставляют данные и подтверждают цели, критерии успеха, бизнес-цели                                                              |
| **Scrum Master**                  | Обычно не участвует, но может помочь в оформлении или обновлении организационной части (процессы, коммуникации), если это требуется |

---

### ✅ **Когда обновляется**

* В начале проекта — создаётся Product Owner.
* При изменении:

  * целей проекта
  * состава команды
  * бизнес-стратегии
  * критериев успеха
* Обычно обновляется **после каждого крупного релиза или пересмотра Product Vision.**

---

### ✅ **Практика**

Можно зафиксировать:

* **ответственного за ведение:** Product Owner
* **reviewer:** Project Manager (если есть), Stakeholders

Также хорошая практика:

* Все изменения вносить через **Pull Request**, чтобы другие участники видели и могли прокомментировать.
* В `CHANGELOG.md` фиксировать ключевые правки в Overview.


### ✅ **Что должно быть в `1-DELIVERABLES.md`** и кто его ведет.

# Deliverables

Документ описывает все ключевые результаты (deliverables), которые команда обязуется поставить в рамках проекта. Каждый deliverable связан с этапом или версией продукта.


### ✅ **Кто ведёт `1-DELIVERABLES.md`**

| Роль                              | Ответственность                                                                                                                                                         |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**            | Основной владелец файла. Формирует и обновляет список всех **поставляемых результатов (deliverables)** проекта. Уточняет состав и приоритеты фич с учётом бизнес-целей. |
| **Project Manager** *(если есть)* | Может помогать фиксировать сроки поставок и контролировать актуальность планируемых дат.                                                                                |
| **Tech Lead / Development Team**  | Уточняют **состав функционала deliverables**, дают технические комментарии (что реально реализовать, что входит в версию).                                              |
| **Stakeholders / Заказчик**       | Подтверждают, что deliverables соответствуют их ожиданиям.                                                                                                              |

---

### ✅ **Когда обновляется**

* В начале проекта — составляется исходный список deliverables (обычно после формирования Product Vision).
* После каждого Sprint Review или большого релиза — если:

  * появились новые deliverables
  * изменился состав версий
  * изменились приоритеты или сроки

---

### ✅ **Резюме**

| Задача                              | Кто выполняет                   |
| ----------------------------------- | ------------------------------- |
| Создать первичный `DELIVERABLES.md` | Product Owner                   |
| Технически уточнить состав фич      | Tech Lead / команда             |
| Зафиксировать даты поставок         | Product Owner + Project Manager |
| Подтвердить приоритеты и ожидания   | Stakeholders                    |




### ✅ **Кто ведёт `TIMELINE.md`**

| Роль                             | Ответственность                                                                                                                                               |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**           | Ведущий и основной владелец файла. Формирует и обновляет таймлайн исходя из **бизнес-приоритетов и целей**, Roadmap и Product Backlog.                        |
| **Project Manager (если есть)**  | В проектах с Project Manager он обычно **ведёт и актуализирует таймлайн**. Контролирует даты, фиксирует сдвиги сроков, отслеживает риски, влияющие на график. |
| **Scrum Master**                 | Помогает **поддерживать актуальность таймлайна** после спринтов, ретроспектив и Review, особенно если возникли препятствия или изменения в процессе.          |
| **Tech Lead / Development Team** | Дают **оценку реалистичности сроков** и указывают на технические блокеры, которые могут повлиять на таймлайн.                                                 |

---

### ✅ **Когда обновлять `TIMELINE.md`**

* После составления Roadmap и Product Backlog.
* В начале проекта — формируется изначальный таймлайн.
* После каждого Sprint Review — если появились изменения в приоритетах или обнаружены задержки.
* При выявлении новых рисков, которые влияют на сроки.
* При утверждении новых этапов проекта или новых Deliverables.

---

### ✅ **Типичная схема обновления**

| Событие                           | Кто обновляет TIMELINE.md                    |
| --------------------------------- | -------------------------------------------- |
| Старт проекта                     | Product Owner / Project Manager              |
| После спринта                     | Product Owner, Scrum Master помогает         |
| Изменение приоритетов заказчика   | Product Owner                                |
| Появление технических препятствий | Product Owner после консультации с Tech Lead |

---

### ✅ **Итог**

\| Ведёт | Product Owner **или** Project Manager |
\| Помогает | Scrum Master, Tech Lead, команда |
\| Утверждает | Stakeholders / Заказчик (если критичные изменения) |


### ✅ **Что должно быть в `3-SCOPE.md`**

`SCOPE.md` — это документ, который фиксирует:

* **Что входит в объём проекта** (что будет сделано)
* **Что не входит в проект** (границы и исключения)
* **Критерии завершённости** — по каким признакам понимаем, что объём проекта выполнен
* Дополнительно:

  * Ограничения по технологиям, платформам
  * Явные исключения или отложенные фичи

---

### ✅ **Кто ведёт `3-SCOPE.md`**

| Роль                              | Ответственность                                                                                                                     |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**            | Основной владелец. Формирует и актуализирует список того, что входит и не входит в проект, опираясь на Product Vision и бизнес-цели |
| **Project Manager** *(если есть)* | Может фиксировать ограничения, уточнять границы проекта в зависимости от бюджета и сроков                                           |
| **Tech Lead / Development Team**  | Помогают уточнить технические ограничения, дают рекомендации по реалистичности объёма                                               |
| **Stakeholders / Заказчик**       | Подтверждают, что Scope соответствует их ожиданиям и бизнес-целям                                                                   |

---

### ✅ **Когда обновлять**

* В начале проекта при формировании видения и backlog
* После крупных изменений Product Backlog
* После Sprint Reviews (если появились изменения в требованиях)
* При изменении бюджета, сроков, ресурсов

---

## ✅ **Итоги**

| Файл         | Кто ведёт         | Когда обновляется                           |
| ------------ | ----------------- | ------------------------------------------- |
| `3-SCOPE.md` | **Product Owner** | В начале проекта и после значимых изменений |

---

### ✅ **Что должно быть в `4-TEAM_ROLES.md` и кто его ведет** 

`TEAM_ROLES.md` — это документ, где фиксируются:

* Состав всей команды проекта
* Роли и зоны ответственности каждого участника
* Контактная информация (если нужно)
* Замены или резервные роли (при необходимости)
* При необходимости — время участия (если не все участники фуллтайм)

### ✅ **Кто ведёт `4-TEAM_ROLES.md`**

| Роль                                   | Ответственность                                                                                   |
| -------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**                 | Основной владелец. Формирует состав, фиксирует роли и ответственность, обновляет при изменениях   |
| **Project Manager** *(если есть)*      | Может помогать поддерживать актуальность: фиксировать рабочее время, занятость, контактные данные |
| **Scrum Master**                       | Может инициировать обновление, если меняется состав Scrum-команды или роли                        |
| **HR / People Ops** *(если участвуют)* | Если команда большая, могут помочь зафиксировать занятость и график работы                        |

---

### ✅ **Когда обновлять**

* В начале проекта — фиксируется базовый состав.
* При любом изменении состава или ролей:

  * Новый участник
  * Перераспределение зон ответственности
  * Уход участника
* При переходе к новому этапу проекта (если состав меняется)

---

### ✅ **Резюме**

| Файл              | Кто ведёт                                        | Когда обновлять                                   |
| ----------------- | ------------------------------------------------ | ------------------------------------------------- |
| `4-TEAM_ROLES.md` | **Product Owner**, при поддержке Project Manager | В начале проекта и при любых изменениях в команде |


### ✅ **Что должно быть в `5-RISKS.md` и кто его ведет**

`RISKS.md` — это документ, который фиксирует:

* Все известные **риски проекта**
* **Оценку вероятности и влияния каждого риска**
* **Стратегию управления риском** (что делать, если риск реализуется)
* **Ответственного** за мониторинг риска
* Текущий статус (активен / устранён / реализовался)

---
## ✅ **Кто ведёт `5-RISKS.md`**

| Роль                              | Ответственность                                                                                                                   |
| --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**            | Основной владелец. Формирует и фиксирует все бизнес- и продуктовые риски.                                                         |
| **Project Manager** *(если есть)* | Отвечает за **регулярное обновление**, мониторинг рисков, фиксирует статус, добавляет новые риски, особенно по срокам и ресурсам. |
| **Scrum Master**                  | Может помочь выявить **процессные риски** и фиксировать их в документе.                                                           |
| **Tech Lead / QA**                | Сообщают о технических и качественных рисках.                                                                                     |

---

## ✅ **Когда обновлять**

* В начале проекта — создать базовый список рисков.
* После каждого **Sprint Review и Retrospective** — могут появиться новые риски.
* При изменении сроков, состава команды, при изменении Scope.
* При появлении новых внешних факторов.

---

## ✅ **Резюме**

| Файл         | Кто ведёт                               | Когда обновлять                                            |
| ------------ | --------------------------------------- | ---------------------------------------------------------- |
| `5-RISKS.md` | **Product Owner** / **Project Manager** | В начале проекта, после каждого спринта, при новых угрозах |


### ✅ **Что должно быть в `6-COMMUNICATION_PLAN.md`**

`COMMUNICATION_PLAN.md` — это документ, который определяет:

* **Как, когда и через какие каналы** участники проекта должны общаться
* Кто отвечает за какие **типы коммуникации**
* **Формат и регулярность встреч**
* Правила **отчётности и эскалации проблем**
* Используемые **инструменты коммуникации**

---

## ✅ **Кто ведёт `6-COMMUNICATION_PLAN.md`**

| Роль                              | Ответственность                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------- |
| **Scrum Master**                  | Основной владелец. Ведёт и поддерживает план коммуникации, следит за его соблюдением. |
| **Product Owner**                 | Вносит изменения, касающиеся общения с заказчиком, требований и фидбэка.              |
| **Project Manager** *(если есть)* | Добавляет информацию по отчётности, эскалации и межкомандным коммуникациям.           |

---

## ✅ **Когда обновлять**

* В начале проекта — составляется начальный план.
* При смене состава команды или каналов общения.
* При возникновении проблем с коммуникацией (выявленных на ретроспективах).
* При подключении новых стейкхолдеров.

---

## ✅ **Резюме**

| Файл                      | Кто ведёт                                           | Когда обновлять                                                         |
| ------------------------- | --------------------------------------------------- | ----------------------------------------------------------------------- |
| `6-COMMUNICATION_PLAN.md` | **Scrum Master** (при участии PO и Project Manager) | В начале проекта, при смене форматов взаимодействия, после ретроспектив |


### ✅ **Что должно быть в `7-BUDGET.md`**

`BUDGET.md` — это документ, в котором фиксируются:

* **Общий бюджет проекта**
* **План распределения бюджета** (по этапам, категориям затрат)
* **Оценка фактических расходов** (опционально)
* **Запас на риски и непредвиденные расходы**
* При необходимости — **финансовые условия с заказчиком** (например, условия платежей)

---

## ✅ **Кто ведёт `7-BUDGET.md`**

| Роль                                 | Ответственность                                                                                         |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------- |
| **Project Manager**                  | Основной владелец. Составляет бюджет, отслеживает расходование, актуализирует при изменениях в проекте. |
| **Product Owner**                    | Участвует в формировании бюджета, особенно по продуктовым приоритетам и составу работ.                  |
| **Finance / Accounting (если есть)** | Контролирует фактические платежи, может дополнять документ.                                             |
| **Stakeholders / Заказчик**          | Подтверждают бюджет и график платежей.                                                                  |

---

## ✅ **Когда обновлять**

* В начале проекта — формируется базовый бюджет.
* При изменении Scope, сроков, команды.
* После каждого этапа — фиксировать фактические расходы (если необходимо).
* При появлении новых рисков и корректировке запасов.

---

## ✅ **Резюме**

| Файл          | Кто ведёт                                          | Когда обновлять                                              |
| ------------- | -------------------------------------------------- | ------------------------------------------------------------ |
| `7-BUDGET.md` | **Project Manager** (при участии PO и финансистов) | В начале проекта, после изменений Scope, после каждого этапа |


### ✅ **Что должно быть в `8-APPROVALS.md`**

`APPROVALS.md` — это документ, где фиксируются:

* **Кто и когда официально утвердил** ключевые документы, этапы или решения в проекте
* Какие **документы или версии** были утверждены
* Кто является **уполномоченным лицом для утверждения** (Product Owner, заказчик, Project Manager и т.д.)
* При необходимости — **комментарии или условия утверждения**

---
## ✅ **Кто ведёт `8-APPROVALS.md`**

| Роль                        | Ответственность                                                                                    |
| --------------------------- | -------------------------------------------------------------------------------------------------- |
| **Project Manager**         | Основной владелец. Фиксирует все утверждения, хранит историю согласований, следит за актуальностью |
| **Product Owner**           | Участвует в согласовании документов и изменений, инициирует фиксацию в `APPROVALS.md`              |
| **Stakeholders / Заказчик** | Подтверждают ключевые документы, этапы, изменения                                                  |

---

## ✅ **Когда обновлять**

* После утверждения любого ключевого документа (Scope, Product Overview, Deliverables, Budget и т.д.)
* После каждого завершённого Milestone (MVP, релиз)
* При изменении Scope, бюджета, сроков
* При появлении новых версий утверждённых документов

---

## ✅ **Резюме**

| Файл             | Кто ведёт           | Когда обновлять                                          |
| ---------------- | ------------------- | -------------------------------------------------------- |
| `8-APPROVALS.md` | **Project Manager** | После каждого утверждения документа, этапа или изменения |

### ✅ **Что должно быть в `9-CHANGELOG.md`**

`CHANGELOG.md` — это файл, где фиксируются **все изменения в проектной документации и ключевых артефактах проекта**.
Он помогает отслеживать:

* Что изменилось в планах, сроках, составе команды, deliverables, scope и др.
* Когда это произошло
* Кто автор изменения
* Причина изменений (опционально)

---

## ✅ **Кто ведёт `9-CHANGELOG.md`**

| Роль                         | Ответственность                                                                                                |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Project Manager**          | Основной владелец. Вносит записи при любых изменениях проектной документации, сроков, бюджета, состава команды |
| **Product Owner**            | Вносит записи при изменениях Product Vision, Deliverables, Scope, которые сам инициирует                       |
| **Tech Lead / Scrum Master** | Могут инициировать запись, если изменяются технические решения, процесс, команда                               |

---

## ✅ **Когда обновлять**

* После любого **существенного изменения** в:

  * Scope
  * Timeline
  * Deliverables
  * Команде
  * Рисках
  * Бюджете
  * Коммуникациях
* При выпуске **новой версии плана или документа**

---

## ✅ **Резюме**

| Файл             | Кто ведёт                          | Когда обновлять                                            |
| ---------------- | ---------------------------------- | ---------------------------------------------------------- |
| `9-CHANGELOG.md` | **Project Manager**, Product Owner | После каждого значимого изменения в проектной документации |



Исходя из предложенной структуры проектных файлов, вот **необходимые роли для их ведения и сопровождения**:

---

| Файл                         | Роль, ведущая документ                    | Дополнительные роли                                                                    |
| ---------------------------- | ----------------------------------------- | -------------------------------------------------------------------------------------- |
| **0-PROJECT\_OVERVIEW\.md**  | **Product Owner**                         | Project Manager, Stakeholders (для согласования)                                       |
| **1-DELIVERABLES.md**        | **Product Owner**                         | Tech Lead (уточнение состава фич), Project Manager (если фиксируются даты)             |
| **2-TIMELINE.md**            | **Project Manager** или **Product Owner** | Scrum Master (сопровождение статусов), Tech Lead (оценка реализуемости сроков)         |
| **3-SCOPE.md**               | **Product Owner**                         | Project Manager (для контроля границ), Tech Lead (технические ограничения)             |
| **4-TEAM\_ROLES.md**         | **Product Owner**                         | Project Manager (для актуализации времени участия и ролей)                             |
| **5-RISKS.md**               | **Product Owner** / **Project Manager**   | Scrum Master (процессные риски), Tech Lead (технические риски), QA (риски качества)    |
| **6-COMMUNICATION\_PLAN.md** | **Scrum Master**                          | Product Owner (каналы заказчика), Project Manager (отчётность, внешняя коммуникация)   |
| **7-BUDGET.md**              | **Project Manager**                       | Product Owner (приоритизация трат), Finance / Accounting (если есть)                   |
| **8-APPROVALS.md**           | **Project Manager**                       | Product Owner (инициирует согласования), Stakeholders (утверждают)                     |
| **9-CHANGELOG.md**           | **Project Manager**                       | Product Owner (если изменения инициированы им), Scrum Master (если касается процессов) |

---

## ✅ **Итоговый список необходимых ролей**

| Роль                                     | Функция в проекте                                               |
| ---------------------------------------- | --------------------------------------------------------------- |
| **Product Owner**                        | Формирует требования, видение, scope, deliverables              |
| **Project Manager**                      | Управляет сроками, бюджетом, рисками, changelog, согласованиями |
| **Scrum Master**                         | Ведёт план коммуникаций, следит за процессами                   |
| **Tech Lead**                            | Уточняет технические детали, ограничения, оценивает сроки       |
| **QA Engineer**                          | Предоставляет данные о рисках качества                          |
| **Finance / Accounting** *(опционально)* | Контролируют бюджет и расходы                                   |
| **Stakeholders / Заказчик**              | Утверждают документацию, дают фидбэк                            |

---

Если проект небольшой, **Project Manager и Product Owner** могут быть совмещены в одном человеке.


