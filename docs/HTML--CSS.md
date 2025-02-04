[:arrow_left: Back](https://github.com/Awake-coding/cheat-sheets)

# HTML/CSS шпаргалка

1. [Селекторы +, >, ~](#селекторы)
1. [Селекторы атрибутов CSS: a[target]{}...](#селекторы-атрибутов-css-atarget-typecheckbox)



## Селекторы `+`, `>`, `~`
  - `A + B`
      - Применить стиль к элементу `B`, который находиться сразу после `A`
          - простыми словами: `+` - наследование соседних тегов
          - Пример (код 👇):
              - отработает `display: none` только для первого блока с классом `.myToggle`, так как этот блок находиться сразу после `<input>`, а вот для второго блока с классом `.myToggle` уже не отработает `display: none`
              - и при этом для каждого блока с классом `.myToggle`, который сразу следует после других `<input>`, для них тоже отработает `display: none`

                ```scss
                  input
                    &:checked + .myToggle
                      display: none;
                    &:checked + .myMark
                      display: none;
                ```
                ```html
                    <input type="checkbox">
                    <div class="myToggle"></div>
                    <div class="myMark"></div>
                    <div class="myToggle"></div>

                ```
  - `A ~ B`
      - Применить стиль к элементам `B`, которые находятся после `A`
          - простыми словами: `~` - похоже на `+`, но не такой строгий
          - Пример (код 👇):
              - отработает `display: none` для всех блоков с классами `.myToggle` и `.myMark`, которые находятся на том же уровне что и `<input>` (под кнопкой)
              - а вот для блока с классом `.myToggle`, который между `<div class="myMark">`, уже не отработает `display: none`

                ```scss
                  input
                    &:checked ~ .myToggle
                      display: none;
                    &:checked ~ .myMark
                      display: none;
                ```
                ```html
                    <input type="checkbox">
                    <div class="myToggle"></div>
                    <div class="myMark">
                      <div class="myToggle"></div>
                    </div>
                    <div class="myToggle"></div>

                ```
  - `A > B`
      - Применить стиль к элементам `B`, которые являются дочерними по отношению к `A`
          - простыми словами: `>` - наследование внутренних тегов
          - Пример (код 👇):
              - будут выбраны только те `<h2>`, что прописаны сразу между `<section></section>`, а те `<h2>` что между другими блоками, не будут задействованы.
              - Таким образом текст в `<h2>`, что между `<div></div>`, не будет окрашен в красный цвет

                ```scss
                  section > h2
                      color: red;
                ```
                ```html
                  <section>
                      <h2>Заголовок 1</h2>
                      <div><h2>Заголовок 2</h2></div>
                      <h2>Заголовок 3</h2>
                  </section>
                ```

## Селекторы атрибутов CSS `a[target]{}`, `[type="checkbox"]{}`
  - Можно вот так обращаться к стилям блока:
      - `a[target]{}`
      - `[type="checkbox"]{}`







  <br><br>
[👆 Upward](#htmlcss-шпаргалка)