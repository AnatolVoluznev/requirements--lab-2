# Требования к проекту

## 1. Введение
Создаваемый проект – мобильное приложение под Android, позволяющее определять цвет, используя камеру телефона. Название – ColorPicker.  Также приложение позволяет просмотреть всю палитру цветов и их названия, используя rgb значения.

## 2. Требования пользователя
  * Программные интерфейсы
  Приложение требует разрешение на доступ к камере телефона. Не использует дополнительных библиотек или сервисов, все данные о цветах хранятся в самом приложении в виде текстового файла.
  * Интерфейс пользователя
  Приложение использует максимально упрощенный, интуитивно понятный интерфейс. Поскольку оно выполняет только одну функцию, нет смысла делать главное меню, усложняя тем самым алгоритм работы и увеличивая количество действий пользователя. При запуске приложения автоматически открывается камера, и, по нажатию в любую область экрана, показывается окно с информацией о выбранном цвете.
  
  ![View from camera](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/screens/CameraScreenView.jpg)
   ![View from camera](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/screens/ResultScreenView.jpg)
   
   * Характеристики пользователей
   Приложение ориентировано на самых неопытных и неподкованных в техническом плане пользователей. Чтобы приложение выполнило свою основную функцию, пользователю требуется всего лишь запустить приложение, навести телефон на интересующий его предмет и нажать пальцем в любую область экрана. Никаких кнопок, функций или входных данных, сбивающих с толку начинающих, неопытных пользователей, людей пожилого возраста. 	Также приложение идеально подойдет молодым людям, чтобы демонстрировать свой вкус, разборчивость и внимательность, когда в разговоре с девушкой приходится определять цвет ее новой сумочки.
   
   * Предположения и зависимости
   Приложение абсолютно нетребовательно к системным ресурсам, за исключением камеры. Качество и цветопередача камеры напрямую определяет точность определения цвета. Также на моделях мобильных телефонов со слабым процессором возможны зависания при быстрой прокрутке ползунков определения rgb цвета.
   
## 3. Системные требования
 Приложение разрабатывается под платформу android 6-й версии.
 
   * Функциональные требования
      * Окно камеры:
          1.	Использование камеры смартфона напрямую, не используя стандартное приложение.
          2.	 При нажатии на экран не сохранять снимок, обрабатывать только выбранную область.

       * Окно палитры:
          1.	Использование ползунков вместо полей для ввода значений для упрощения взаимодействия с функционалом приложения.
          2.	Кнопка «Камера», возвращающая пользователя обратно к определению цвета. 
       * Определение цвета:
          1.	Определять усредненный цвет области, в которую было совершенно нажатие.
          2.	Фильтр шумов, удаление из выборки пикселей с шумовыми и неопределенными цветами.
        
   * Нефункциональные требования:
        * АТРИБУТЫ КАЧЕСТВА
Главным атрибутом качества является точность определения цвета. При недостаточном освещении в область определения цвета попадают шумы, которые могут помешать корректной работе приложения.


# Диаграммы
* Классов:
 ![classes](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/schemas/classes.png)

* Состояний
![Sequences](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/schemas/sequence%20diagramm.png)

* Использования
![Sequences](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/schemas/useCase.png)

* Компонентов
![Sequences](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/schemas/components.png)

* Деятельности
![Sequences](https://github.com/AnatolPiskarev/requirements--lab-2/blob/master/schemas/activity.png)

     
