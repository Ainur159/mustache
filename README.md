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

        1. создание, добавление и изменение элемента  
![image](https://github.com/user-attachments/assets/850c947b-b6f0-46af-8a25-e6d26ae07d2a)

        2. вывод массива  
![image](https://github.com/user-attachments/assets/95515a45-6ddf-496b-977b-3741f6f41ea8)

        3. создание подмассива в элементе массива  
![image](https://github.com/user-attachments/assets/466504ce-5e72-4904-a8f3-0c70e189891c)

        4. вывод подмассива  
![image](https://github.com/user-attachments/assets/10413b90-8c18-49f2-852a-bcd2d07a8a08)


    3. Работа с условиями  
Шаблон вывода: ***{{#if_setting}}...then content{{/if_setting}}{{^if_setting}}...else content{{/if_setting}}***

        1. Примитивные настройки  
![image](https://github.com/user-attachments/assets/887532a1-af0e-4881-87a7-79d6a7264e65)
![image](https://github.com/user-attachments/assets/3354c9f8-4760-4bd0-828e-3348d596312e)



        2. Массивы  
![image](https://github.com/user-attachments/assets/7f960b1c-f958-45c9-8a3a-4ea9c871420b)  
![image](https://github.com/user-attachments/assets/4ca2a966-4e20-45da-999b-0f76b94f1f5d)



2. Работа с встроенными функцяими  
Объект lowcode позволяет работать с дополнительным функционалом    

    1. Значение атрибута  
Шаблон вывода: ***{{#lowcode.object.attr}}<ident_path>{{/lowcode.object.attr}}***  
![image](https://github.com/user-attachments/assets/e34502d8-08f2-450d-b8d9-57ccab7c44fa)


    2. Ссылка на файл  
Шаблон вывода: ***{{#lowcode.object.file}}<id>{{/lowcode.object.file}}***   
![image](https://github.com/user-attachments/assets/03c1d8d9-57a5-4d0c-a71a-648a2586c214)


    3. Стиль  
Шаблон вывода: ***{{#lowcode.object.style}}<id>{{/lowcode.object.id}}***  
![image](https://github.com/user-attachments/assets/e04bb095-9706-4d62-9361-13155553ef9b)


    4. Локализация  
Значение берется из [tolgee]([https://tolgee.k8s-ingress-nginx.greendatasoft.ru/projects/2](https://tolgee.k8s-ingress-nginx.greendatasoft.ru/projects/2/translations)) (Пользователь: readonly@readonly.ru|readonly)    
Шаблон вывода: ***{{#lowcode.theme.ln}}<ident>{{/lowcode.theme.ln}}***  
![image](https://github.com/user-attachments/assets/13a85677-4031-468a-8f93-56a6b30cff27)


    5. Переменные тем  
Шаблон вывода: ***{{#lowcode.theme.vars}}<variableName>{{/lowcode.theme.vars}}***  
![image](https://github.com/user-attachments/assets/a5e6fe5a-f08d-47b3-b19f-9f0b0ec45618)


3. Защита  
Из шаблонов перед выводов будут удаляться события на элементах, а также элементы ***script***, ***style***, чтобы не нарушить работу и внешний вид системы  
![image](https://github.com/user-attachments/assets/24c0582f-8fc1-4e73-bfe4-43983322414f)


