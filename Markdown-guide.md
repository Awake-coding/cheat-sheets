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

10. <details><summary>👈 Эмодзи</summary><p>

  - Всё эмодзи тут [Emoji - шпаргалка](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
    - [Эмоции](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#emotion) :blue_heart: :yellow_heart: :speech_balloon: :left_speech_bubble: и тд
    - [Жесты рук, тела](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#hand-fingers-open) :wave: :vulcan_salute: :ok_hand: :v: :point_right: :point_left: :point_up_2: :point_down: :+1: :-1: :muscle: :eye:
    - [Еда](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#food-fruit) :banana: :peach: :carrot:
    - [Глобус, карта, здания](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#place-map) :earth_africa: :globe_with_meridians: :world_map:
    - [Время](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#time) :hourglass: :alarm_clock:
    - [Погода](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#time) :fire: :star: :zap: :sun_with_face:
    - [Деятельность](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#activities) :balloon: :ribbon: :trophy: :dart: :video_game: :diamonds:
    - [Объекты](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#objects) :gem: :crown: :mortar_board: :loud_sound: :bell: :musical_note: :phone: :telephone_receiver: :desktop_computer: :floppy_disk: :cd: :dvd: :movie_camera: :camera: :mag: :mag_right:
    - [Книга, деньги, почта, писать](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#book-paper) :memo: :page_facing_up: :receipt: :green_book: :label: :chart: :moneybag: :envelope: :pencil2:
    - [Офис](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#office) :open_file_folder: :clipboard: :pushpin: :calendar: :chart_with_upwards_trend: :scissors: :wastebasket:
    - [Замки](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#lock) :lock:
    -
    -
    -
    -
  </p><hr></details>

