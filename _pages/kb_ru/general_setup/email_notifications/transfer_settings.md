---
lang: ru
layout: article_with_sidebar
updated_at: '2018-04-26 12:22 +0400'
identifier: ref_0Yn6vP7I
title: Настройка отправки почтовых сообщений
order: 230
published: true
---
Настройка отправки - важный этап в создании почтовых уведомлений, от него зависит, прочитают ли получатели сообщения.

Для настройки почты перейдите в раздел **Настройка магазина / Уведомления по электронной почте** и откройте вкладку **Настройки отправки E-Mail**.

![1.jpg]({{site.baseurl}}/attachments/ref_0Yn6vP7I/1.jpg)

**Адрес email для использования в поле FROM** - выберите адрес, который будет стоять в поле **От** в email сообщениях покупателям и сотрудникам магазина:

- Адрес из секции **Контактная информация** - В поле **От** будет стоять адрес или адреса, указанные в разделе {% link "**Настройка магазина / Информация о магазине / Контакты**" ref_3aBNbHWr %}
- Адрес отправителя по данным сервера - Сервер почтовой связи определит отправителя автоматически.
- Указанный ниже адрес - При выборе этой опции появится поле для ввода нового адреса отправителя.

Адрес в поле **От** не совпадает с адресом **Ответить**. Адреса для поля **Ответить** будут автоматически выбираются из адресов, указанных в секции **Контактная информация**, в зависимости от типа email-сообщения.

![4.jpg]({{site.baseurl}}/attachments/ref_0Yn6vP7I/4.jpg)

**Использовать SMTP сервер** - включите опцию, чтобы использовать SMTP протокол для отправки сообщений. При активации опции откроются поля настройки, укажите сервер, порт, имя пользователя, пароль и тип защищённого соединения. Если на сервере настроена {% link "фоновая обработка задач" ref_queue %}, ускоряется отправка писем и повышается производительность сайта.

Также, в качестве почтовой службы магазина можно настроить модуль [Mandrill](https://market.x-cart.com/addons/mandrill-transactional-emails-integration.html "Настройка отправки почтовых сообщений").

![2.jpg]({{site.baseurl}}/attachments/ref_0Yn6vP7I/2.jpg)

**Сохраните** настройки и отправьте тестовое сообщение в секции **Проверка параметров электронной почты**. Проверьте правильность настройки почты с помощью сервиса {% link "**Mail Tester**" ref_5hU36ima %}.

![3.jpg]({{site.baseurl}}/attachments/ref_0Yn6vP7I/3.jpg)
