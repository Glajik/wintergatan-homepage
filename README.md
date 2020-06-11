# The Wintergatan Homepage

This is not official website, it's only a hypotetic new website wireframe, created for learning purposes.

[Official Website](https://wintergatan.net/)

Wintergatan (Swedish pronunciation: [ˈvɪ̂nːtɛrˌɡɑːtan], "the Milky Way", lit. '"the Winter Street"') is a Swedish folktronica band from Gothenburg. Martin Molin and Marcus Sjöberg were previously part of the former band Detektivbyrån. The band uses a variety of unconventional instruments including the Modulin, a fingerboard-controlled synthesizer built from Doepfer eurorack modules,[3] the Moog Theremini digital theremin, an electric autoharp, a hammered dulcimer, a self-built punch-card music box, a slide projector, a musical saw, and a typewriter for use as percussion.

## Marble Machine
Between December 2014 and March 2016, the band uploaded several YouTube videos featuring Martin Molin documenting the construction of a music box that uses marbles to play instruments. The machine is powered by a hand-crank, and works by raising steel marbles through the machine into multiple feeder tubes, where they are then released from height via programmable release gates, falling and striking a musical instrument below. Instruments played by marbles striking them include a vibraphone, bass guitar, cymbal, and emulated kick drum, high hat and snare drum sounds using contact microphones. The music score is stored on two programmable wheels that utilize Lego Technic beams and stud connectors to trigger armatures to release the marbles. A final music video showing the machine in use was released in 2016, and has been viewed over 141 million times.

[Wikipedia](https://en.wikipedia.org/wiki/Wintergatan)

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