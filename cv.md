# Tatiana Yudakova
#### Contact Info

Samara, Russia
* Telephone: +7-909-370-11-55
* E-mail: yudakovatl@gmail.com

#### Summary

I am a creative person who wants to develop in the field of frontend development. Not afraid to face difficult tasks. I like to learn new technologies.

#### Skills

* *Programming languages:* Java, JavaScript, C#, PL/SQL
* *Frameworks:* Spring, Hibernate
* *Build tool:* Maven
* *Version control:* Git

#### Code examples

Code from project "Weather forecast", where I get weather data from online service [Openweathermap](https://openweathermap.org/):
```javascript
window.onload = function() {
	var xhr = new XMLHttpRequest();

	xhr.open('GET', 'https://api.openweathermap.org/data/2.5/forecast?id=499099&units=metric&lang=ru&appid=22d697eb938c6d57b2a4ec8f405bcf84', false);

	xhr.send();

	if (xhr.status != 200) {
	  alert( xhr.status + ': ' + xhr.statusText );
	} else {
	 fillWeatherForecastArray(xhr.responseText);
	 insertWeather(currentweatherForecastArray);
	 checkedDisabledButtons();
	}
};
```
