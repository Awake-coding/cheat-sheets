# Markdown синтаксис

1. <details><summary>👈 Заголовок <code>#(1-6)</code></summary><p>

      - # h1 `#`
      - ## h2 `##`
      - ### h3 - h6
    </p><hr></details>

2. <details><summary>👈 Стилизация текста <code>*</code>,<code>_</code>,<code>~</code></summary><p>

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

    - ```markdown
      ![Octocat](https://myoctocat.com/assets/images/base-octocat.svg)
      ```
    - <img width="70px" alt="Octocat" title="Octocat" src="https://myoctocat.com/assets/images/base-octocat.svg">

      ```html
        <img width="70px" alt="" title="" src="">
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

8. <details><summary>👈 Списки</summary><p>

  -
  -
  -
  -
  -
  </p><hr></details>





