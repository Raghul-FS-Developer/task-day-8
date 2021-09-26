(a).
fetch("https://restcountries.com/v3/all")
.then(data=>data.json())
.then(countries=>
      countries.filter((country) =>country.region = "asia"))
.then(country=>console.log(country))




(b).
fetch("https://restcountries.com/v2/all")
.then(data=>data.json())
.then(countries=>
      countries.filter((country) =>country.population < 200000))
.then(country=>console.log(country))


(c)
fetch("https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json")
.then(data=>data.json())
.then(countries => {
  countries.forEach(country=>{console.log(country.name)
                              console.log(country.capital)
                              console.log(country.flag)
    
  })
})

