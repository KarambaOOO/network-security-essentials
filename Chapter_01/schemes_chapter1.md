
Из книги “Network Security Essentials” (William Stallings)

Цель главы:
Понять, зачем вообще нужна информационная безопасность, какие у неё задачи и какие бывают атаки.

Основные понятия и перевод
               1. Информационная безопасность (Information Security)

3 главные цели:

Цель	                 На английском	        Объяснение
Конфиденциальность	   Confidentiality	      Защита данных от чужих глаз
Целостность	           Integrity	Данные      не должны быть подделаны
Доступность	           Availability	        Доступ к данным должен быть всегда

 Пример: 
если кто-то украл логин/пароль — нарушена конфиденциальность,
если изменил файл — целостность,
если завалил сервер DDoS-атакой — доступность.

              2. Типы атак

Тип              	Обозначение	        Пример
Пассивная	        Passive attack	    Подслушивание трафика (например, Wireshark)
Активная	        Active attack	      Изменение данных, подмена, внедрение зловреда

    Пассивная — атакующий просто читает, не вмешивается
    Активная — атакующий что-то делает с данными (подменяет, атакует)

             3. Механизмы безопасности (Security Mechanisms) 

Механизм	         Назначение
Шифрование         (Encryption)	Спрятать смысл сообщения
Хэширование	       Проверка целостности
Аутентификация	   Проверка «ты ли это?»
Контроль доступа	 У кого есть права на доступ
Журналирование	   Логирование событий
Фаерволы	         Защита от нежелательного трафика

             4. Службы безопасности (Security Services)
Служба	                  Объяснение
Конфиденциальность	      Данные не читаются посторонними
Аутентификация	          Проверка личности отправителя
Контроль доступа	        Разрешение/запрет доступа
Целостность данных	      Защита от изменения
Невозможность отказа	    Подпись, доказывающая факт действия (non-repudiation)

   Суть главы:
Безопасность — это не только защита от хакеров, но и целая система из:
целей (CIA — Confidentiality, Integrity, Availability)
угроз (пассивных и активных атак)
механизмов (шифрование, хэши, контроль)
служб (аутентификация, фаервол, логирование).

## 🛡️ Security Principles: CIA + AA

A summarized table of the five key principles of information security, including examples for each with varying impact levels.

| **Principle**       | **Definition**                                                                                 | **High Impact Example**                       | **Moderate Impact Example**         | **Low Impact Example**                   |
| ------------------- | ---------------------------------------------------------------------------------------------- | --------------------------------------------- | ----------------------------------- | ---------------------------------------- |
| **Confidentiality** | Protection from unauthorized access or disclosure of data.                                     | Student grade records (FERPA protected)       | Student enrollment records          | Public faculty directory                 |
| **Integrity**       | Ensuring data accuracy, consistency, and trustworthiness.                                      | Patient allergy data in a hospital database   | User forum with editable posts      | Personal hobby blog                      |
| **Availability**    | Guaranteeing timely and reliable access to systems and data.                                   | Airline flight scheduling system              | Company website with product info   | Personal blog site                       |
| **Authenticity**    | Confidence that users, messages, or systems are genuine and unaltered.                         | Bank system login and transaction validation  | Internal email-based authentication | Login form on a fan forum                |
| **Accountability**  | Ability to trace actions to responsible entities. Supports logging, forensics, and deterrence. | Audit trail in healthcare or e-voting systems | Internal wiki with change history   | Comment logging on entertainment website |

> This table supports understanding of core security objectives used in modern cybersecurity models, especially in assessing threats and designing protective systems.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 🛡️ Расширенная модель безопасности: CIA + AA

Эта таблица описывает 5 ключевых принципов информационной безопасности: классическую **триаду CIA** (Confidentiality, Integrity, Availability), а также два дополнительных принципа: **Authenticity** и **Accountability**.

| **Принцип**                            | **Определение**                                                                                                                                        | **Пример с высоким уровнем важности**                                               | **Умеренный уровень**                                          | **Низкий уровень**                              |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|----------------------------------------------------------------|---------------------------------------------------------------|
| **Конфиденциальность (Confidentiality)** | Защита от несанкционированного доступа и раскрытия информации.                                                                                       | Оценки студентов (регулируется FERPA)                                             | Данные о зачислении студентов                                  | Публичные списки на сайте                       |
| **Целостность (Integrity)**            | Гарантия точности, полноты и достоверности информации.                                                                                                 | Медицинская карта пациента                                                         | Форум зарегистрированных пользователей                         | Личный блог                                     |
| **Доступность (Availability)**         | Обеспечение своевременного и надёжного доступа к системам и данным.                                                                                    | Система управления авиарейсами                                                      | Веб-сайт компании                                              | Хобби-сайт                                      |
| **Подлинность (Authenticity)**         | Уверенность, что пользователь, сообщение или система — настоящие и не подделаны.                                                                       | Аутентификация в онлайн-банкинге                                                  | Корпоративная почта                                            | Логин на фан-сайте                              |
| **Ответственность (Accountability)**   | Возможность проследить, кто выполнил конкретное действие. Требует логирования и идентификации.                                                         | Логи в системе электронного голосования                                         | Журнал редактирования в вики                                   | Комментарии на развлекательных сайтах           |
 
## 🔍 Примечание
- Используется градация риска: **High**, **Moderate**, **Low**.
- Подходит для быстрого анализа при оценке рисков и проектировании систем безопасности.
