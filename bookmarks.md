```
deviant art age bypass:
javascript:(function()%7B(function()%20%7Bfunction%20jsonp(url%2C%20callback)%20%7Bvar%20callbackName%20%3D%20'jsonp_callback_'%20%2B%20Math.round(100000%20*%20Math.random())%3Bwindow%5BcallbackName%5D%20%3D%20function(data)%20%7Bdocument.body.removeChild(script)%3Bcallback(data)%3B%7D%3Bvar%20script%20%3D%20document.createElement('script')%3Bscript.src%20%3D%20url%20%2B%20'%26format%3Djsonp%26callback%3D'%20%2B%20callbackName%3Bdocument.body.appendChild(script)%3B%7Djsonp(%22http%3A%2F%2Fbackend.deviantart.com%2Foembed%3Furl%3D%22%20%2B%20encodeURIComponent(document.URL.split(%22%3F%22)%5B0%5D)%2C%20function(data)%20%7Bwindow.location.href%3Ddata%5B%22url%22%5D%3B%7D)%3B%7D())%7D)()
```

removeddit:
```javascript: document.location = document.URL.replace('reddit.com','removeddit.com')```

postHN:
```javascript:window.location=%22https://news.ycombinator.com/submitlink?u=%22+encodeURIComponent(document.location)+%22&t=%22+encodeURIComponent(document.title)```

dl-R:
```javascript: if (window.location.href.indexOf('reddit.com') > -1) {(function() {let open = window.open; open.opener = null; open('https://redditsave.com/info?url='  + window.location.pathname.slice(0))})()}```

dl-pdf:
```javascript:(function()%7Bfunction%20callback()%7B(function(%24)%7Bvar%20jQuery%3D%24%3B%24(%22aalink%22).each(function%20()%7B%24(this).trigger('click')%3Bvar%20href%20%3D%20%24(this).attr(%22href%22)%3B%7D%7D)%7D)(jQuery.noConflict(true))%7Dvar%20s%3Ddocument.createElement(%22script%22)%3Bs.src%3D%22https%3A%2F%2Fajax.googleapis.com%2Fajax%2Flibs%2Fjquery%2F1.11.1%2Fjquery.min.js%22%3Bif(s.addEventListener)%7Bs.addEventListener(%22load%22%2Ccallback%2Cfalse)%7Delse%20if(s.readyState)%7Bs.onreadystatechange%3Dcallback%7Ddocument.body.appendChild(s)%3B%7D)()
```

