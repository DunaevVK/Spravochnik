# Spravochnik
[Электронный телефонный справочник сотрудников.](https://dunaevvk.github.io/Spravochnik/)  
Используются технологии: **HTML, CSS (SASS, SCSS), MySQL, PHP**.  
Так как доступа к серверу нет, то представлена только статичная верстка, многостраничник.  
На главной странице, как пример, созданы 2 элемента поиска (1 - обычный input, 2 - input c использованием **datalist**). Сам поиск работает на сервере.
В навигации активна только кнопка **"Справочник"**.  

На странице "Справочник" (spravochnikWorkers.html) по умолчанию отображается полный список сотрудников (данные берутся из БД на сервере). Доступны 2 ссылки для навигации ("Сотрудники" и "Подразделения"). Навигация по алфавиту не доступна, т.к. работает только с БД на сервере. При нажатии на ФИО сотрудника (фамилия и имя-отчество разделены, т.к. используются flex-shrink, flex-grow, flex-basis для выравнивания столбцов) осуществляется переход на страницу конкретного сотрудника с более подробной информацией.  

На странице "Подразделения"(spravochnikOtdel.html) по умолчанию отображается полный список всех отделов. Добавлена анимация на клик, с раскрытием всех подразделений отделов (данные берутся из БД на сервере).  

На странице конкретного сотрудника (spravochnikWorkersPerson.html) отображается подробная информация о сотруднике. Также созданы breadcrumbs (данные берутся из БД на сервере). При клике по breadcrumbs осуществляется переход на страницу Отделов и раскрывается необходимый отдел.  

На данный момент я могу переписать всё на **Vue**, с использованием API, компонентов, роутера и сделать SPA.
