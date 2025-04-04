# ArtPlast Desktop
Windows selling company application using Windows Forms, ADO.NET

---

[Google Drive Document](https://docs.google.com/document/d/1IWH6SLdk9yXwMSJtrkxAeja8QF28xwZ3z5G5jxgzDfg/edit)
---

# Техническое задание

## проект “ArtPlast Desktop”

Версия 1.0. *Виталий Повстенко*

### Содержание

1. [Общие положения](#item1)
2. [Назначение и цели создания системы](#item2)
3. [Характеристики объекта](#item3)
4. [Требование к системе](#item4)
5. [Состав и содержание проекта](#item5)
6. [Порядок контроля и приемки системы](#item6)
7. [Требования к вводу системы в эксплуатации](#item7)

---

1. ### <a name="item1"></a> Общие положения

	1.1. Наименования информационной системы

	Наименование системы - **ArtPlast Desktop**.

	1.2. Наименование предприятия Заказчика Системы и его реквизиты
	
	Заказчик - ООО “**STEP-ArtPlast**”.

	1.3. Перечень документов, на основе которых создается Система:
	
	* Техническое задание.
	* Переписка между Сторонами.

	1.4. Плановые сроки начала и окончания работ по созданию Системы
	
	* начало работ с **03.03.2019**  
	* готовность проекта к **31.03.2019**

2. ### <a name="item2"></a> Назначение и цели создания системы

	2.1. Назначение программы

	Программа для расчета стоимости металлопластикового окна.

	2.2. Цель создания программы

	Создать десктопное приложение для покупки окон, просмотр актуальных цен на материалы фирмы **ArtPlast**.

	2.3. Целевая аудитория программы

	Целевая аудитория программы представлена следующими группами пользователей:
	
	* Покупатели (клиенты компании)
	* Администраторы

	2.4. Основные задачи Программы

	Программа должна обеспечивать реализацию следующих задач:

	* База данных содержит описание всех материалов (категория, название, цвет, стоимость за квадратный метр, описание).
	* База данных содержит двух пользователей – admin и manager. Администратор может редактировать все таблицы, просматривать данные и выполнять хранимые процедуры (если такие имеются). Менеджер может только просматривать таблицы и выполнять хранимые процедуры.
	* Программа запрашивает размеры окна (ширина, высота) , количество секций, ширина рамы, размер подоконника, количество открывающихся секций, тип пластика и тип стекла и выполняет расчет стоимости.
	* Добавление и редактирование осуществляется в отдельных окнах.
	* Программа предусматривает просмотр отдельно списка материалов.
	* Список материалов отображается в ListView.
	* Реализовать поиск материала по названию, стоимости, категории или любой комбинации из выше перечисленного.

3. ### <a name="item3"></a> Характеристики объекта

	Заказчиком выступает компания аэроперевозок ООО “STEP-ArtPlast”, которая планирует выйти на новый рынок.

4. ### <a name="item4"></a> Требование к системе

	Покупатель хочет заказать металлопластиковое окно и хочет заранее узнать его стоимость. Для оформления заказа необходимо замерить размеры окна и определиться с материалами (рама, стекла, фурнитура). Для учета форс-мажорных ситуаций после всех вычислений программа к полученной сумме прибавляется 10%. Программа предусматривает редактирование базы данных, но под определенными правами.

	4.1. Требования к стилистическому оформлению Программы  

	Стилистическое оформление приложения должно соответствовать требованиям заказчика.  После согласования графического эскиза программы дизайнера с заказчиком, переделка стилистического оформления программы невозможна (за исключением незначительных поправок).

	4.2. Требования к графическому Дизайну Программы
	
	Дизайн приложения должен быть лаконичным и в то же время выглядеть стильно, современно.

	Предпочтительные цвета приложения:
	* синий
	* голубой
	* белый
	* желтый

	4.3. Требования к шрифтовому оформлению Программы

	Размер (кегль) шрифтов должен обеспечивать удобство восприятия текста при минимально допустимом размере экрана. Предпочтителен шрифт без засечек

	4.4. Требования к средствам использования Программы

	Программа должна поддерживаться операционными системами:
	*   Windows 10
	*   Windows 8.1
	*   Windows 8
	*   Windows 7

	4.5.  Программная часть проекта

	Языки программирования:
	* C#

	Клиентские технологии ( языки разметки ):
	* Windows Forms

	Системы управления базами данных:
	* MSSQL

5. ### <a name="item5"></a> Состав и содержание проекта

	5.1. Регистрация/авторизация:
	
	* Имя
	* Фамилия
	* E-mail
	* Логин
	* Пароль
	* Кнопка зарегистрироваться/авторизироваться

	5.2. Главная страница:
	
	* Навигация слева(Главная, Заказ окна, Просмотр материалов, Редактирование базы данных)
	* Галерея
	* Новые материалы
	* Информация о компании

	5.3. Заказ окна:
	
	* Выбор материалов 
	* Корзина
	* Чек
	* Ввод размеров окна

	5.4. Просмотр материалов
	
	* Список материалов
	* Поиск по материалам
	* Сортировка
	* Группировка **ASC/DESC**

	5.5.  Редактирование базы данных
	
	* Строка запроса **SQL**
	* Удаление строки
	* Добавление строки
	
	5.6.  Справка
	
	* Переход на сайт поддержки

6. ### <a name="item6"></a> Порядок контроля и приемки системы

	Тестирование функционала, проверка документации, проверка кода на соответствие требованиям проводится согласно графику:
	
	*   полное тестирование с **24.03.2019** по **31.03.2019**
	*   проверка кода на соответствие требованиям с **26.03.2019** по **31.03.2019**
	*   проверка/согласование документации с **29.03.2019** по **31.03.2019**
		
7. ### <a name="item7"></a> Требования к вводу системы в эксплуатации

	Использование **sql Server** для **windows 7** и выше. Создание **.exe** приложения.
