# The Wintergatan Homepage

## Интересности

### Схлопывание отступов (margin)

[htmlbook](http://htmlbook.ru/samlayout/blochnaya-verstka/skhlopyvayushchiesya-otstupy)

### Управление проигрывателем Youtube, встроенным через IFrame

[IFrame player API](https://developers.google.com/youtube/iframe_api_reference)
[API Demo and IFrame constuctor](https://developers.google.com/youtube/youtube_player_demo)

### Позиционирование: relative - absolute

```HTML
<div class="parent">
  <button class="child">
  </button>
</div>

<style>
  .parent {
    position: relative;
  }

  .child {
    position: absolute;
    bottom: 0px;
  }
</style>
```

### CSS variables

[Using CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)

### Три элемента в строке

[stackoverflow](https://stackoverflow.com/questions/48464444/how-to-display-3-items-per-row-in-flexbox/48464559)

### Работа с формой

```JS
// Предотвращение отправки
const formEl = document.getElementById('form');
formEl.addEventListener('submit', (event) => {
  event.preventDefault();
  console.log(event);
});

// Можно вручную опросить элементы
let email = document.querySelector('[name="inputEmail"]').value
let name = document.querySelector('[name="firstname"]').value
let data = `FirstName: ${name}, Email: ${email}`

// А можно использовать FormData object
const data = new FormData(formEl);
console.log(data);
```

[Submit event](https://developer.mozilla.org/en-US/docs/Web/API/HTMLFormElement/submit_event)
[Using FormData Objects](https://developer.mozilla.org/en-US/docs/Web/API/FormData/Using_FormData_Objects)


### Навигация

```JS
// Navigate to a new page
location.assign("http://www.mozilla.org");

// Force reloading the current page from the server
location.reload(true);
```

[Location](https://developer.mozilla.org/en-US/docs/Web/API/Window/location)
[History](https://developer.mozilla.org/en-US/docs/Web/API/History/pushState)