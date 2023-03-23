# Pavel Fursevich

---

### Contacts

- **Location:** Minsk, Belarus
- **Email:** edelwei14ss@gmail.com
- **Telegram:** @wiseseal
- **[Linkedin](https://www.linkedin.com/in/edelweiss/)**
- **[Github](https://github.com/PaulusWhite)**

---

### About me

I have been interested in programming since of 2020. In the end of that year I decided to start my studies in this sphere. At first I had taken several paid courses in my city, after that I preferred to study by myself. Unfortunately I did not have opportunity to devote enough time to my self education, so because of it programming was like a favorite hobby for me.
Now I have prioritized and finnaly put web development at first place. Today I spend all my time on self education, place enormous emphasis on English and also I am ready to spend as much time on my future career as it needed.

---

### Skills and abilities

- HTML
- CSS/SASS(SCSS)
- JavaScript
- TypeScript
- React
- Redux (Redux Toolkit)
- React-redux
- Git/Github
- API, NPM, JSON, BEM
- Firebase

---

### Code examples

```
let getWeatherForecast = async (location: string) => {
    let options = {
        method: 'GET',
        url: 'https://weatherapi-com.p.rapidapi.com/forecast.json',
        params: {q: location, days: '3'},
        headers: {
          'X-RapidAPI-Key': '8012bd5a3amsh1191195c3b8dbf4p1ef8ffjsn75cd7de35e4a',
          'X-RapidAPI-Host': 'weatherapi-com.p.rapidapi.com'
        }
    };
    try{
        let response = await axios.request(options);
        let forecastday = response.data.forecast.forecastday;
        let location = response.data.location;

        let dailyForecast: DailyForecastI[] = getDailyForecast(forecastday, location);
        let todayForecast: DailyForecastI = getNowForecast(response, location, dailyForecast[0].astro, dailyForecast[0].hourlyForecast);

        return { status: 200, data: { todayForecast, dailyForecast }};
    }catch(error){
        return {status: 400, error };
    }
}
```

---

### Experience

Here are my pet projects:

- BookHunter

  - **Description:** The online bookstore where you can find any book you want (it is used Google Books API), sign up and sign in (it is used Firebase), make a purchase. It was big job for me as graduation project after my React learning
  - **Written with:** React
  - **Source:** https://github.com/PaulusWhite/bookhunter-app
  - **Notes:** You can check the app on your localhost. **The app does not work on the area of Republic of Belarus (you must use VPN)**

- WeatherToday

  - **Description:** The weather forecast as graduation project after my TypeScript learning
  - **Written with:** React + TypeScript
  - **Source:** https://github.com/PaulusWhite/weatherToday-app
  - **Notes:** You can check the app on your localhost

  ***

### Education

- IT Academy (https://www.it-academy.by/about/it-academy/)
  - Preparatory course "Basics of web technologies" (07.10.2020 - 04.11.2020)
  - The training course "Development of websites using HTML and CSS" with a small JavaScript module (02.12.2020 - 08.02.2021)
  - Web application development with JavaScript (05.05.2021 - 18.08.2021)
- Udemy

  - [React Front To Back](https://www.udemy.com/share/105yDQ3@9T2z8LMEU0APP4WQGliGXREMV6YR9egd4PFbWxWuM0oI7XVREMBOAZdbiSrhQqEozA==/) (01.01.2022 - 20.02.2022)

  ***

### Knowledge of languages

- English - Strong Intermediate Plus (CEFR B1+)
- Ukrainian - Perfect on understanding level
- Belarussian - Native
- Russian - Native
