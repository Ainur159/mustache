### Документация библиотеки
https://www.npmjs.com/package/mustache

### Компоненты  
Можно использовать все базовые тэги HTML, а также Дизайн компоненты из системы  
https://nl.gdcloud.org/?path=/docs/components-components-overview--page.  
Пример использования текстового поля  
https://nl.gdcloud.org/?path=/docs/components-textfield--text-field-example  
![image](https://github.com/user-attachments/assets/1153a43f-7da4-480d-acd0-ca6989c93dbd)



### Использование в системе  

1. Работа с настройками  
Благодаря двум шаблонам мы можем создавать собственные настройки и выводить их в любом виде  
Шаблон вывода: ***{{param}}***

    1. Примитивные настройки
        1. создание и изменение   
       ![image](https://github.com/user-attachments/assets/e2c4bc4a-006c-4953-bac4-f76f8de214b7)

        2. вывод  
![image](https://github.com/user-attachments/assets/5cc55f60-c8eb-4f54-a200-a7cec1cdcad8)


    2. Массивы и события  
Шаблон вывода: ***{{#array}}...{{/array}}***

        1. создание и добавление в массив
        2. изменение значений объекта массива
        3. вывод массива

    3. Работа с условиями  
Шаблон вывода: ***{{#if_setting}}...then content{{/if_setting}}{{^if_setting}}...else content{{/if_setting}}***

    1. Примитивные настройки
    2. Массивы

2. Работа с встроенными функцяими  
Объект lowcode позволяет работать с дополнительным функционалом    

    1. Значение атрибута  
Шаблон вывода: ***{{#lowcode.object.attr}}<ident_path>{{/lowcode.object.attr}}***

    2. Ссылка на файл  
Шаблон вывода: ***{{#lowcode.object.file}}<id>{{/lowcode.object.file}}***

    3. Стиль  
Шаблон вывода: ***{{#lowcode.object.style}}<id>{{/lowcode.object.id}}***

    4. Локализация  
Значение берется из [tolgee](https://tolgee.k8s-ingress-nginx.greendatasoft.ru/projects/2)   
Шаблон вывода: ***{{#lowcode.theme.ln}}<ident>{{/lowcode.theme.ln}}***

    5. Переменные тем  
Шаблон вывода: ***{{#lowcode.theme.vars}}<variableName>{{/lowcode.theme.vars}}***
