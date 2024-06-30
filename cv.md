# Nikita Simonov
### _junior front-end developer_ ###
### My contact information: ###
 * #### Number: _+7 (919) 376-72-66_ #### 
 * #### Mail: _ngsimonov@yandex.ru_ ####
 * #### Telegram: [_@troyez_](t.me/troyez) ####
 * #### GitHub: [_@troyezg_](https://github.com/troyezg) ####

# About me #
#### I have been interested in programming and especially web development for quite a long time. However, most of my knowledge was acquired on my own, which is why there are many gaps. In order to fill these knowledge gaps and learn React, I decided to take the Rolling Scopes School courses. ####

# Skills #
 * #### Programming languages: C#, C++, Java, Python, JavaScript, HTML, CSS, Node, PHP, MySQL, VBA ####
 * #### Frameworks and libraries: Vue.js, Express.js, MySQL.js ####
 * #### Motion Design: Adobe Photoshop, Adobe illustrator, Figma, Davinci Resolve ####

# Code example's #
#### This script allows you to add additional form by clicking "Add Step" button to add an additional step on the post loading page. ####

```javascript
try {
const node5 = document.getElementById('addstepbutton');
var stepnubmer = 1;
document.addEventListener('click', function(d) {  
  if (node5.contains(d.target)) {
    const steps = document.getElementById("createpostcontainer");
    stepnubmer = stepnubmer + 1;
    console.log(stepnubmer);
    steps.insertAdjacentHTML( "beforeend", '<div class="addstepform"><textarea class="addstepformtext" id="addstepform' + stepnubmer +'" placeholder="Шаг ' + stepnubmer + ' "></textarea><input type="file" class="loadimagestep" id="loadimagestep' + stepnubmer + '"></div>');
  }
})
} catch (error) {
  console.error(error);
}
```
#### This script allows you to search for the posts with similar post name. By clicking enter you clearing the feed and sending the search information to API by calling lentaload function. ####

```javascript
try {
var searchbar = document.getElementById("search");
searchbar.addEventListener("keyup", function(event){
  if (event.key == "Enter") {
    const lentabodyid = document.getElementById("lentacontainer");
    lentabodyid.innerHTML = '';
    searchname = searchbar.value;
    posts = 10;
    lentaload();
  }
  if (searchbar.value == '' && event.key == "Backspace") {
    const lentabodyid = document.getElementById("lentacontainer");
    lentabodyid.innerHTML = '';
    searchname = undefined;
    posts = 10;
    lentaload();
  }
})
} catch (error) {
  console.error(error);
}
```

# Frontend Junior Developer expirience #

* #### [My first vue project](https://github.com/troyezg/vue-project) which i did as a test for the job. This project was created using figma's design and API to load cards into the feed. It takes me 3 days to code this project considering that i was learning vue and API while coding. However it was verry fun and interesting, i learned a lot of new by working on this project. ####

```javascript
getCurrentPageData() {
fetch(this.request)
.then(response => response.json())
.then(data => {
  this.TotalCards = (Object.keys(data.data)).length;
if (data.meta.current_page <= data.meta.last_page) {
  this.CurrentPage = data;
} else {
  page = data.meta.last_page;
}
this.PerPageCounter();
})
.catch(error => {
console.error('Произошла ошибка:', error);
});
}
```

* #### This is [another test project](https://github.com/troyezg/another-test-project) that i did for another job. It was also created from figma's design, but this time it was pretty simple. The only difficulty here was the implementation of the progress bar, which had to be done using the css variable. ####

```html
<div class="showcase">
	<div class="mainframe">
		<button class="openchecklist" id="openchecklist"><p class="buttontext">Открыть чеклист</p></button>
		<div class="eventname">
			<p class="eventtext">Чеклист</p>
		</div>
		<p class="bigtext">Выполнено: 3 из 7 действий</p>
		<p class="smalltext">Следующее действие: Созвониться с клиентом до 23.05.24 12:00</p>
		<div class="progressbarback" style="--progress: 42%;">
			<svg class="svgblock">
				<circle class="scale-progress" r="29.5px" cy="50%" cx="50%"></circle>
			</svg>
		</div>
		<p class="counter">3/7</p>
	</div>
</div>
```

* #### Currently im working on the multipage website for my graduate work using HTML5, CSS, JavaScript, Node.js, MySQL, React.js. This site is not ready yet, so it doesn't have a GitHub page yet, but i can show you some code. ####

```javascript
try {
  document.addEventListener('DOMContentLoaded', function() {
    fetch('http://localhost/ingridients')
      .then(response => response.json())
      .then(data => {
       y = data;
        for (var rollingcycling = 0; rollingcycling < y.length; rollingcycling++) {
          const ingridientlist = document.getElementById("rollinglist2");
          ingridientlist.innerHTML += '<div class="checkboxform"><input type="checkbox" id="ingridient-' + y[rollingcycling].id + '" style="accent-color: #E53935;"> <label for="ingridient-' + y[rollingcycling].id + '" class="rollinglist2text">'+ y[rollingcycling].i_name +'</label></div>';
        }  
      })
      .catch(error => {
        console.error('Произошла ошибка:', error);
      });
  }); 
} catch (error) {
  console.error(error);
}
```

# Education #
#### At the moment I am finishing my studies at USPU with a specialization in Information Systems and Technologies. ####

# Languages #
* #### English Language: ####

     #### I have been learning English since first grade because my school focused on teaching English. At the moment i know English on the B1 level. I can freely understand english while watching some video's or reading some text's. Sometimes I have to read documentation in English, which is quite simple for me. ####