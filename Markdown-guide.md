[:arrow_left: Back](https://github.com/Awake-coding/cheat-sheets)

# Markdown синтаксис

1. <details><summary>👈 Заголовок <code>#(1-6)</code></summary><p>

      - # h1 `#`
      - ## h2 `##`
      - ### h3 - h6
    </p><hr></details>

2. <details><summary>👈 Стилизация текста <code>*</code>, <code>_</code>, <code>~</code></summary><p>

      | Синтаксис | Результат                       |
      | ---       | ---                             |
      | `** **`   | **Жирный** vs Обычный           |
      | `* *`     | *Курсив* vs Обычный             |
      | `**_ _**` | **Жирный и _вложенный курсив_** |
      | `*** ***` | ***Все жирным и курсивом***     |
      | `~~ ~~`   | ~~Зачеркнутый~~                 |
    </p><hr></details>

3. <details><summary>👈 Цитирование текста <code>></code></summary><p>

      - `<blockquote> </blockquote>`
      - ![quote](img/quote.jpg)

      - >    Цитата
        >>   Цитата
        >>>  Цитата
        >>>> Цитата
    </p><hr></details>

4. <details><summary>👈 Код <code>` `</code> (однострочный)</summary><p>

      - <code>\` \`</code>
      - `<code> </code>`
    </p><hr></details>

5. <details><summary>👈 Код <code>``` ```</code> (многострочный)</summary><p>

    - ` ``` ``` `
    - `<pre><code> </code></pre>`

    - Не указан язык
      ```
      document.querySelector('div');
      ```
    - Указан язык JS
      ```JS
      document.querySelector('div');
      ```
      <pre>
      ```JS
        document.querySelector('div');
      ```
      </pre>
    </p><hr></details>

6. <details><summary>👈 Ссылки <code>[](Link)</code></summary><p>

    - `[title](Link)`
    - `<a href=""> </a>`
    - Ссылка на репозиторий ['cheat-sheets'](https://github.com/Awake-coding/cheat-sheets)
      - `['cheat-sheets'](https://github.com/Awake-coding/cheat-sheets)`
    - Ссылки на разделы
      - <img width="220px" alt="link__h1-h6" title="" src="img/link__h1-h6.jpg">
    - Относительные ссылки
      - `[LICENSE watch file](LICENSE.md)`
    </p><hr></details>

7. <details><summary>👈 Картинки <code>![](Link)</code></summary><p>

    - <img width="70px" alt="Octocat" title="Octocat" src="https://myoctocat.com/assets/images/base-octocat.svg">

      ```html
        <img width="px" alt="" title="" src="">
      ```
    - ```markdown
      ![Octocat](https://myoctocat.com/assets/images/base-octocat.svg)
      ```
    - Совет: Если вы хотите отобразить изображение, которое находится в вашем репозитории, вы должны использовать относительные ссылки `/assets/images/electrocat.png`
    - Темы, в которой показано изображение:
        - Тему можно задать, в которой будет показано изображение, добавив `#gh-dark-mode-only` или `#gh-light-mode-only` в конец URL-адреса изображения в Markdown.
          - Темная тема
          ```markdown
          ![Title-for-Dark](https://github.com/github-light.png#gh-dark-mode-only)
          ```
          - Светлая тема
          ```markdown
          ![Title-for-Light](https://github.com/github-dark.png#gh-light-mode-only)
          ```
    </p><hr></details>

8. <details><summary>👈 Списки <code>-</code>, <code>*</code>, <code>1.-999.</code></summary><p>

    - `- Text` Неупорядоченный список
        - в начале строки поставить `-` или `*`
          - Иногда делать 1 пустую строку перед списком, что бы он заработал
    - `1. Text` Упорядоченный список
        - в начале строки поставить любое число
          - Иногда делать 1 пустую строку перед списком, что бы он заработал
    - Вложенные списки
        ```
        - Пункт списка
            - Пункт вложенного списка
        👆👆 2 таба для вложенного списка
        ```
    1. 1.1 ————— `1. 1.1`
        1. 1.2 ——— `1. 1.2`
            1. 1.3 — `1. 1.3`
            1. 2.3 — `1. 2.3`
        1. 2.2 ——— `1. 2.2`
    </p><hr></details>

9. <details><summary>👈 Списки задач <code>- [ ]</code>, <code>- [x]</code></summary><p>

    - [x] — `- [x]` выполнено
    - [ ] — `- [ ]` задача
    - Если начало текста такого списка `(`, то писать так `- [ ] \() Text`
    </p><hr></details>

10. <details><summary>👈 Эмодзи (emoji) ✌️</summary><p>

    - Всё эмодзи тут [`Emoji - шпаргалка`](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
      - [Эмоции](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#emotion) :speech_balloon: :left_speech_bubble: :blue_heart: :yellow_heart: и тд
      - [Жесты рук, тела](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#hand-fingers-open) :point_right: :point_left: :point_up_2: :point_down: :wave: :vulcan_salute: :ok_hand: :v: :+1: :-1: :muscle: :eye:
      - [Еда](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#food-fruit) :banana: :peach: :carrot:
      - [Глобус, карта, здания](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#place-map) :earth_africa: :globe_with_meridians: :world_map:
      - [Время](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#time) :hourglass: :alarm_clock:
      - [Погода](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#time) :fire: :star: :zap: :high_brightness: :sun_with_face:
      - [Деятельность](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#activities) :dart: :diamonds: :balloon: :trophy: :video_game: :ribbon:
      - [Объекты](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#objects) :phone: :telephone_receiver: :gem: :desktop_computer: :loud_sound: :floppy_disk: :movie_camera: :camera: :mortar_board: :musical_note: :mag: :mag_right: :cd: :dvd: :crown: :bell:
      - [Книга, деньги, почта, писать](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#book-paper) :memo: :page_facing_up: :receipt: :green_book: :label: :chart: :moneybag: :envelope: :pencil2:
      - [Офис](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#office) :open_file_folder: :clipboard: :pushpin: :calendar: :chart_with_upwards_trend: :scissors: :wastebasket:
      - [Замки](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#lock) :lock:
      - [Инструмент...](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#tool) :hammer: :wrench: :hammer_and_wrench: :gear: :link: :drop_of_blood: :shopping_cart:
      - [Символы](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#symbols) :warning: :exclamation: :o: :no_entry: :x: :heavy_check_mark: :white_check_mark: :arrow_right: :arrow_left: :arrow_up: :arrow_down: :arrow_heading_down: :arrow_forward: :arrow_backward: :one: :two: :information_source: :high_brightness: :heavy_plus_sign: :heavy_minus_sign: :fleur_de_lis:
      - [Геометрические](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#geometric) :radio_button: :green_circle: :red_circle: :orange_circle: :yellow_circle: :black_circle: :large_orange_diamond: :small_orange_diamond: :triangular_flag_on_post:
    </p><hr></details>

11. Переносы `<br>` or `пустая строка`

12. <details><summary>👈 Сноски <code>[^1]</code>, <code>[^1]:</code></summary><p>

    - Простая сноска[^1].
    [^1]: Справка, перевод, толкование, помещаемые в нижней части README

    - Сноска может состоять из нескольких строк[^2].
      [^2]: Эта строка должна заканчиваться 2мя пробелами, а каждая новая строка должна начинаться с двух пробелов.
        Это позволяет вам иметь сноску с несколькими строками.

    - Можно использовать слова в названии сноски, чтобы лучше соответствовать контексту[^note].
    [^note]:
        Именованные сноски по-прежнему будут отображаться с номерами вместо текста, но упрощают идентификацию и связывание.

    - ```
      - Простая сноска[^1].
      [^1]: Справка, перевод, толкование, помещаемые в нижней части README

      - Сноска может состоять из нескольких строк[^2].
      [^2]: Эта строка должна заканчиваться 2мя пробелами, а каждая новая строка должна начинаться с двух пробелов.
        Это позволяет вам иметь сноску с несколькими строками.

      - Можно использовать слова в названии сноски, чтобы лучше соответствовать контексту[^note].
      [^note]:
          Именованные сноски по-прежнему будут отображаться с номерами вместо текста, но упрощают идентификацию и связывание.
      ```

    - ❗ `[^1]:` Текст сноски можно располагать где угодно внизу, после предложения со сноской `[^1]`
    </p><hr></details>

13. Комментарий (скрытый текст) `<!-- -->`

14. <details><summary>👈 Символ игнор/экранирование в Markdown <code>\</code></summary><p>

    - Пример:
        - k и *k* `k и *k*`
        - k и \*k\* `k и \*k\*`
    </p><hr></details>





15. <details><summary>👈 Таблицы <code>|</code> + <code>-</code></summary><p>

    - | Header        | Header        |
      | ---           | ---           |
      | Content Cell  | Content Cell  |
      | Content Cell  | Content Cell  |
    - <table>
        <thead align="center">
          <tr> <th>Header</th> <th>Header</th> </tr>
        </thead>
        <tbody>
          <tr> <td>Content Cell</td> <td>Content Cell</td> </tr>
          <tr> <td>Content Cell</td> <td>Content Cell</td> </tr>
        </tbody>
      </table>
    -
    -
    -
    </p><hr></details>










<br><br>


##### За основу взяты источники:
  - #### Для 1-14
      - [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
      - [Basic Syntax](https://www.markdownguide.org/basic-syntax/)
      - [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)
  - #### Для 15-
      - [Advanced formatting](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting)

[:arrow_left: Back](https://github.com/Awake-coding/cheat-sheets)