[:arrow_left: Back](https://github.com/Awake-coding/cheat-sheets)


# Примеры "BEM":

- ### Выпадающее меню ```nav>ul>li>a+(ul>li>a)```
  ```HTML
  <nav class="menu">
     <ul class="menu__list">
       <li class="menu__item active">
         <a class="menu__link" href="#">
            Обувь
         </a>
         <ul class="submenu__list">
            <li class="submenu__item">
               <a class="submenu__link" href="#">
                  Босоножки
               </a>
            </li>
         </ul>
       </li>
     </ul>
  </nav>
  ```
- ### Сообщение успех/ошибка
  ```HTML
  <div class="message message--success">
     <h3 class="message__title">Заголовок сообщения</h3>
     <div class="message__text">Текст сообщения</div>
  </div>

  <div class="message message--error">
     <h3 class="message__title">Заголовок сообщения</h3>
     <div class="message__text">Текст сообщения</div>
  </div>
  ```

  Обоим элементам можно добавить одинаковые стили используя общий класс .message и так же легко можно добавить отдельные стили для каждого из них, используя уникальный класс с модификатором.

  ```CSS
  .message {
    border: 1px solid gray;
  }
    .message--success {
      border-color: green;
    }
    .message--error {
      border-color: red;
    }
  ```
- ### Галерея
  ```HTML
  <div class="gallery">
    <ul class="gallery__list">
      <li class="gallery__item">
        <img class="gallery__img" src="flowers.jpg" alt="Цветы">
      </li>
      <li class="gallery__item">
        <img class="gallery__img" src="trees.jpg" alt="Деревья">
      </li>
    </ul>
  </div>
  ```
- ### Картинка пользователя
  ```HTML
  <div class="user">
    <img class="user__img" src="userpic.png" alt="Дормидонт Петрович">
    <a class="user__link" href="#">Дормидонт Петрович</a>
  </div>
  ```
- ### Виджет в боковой колонке
  ```HTML
  <div class="widget">
    <h4 class="widget__title">Выращиваем желе</h4>

    <div class="widget__content">
      <p>Чтобы вырастить общительное дружелюбное желе,
      нам потребуется рулон поролона, два килограмма сахара,
      три яйца и пол чайной чашки ацетона.</p>

      <a class="widget__link" href="#">Не читать дальше...</a>
    </div>
  </div>
  ```
- ### Блок новостей
  ```HTML
  <div class="news">
    <h3 class="news__title">Вчерашние новости</h3>

    <ul class="news__list">
      <!-- к классу элемента добавляем класс блока,
            чтобы создать новое пространство имён -->
      <li class="news__item item-news">
        <h4 class="item-news__title">Соревнования среди воблы по конькобежному спорту</h4>
        <div class="item-news__text">
          <p>Победила команда килек из Петрозаводска</p>

          <a href="#" class="item-news__link">Читать дальше</a>
        </div>
      </li>

      <li class="news__item item-news">
        <h4 class="item-news__title">Учёные уточнили роль напильника в уходе за ногтями</h4>
        <div class="item-news__text">
          <p>Британские учёные высоко оценили вклад
            напильника в отращивание полутораметровых ногтей.</p>

          <a href="#" class="item-news__link">Не читать дальше</a>
        </div>
      </li>
    </ul>
  </div>
  ```
- ### Статья или пост в блоге (простой вариант)
  ```HTML
  <article class="article">
    <h3 class="article__title">Нащупываем чакры у пучка петрушки</h3>
    <time class="article__datetime">32 мая, 10:87</time>

    <div class="article__author author-article">
      <img class="author-article__img" src="userpic.png" alt="Клешня Андреевна">
      <a class="author-article__link" href="#">Клешня Андреевна Долгорукая</a>
      <div class="author-article__desc">Наш эксперт по чакрам</div>
    </div>

    <div class="article__content">
      Сходите на рынок и купите у старушек пучок петрушки грамм на 100.
      Как следует переберите, очистите от жуков и гусениц. Жуков отдайте поиграться
      коту, гусениц поселите в горшок с кактусами, пусть одна будет Джоном,
      вторая Билли, а у вас в горшке теперь будет Дикий Запад. Вернитесь
      к пучку петрушки. Ласково взгляните на него и как следует почешите
      за ухом, можно себе или коту. Перевяжите атласной ленточкой,
      непременно завяжите бант. Поздравляем! Теперь у вас есть полностью
      одомашненный пучок петрушки, который будет весело бегать за вами
      по пятам и проращивать свои семена в ваших тапках.
    </div>
  </article>
  ```
- ### Статья или пост в блоге (сложный вариант)
  ```HTML
  <article class="entry">
    <header class="entry__header">
      <h3 class="entry__title title-entry">
        <a class="title-entry__link" href="#">Резиновые уточки как способ самопознания</a>
      </h3>

      <time class="entry__datetime">32 мая, 10:87</time>
    </header>

    <div class="entry__author author-entry">
      <img class="author-entry__img" src="userpic.png" alt="Василиса Сергеевич">

      <a class="author-entry__link" href="#">Василиса Сергеевич</a>
    </div>

    <div class="entry__content">
      Достаньте с чердака коробку с полусотней резиновых уточек,
      оставшихся после празднования нового года. Из уточек
      и горящих свечей выложите пентаграмму на полу комнаты.
      Сядьте посередине в позу лотоса, в каждую руку возьмите
      по немецко-бразильскому словарю, прокашляйтесь, наберите
      полную грудь воздуха и громко и уверенно,
      с полной самоотдачей скажите "Кря!"
    </div>

    <div class="entry__tags tags-entry">
      <h4 class="tags-entry__title">Метки</h4>

      <ul class="tags-entry__list">
        <li class="tags-entry__item">
          <a class="tags-entry__link" href="#">хоровод своими руками</a>
        </li>
        <li class="tags-entry__item">
          <a class="tags-entry__link" href="#">фарфоровые тапки</a>
        </li>
        <li class="tags-entry__item">
          <a class="tags-entry__link" href="#">гуталин в кулинарии</a>
        </li>
      </ul>
    </div>

    <div class="entry__actions actions-entry">
      <ul class="actions-entry__list">
        <li class="actions-entry__item actions-entry__item--read">
          <a class="actions-entry__link" href="#">238 ответов</a>
        </li>
        <li class="actions-entry__item actions-entry__item--write">
          <a class="actions-entry__link" href="#">Написать в спортлото</a>
        </li>
        <li class="actions-entry__item actions-entry__item--share">
          <a class="actions-entry__link" href="#">Поделиться</a>
        </li>
      </ul>
    </div>
  </article>
  ```


<br><br>


За основу взяты источники:
  - [Слова, часто используемые в CSS-классах](https://github.com/yoksel/common-words)
  - [Как писать классы по БЭМ?](http://yoksel.github.io/easy-markup/bem-rules/)
  - [Методология HTML по БЭМ](https://ru.bem.info/methodology/html/)


[:arrow_left: Back](https://github.com/Awake-coding/cheat-sheets)