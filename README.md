<img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="qamarq" src="https://i.imgur.com/IRySH8e.png">  


## 🍫 CSS Components kit inspired by Windows 11 UI - Kamil Marczak (aka qamarq) 🍫
**[PL]**
Jeżeli chcesz zrobić stronę w stylu najnowszego Windowsa 11, możesz wykorzystać mój CSS z gotowymi komponentami, takimi jak przyciski, pola tekstowe czy pola wyboru.

**[EN]**
If you want to make a website in the style of the latest Windows 11, you can use my CSS with ready-made components such as buttons, text-boxes and check-boxes.



---
## 🛫 Get started
**[PL]**
1. Pobierz plik `w11-components.css` z folderu `src` i umieść go w swoim projekcie
2. W swoim pliku `.html` dodaj w sekcji `<head>` następujące odwołanie: `<link rel="stylesheet" href="./w11-components.css"></link>`
3. Gotowe

**[EN]**
1. Download the `w11-components.css` file from the `src` folder and place it in your project
2. In your `.html` file, add the following reference in the `<head>` section: `<link rel="stylesheet" href ="./w11-components.css"></link>`
3. Done



---
## 🌍 Example page
**[PL]**
W repozytorium znajduje się folder `example-page`. W środku możesz znaleźć przykładową stronę prezentującą komponenty.

**[EN]**
There is an `example-page` folder in the repository. Inside, you can find an example page showing components.

<div>
    <img alt="qamarq" src="https://i.imgur.com/H6Fn6gd.png"> 
    <img alt="qamarq" src="https://i.imgur.com/zRvb8Ok.png"> 
</div>



---
## 🚀 Use  

- Buttons | primary & seconadry
```html
<div class="btn primary">
    <p>Text</p>
</div>
```
```html
<div class="btn secondary">
    <p>Text</p>
</div>
```
- Input text
```html
<div class="textbox">
    <input class="textbox-input" type="text">
    <!-- This span is optional (icon): -->
    <span class="material-icons-outlined textbox-icon">visibility</span> 
</div>
```
- Text area
```html
<textarea name="myInput" cols="45" rows="7" minlength="1" maxlength="500" required></textarea>
```
- Switch (default unchecked)
```html
<!-- Default checked: -->
<label class="switch">
    <input type="checkbox" checked>
    <span class="switch-inside"></span>
</label>                  

<!-- Default unchecked: -->
<label class="switch">
    <input type="checkbox">
    <span class="switch-inside"></span>
</label>
```
- Checkbox 
```html
<!-- Default checked: -->
<label class="check-box">Text
    <input type="checkbox" checked="checked">
    <span class="checkmark-checkbox"></span>
</label>

<!-- Default unchecked: -->
<label class="check-box">Text
    <input type="checkbox">
    <span class="checkmark-checkbox"></span>
</label>
```
- Radio-button 
```html
<!-- Default checked: -->
<label class="radio-button">Text
    <input type="radio" checked="checked" name="radio">
    <span class="checkmark-radiobutton"></span>
</label>

<!-- Default unchecked: -->
<label class="radio-button">Text
    <input type="radio" name="radio">
    <span class="checkmark-radiobutton"></span>
</label>
```
- Banner
```html
<div class="banner">
    <span class="material-icons primary-icon">info</span>            
    <h1>Title</h1>
    <h2>Lorem ipsum dolor sit amet</h2>
    <div class="btn secondary">
        <p>Text</p>
    </div>
    <span class="material-icons secondary-icon">clear</span>
</div>
```
- Dialog
```html
<div class="dialog">
    <p class="dialog-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit, sed do eiusmod tempor.</p>
    <div class="dialog--buttons">
        <div class="btn primary">
            <p>Text</p>
        </div>
        <div class="btn secondary">
            <p>Text</p>
        </div>
    </div>
</div>
```

Slider: 
- HTML:
```html
<!-- Value 35 is 35% width on slider default thumb position -->
<input type="range" class="slider" min="1" max="100" value="35">
```
- JS
```js
//Change left and right color slider in real time

var sliders_list = document.getElementsByClassName("slider");
for (i = 0; i < sliders_list.length; i++) {
    sliders_list[i].oninput = function() {
        var value = (this.value-this.min)/(this.max-this.min)*100
        this.style.background = 'linear-gradient(to right, var(--slider-bg-left) 0%, var(--slider-bg-left) ' + value + '%, var(--slider-bg-right) ' + value + '%, var(--slider-bg-right) 100%)'
    };
}
```


---
## 🚶‍♂️ Author

qamarq#5665
[![Paypal Doante](https://img.shields.io/badge/paypal-donate-blue.svg)](https://paypal.me/KMarczak123)
[![Discord](https://discordapp.com/api/guilds/772941356423315527/embed.png)](https://discord.gg/buSQU2Bjxc)


---
## 🔨 LICENSE
**[PL]**
1. Arkusz CSS możesz edytować do woli i udostępniać swoje wersje. 
2. Jeżeli chcesz wykorzystać ten arkusz CSS na swojej stronie, musisz podać w komentarzu lub stopce link tego repozytorium (https://github.com/QamarQ/w11-css-components-kit/)

**[EN]**
1. You can edit the CSS at will and share your versions.
2. If you want to use this CSS on your website, you must provide the link of this repository in the comment or footer (https://github.com/QamarQ/w11-css-components-kit/)



