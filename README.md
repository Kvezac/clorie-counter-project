This is a project after completing the Java script course. Below is a description and requirements for the project.
- To run the project locally, click the "fork" button
- Run a git clone on your workstation
- npm install
- npm run start
- Open browser fill in form fields
<h2>Lighthouse</h2>
<p align="center">
  ![Image alt](https://github.com/{Kvezac}/{calorie-counter-project}/raw/{main}/{https://github.com/Kvezac/calorie-counter-project/blob/main/src/style/img/lighthouse.png}/lighthouse.png)
</p>

<h2>Техническое задание проекта</h2>
<p>Пример ниже описывает один из способов выполнения проекта.</p>

<h3>Для работы вам понадобятся два класса:</h3>
<ul>
  <li>Counter содержит внутри себя основные  методы расчета, получение данных пользователя, добавление/удаление прослушивателей событий.</li>
  <li>Result необходим только для показа/скрытия результатов расчета пользователю. В нем всего два метода: show и hidden.</li>
</ul>
<h3>Состояние по умолчанию</h3>
<ul>
  <li>Выбран мужской пол.</li>
  <li>В полях ввода стоит 0.</li>
  <li>Выбрана «минимальная»</li> физическая активность.
  <li>Кнопка «Рассчитать» неактивна.</li>
  <li>Кнопка сброса данных из полей ввода неактивна.</li>
  <li>Блок с выводом информации</li> о калориях скрыт.</li>
<li>Кнопка «Рассчитать». Становится активна только когда заполнены все поля ввода.</li>
<li>По клику на кнопку появляется блок с информацией о калориях, если до этого он не был показан. Если блок уже находится на странице, клик по кнопке обновляет расчеты, выводится актуальная информация.</li>
<li>Кнопка «Очистить поля и расчёт». Становится активна, когда произошли изминения в форме.</li>
<li>При клике все элементы приложения сбрасываются до состояния по умолчанию: числовые поля очищаются (плейсхолдер 0), пол становится мужской, физическая активность «минимальная», блок с информацией о калориях скрывается.</li>
</ul>
<h2>Формулы:</h2>
Поддержание веса
<h3>Для женщин:</h3>
<ul>
  <li>N = (10 × вес в килограммах) + (6,25 × рост в сантиметрах) − (5 × возраст в годах) − 161</li>
</ul>
<h3>Для мужчин:</h3>
<ul>
  <li>N = (10 × вес в килограммах) + (6,25 × рост в сантиметрах) − (5 × возраст в годах) + 5</li>
</ul>
- Полученное значение (N) умножаем на коэффициент активности. Результат и будет нормой калорий для поддержания веса.
<h3>Коэффициенты активности</h3>
<ul>
  <li>Минимальная: 1.2.</li>
  <li>Низкая: 1.375.</li>
  <li>Средняя: 1.55.</li>
  <li>Высокая: 1.725.</li>
  <li>Очень высокая: 1.9.</li>
</ul>
<h3>Формулы для набора и сброса веса</h3>
<ul>
  <li>Набор веса: прибавляем 15% от нормы к этой норме.</li>
  <li>Сброс веса: вычитаем 15% от нормы из этой нормы.</li>
</ul>
