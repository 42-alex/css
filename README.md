# CSS Notes

## Sources for learning

* https://ru.code-basics.com/languages/css/ (practical tasks)

---

## CSS Properties

### font-family

Позволяет выбрать один или несколько шрифтов, которые будут использоваться в документе.
Наиболее распространёнными шрифтами являются:
* Times New Roman
* Arial
* Tahoma
* Verdana
* Courier New

С большей долей вероятности эти шрифты будут установлены и в системе у другого пользователя. Если шрифтов, указанных в свойстве font-family, на компьютере нет, то будет использован шрифт по умолчанию, заданный в настройках браузера.

При подключении стилей хорошей практикой является добавление универсального семейства шрифта в правило font-family (в конец, в последнюю позицию). Таких семейств на данный момент 5:

* **serif** — шрифты с засечками (антиквы). Ярким представителем таких шрифтов является Times New Roman.
* **sans-serif** — шрифты без засечек (гротеск). Наиболее знакомыми такими шрифтами являются Arial и Verdana.
* **cursive** — курсивные шрифты.
* **fantasy** — декоративные шрифты. Это семейство используется реже всего. Дело в том, что декоративные шрифты слишком разные, чтобы они были взаимозаменяемые.
* **monospace** — моноширинные шрифты. К ним относятся шрифты, в которых все символы имеют одинаковую ширину. Очень часто их используют программисты в текстовых редакторах.
Добавив универсальное семейство шрифта в правило font-family, мы страхуем себя от того, что у пользователя не окажется такого шрифта, который мы указали. Тогда браузер автоматически выберет ему замену из того универсального семейства шрифтов, которое мы указали.
  
```
.new-font {
    font-family: Arial, Futura, sans-serif;
}
```
Теперь, если у пользователя в системе нет шрифтов Arial или Futura, будет выбран системный шрифт без засечек (из семейства sans-serif).

---