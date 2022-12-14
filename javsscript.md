# Dom Manipulation Assignment

1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./images/Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

```js
document.getElementsByClassName("crayons-subtitle-2 lh-tight mb-4")[1].textContent = "Omkar";
document.getElementsByClassName("color-base-70 mb-4")[1].textContent = "Problem Solving";
```

### Output

![Output](./Output/1st_assgn.png)

---

2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./images/Picture_3.png)

### Fetch all the product name and store in an array

```js
const grid = document.getElementsByClassName("as-imagegrid-item-title");
let devices = [];
for (const each of grid){
    devices.push(each.textContent.replace(" Support", ""));
};
```

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']
---

3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child


### Sample Image

![Sample One](./images/Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

```js
const faq = document.getElementsByClassName("accordion-homepage");
const sec = document.createElement("section");
sec.className = "parent";
sec.innerHTML = '<h3 role="button" tabindex="0" aria-expanded="false" aria-label="Policy, safety and copyright">My New FAQ<svg class="up" viewBox="0 0 24 24"><path d="M7.41 15.41L12 10.83l4.59 4.58L18 14l-6-6-6 6z"></path></svg><svg class="down" viewBox="0 0 24 24"><path d="M7.41 7.84L12 12.42l4.59-4.58L18 9.25l-6 6-6-6z"></path></svg></h3>';
faq[0].appendChild(sec);
```

### Output

![Output](./images/Pic5.png)

---

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./images/Pic6.png)

### Tasks

      Change the contact number

```js
const elem = document.querySelector(".one-tel-number.service-number");
elem.innerText = "+91 6366256689";
```

### Output

![Output](./images/Pic7.png)

---
5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./images//Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out


```js
const btn = document.querySelector(".diwali-deals-product-sale-btn");
btn.innerText = "Check Out";
```

### Output

![Output](./images/Pic9.png)

---

6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./images/Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

```js
const search = document.querySelector(".searchinput___19uW0");
function mouseHoverFunction(){
    search.style.backgroundColor = "red";
};
search.addEventListener("mouseover",mouseHoverFunction);
```

### Output

![Output](./images/Pic11.png)

---

7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./images/Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

```js
const inp = document.querySelector("#hp-search-input");
inp.value = "CSS Selectors";
const form = document.querySelector("#hp-search-form");
form.submit();
```

### Output

![Output](./images/Pic13.png)

---

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./images/Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

```js
let lang = document.querySelectorAll(".z4hgWe > a");
for (let i= 0; i < lang.length; i++){
    if ( i % 2 === 0){
        lang[i].remove();
    }
}
```

### Output

![Output](./images/Pic15.png)

---

9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./images/Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo???s background color.

```js
const elem = document.getElementsByClassName("display-heading-1");
elem[0].style.fontFamily = "Monospace";
elem[0].style.color = "red";
```

### Output

![Output](./images/Pic17.png)

---
10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./images/Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

```js
const btn = document.getElementsByClassName("login-btn-text")[1];
function changeColor(){
    btn.style.backgroundColor = "red";
}
btn.addEventListener("mouseover", changeColor);
```

### Output

![Output](./images/Pic19.png)

---

11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./images/Pic20.png)

### Tasks

    change the realme logo to ineuron logo

```js
const logo = document.querySelector(".icon.icon-logo.in");
logo.style.backgroundImage = "url(https://ineuron.ai/images/ineuron-logo.png)";
```

### Output

![Output](./images/Pic21.png)

---

12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./images/Pic22.png)

### Tasks

     change the background colour of the button to blue.
     
```js
const btn = document.querySelector(".btn.btn-sm.btn-primary");
btn.style.background = "blue";
```

### Output

![Output](./images/btn.png)

---

13.  Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./images/Pic24.png)

### Tasks

Target the top description and change ???Matching developers with great companies??? to ???JSBOOTCAMP???.

```js
const text = document.querySelector("#post-5780 .fl-heading-text");
text.textContent = "JSBOOTCAMP";
```

### Output

![Output](./images/Pic25.png)

---

14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./images/Pic26.png)

### Tasks

       change the fontsize of ???Hot Deals??? to 80px

```js
const text  = document.querySelector(".HotDealsAll__Heading__2fIbe");
text.style.fontSize = "80px";
```

### Output

![Output](./images/Pic27.png)

---

15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./images/Pic28.png)

### Tasks

       Convert the text ???G15 Gaming Laptop??? from left to right

```js
const lap = document.querySelector("#d560824win9b");
lap.querySelector(".ps-title").style.textAlign = "right";
```

### Output

![Output](./images/Pic29.png)

---

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./images/Pic30.png)

### Tasks

      change the heading ???Start with the developer??? to ???Start with Scratch???

```js
const text = document.querySelector(".section-title_title__VEDfK");
text.textContent = "Start with scratch";
```

### Output

![Output](./images/Pic31.png)

---

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./images/Pic33.png)

### Tasks

     change the button text To current Date.

```js
const button = document.querySelector(".btn-container")
button.innerHTML = new Date;
```

### Output

![Output](./images/Pic32.png)

---

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./images/Pic34.png)

### Tasks

    change the background colour blue to orange

```js
const footer = document.querySelector(".p-footer");
footer.style.backgroundColor = "orange";
```

### Output

![Output](./images/Pic35.png)

---

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./images/Pic36.png)

### Tasks

    extract the canon logo

```js
const imageSrc = document.querySelector(".navbar-brand > .logo").src;
```

### Output

![Output](./images/Pic37.png)

---

20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./images/Pic38.png)

### Tasks

      Change the description colour black to orange

```js
const text = document.querySelector(".wide .desc");
```

### Output

![Output](./images/Pic39.png)

---