# Получить описание коммуникации crm.activity.communication.fields

{% note warning "Мы еще обновляем эту страницу" %}

Тут может не хватать некоторых данных — дополним в ближайшее время

{% endnote %}

{% if build == 'dev' %}

{% note alert "TO-DO _не выгружается на prod_" %}

- отсутствуют примеры
- отсутствует ответ в случае успеха
- отсутствует ответ в случае ошибки

{% endnote %}

{% endif %}

> Scope: [`crm`](../../../scopes/permissions.md)
>
> Кто может выполнять метод: любой пользователь

Метод `crm.activity.communication.fields` возвращает описание коммуникации для активности. Коммуникации хранят номера телефонов в звонках, email-адреса в письмах, имена во встречах.

## Параметры

Без параметров

## Примеры

{% list tabs %}

- JS

    ```js
    BX24.callMethod(
        "crm.activity.communication.fields",
        {},
        function(result)
        {
            if(result.error())
                console.error(result.error());
            else
                console.dir(result.data());
        }
    );
    ```

{% endlist %}

{% include [Сноска о примерах](../../../../_includes/examples.md) %}