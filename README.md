Для работы вы должны установить Stylus в свой проект

Например

```
$ npm install --save-dev gulp-stylus
```

И подключить его следуя инструкциям к `gulp-stylus`

Дальше Вы устанавливаете atomic-reset:

```fish
$ npm install atomic-reset --save-dev
```

В любом .styl файле своего проекта вы можете подключить atomic-reset и миксины будут работать:

```stylus
@import './node_modules/atomic-reset'
```

## Миксины

### r-offset()

Сбрасывает наружние и внешние отступы

Параметры: -

```stylus
p
  r-offset()
```

```css
p {
  margin: 0;
  padding: 0;
}
```

### r-clearfix()

Сбрасывает псевдоэлементы `before` и `after`

Параметры: -

```stylus
p
  r-clearfix()
```

```css
p:before,
p:after {
  content: '';
  content: none;
  display: none;
}
```

### r-bs()

Сбрасывает стиль `box-sizing`

Параметры:

- <b>@param $r-bs</b>:
  - <b>border-box</b>: В размеры блока входят padding и border
  - content-box: В размеры блока не входят margin, padding и border
  - padding-box: В размеры блока входит только padding
  - inherit: Наследует значение родителя

``` stylus
div
  r-bs()
```

``` css
div {
  box-sizing: border-box;
}
```

### r-outline()

Сбрасывает стиль `outline`

Параметры: -

``` stylus
button
  r-outline()
```

``` css
button {
  outline: none;
}
```

### r-b()

Параметры:

- <b>@param $r-bs</b>:
  - <b>border-box</b>: В размеры блока входят padding и border
  - content-box: В размеры блока не входят margin, padding и border
  - padding-box: В размеры блока входит только padding
  - inherit: Наследует значение родителя.

``` stylus
span
  r-b()
```

``` css
span {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  display: block;
}
```

... to be continued ...

### r-i()

### r-ib()

### r-f()

### r-button

### r-input

### r-list

### r-link

### r-select

### r-table