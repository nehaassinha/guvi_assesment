     Solving problems using array functions on rest countries data. 
       1) Get all the countries from Asia continent /region using Filter function
      Solution -  
         var xhr = new XMLHttpRequest();
         xhr.open("GET", "https://restcountries.eu/rest/v2/all");
    xhr.onload = function () {
      var data = JSON.parse(this.response);
      //console.log(data);
	  var country=data.filter(function (data){
		  if(data.region="Asia")
		  console.log(data.name);
	  });
    };
    xhr.send();
    
        2) Get all the countries with a population of less than 2 lakhs using Filter function
        Solution:-
        var xhr = new XMLHttpRequest();
    xhr.open("GET", "https://restcountries.eu/rest/v2/all");
    xhr.onload = function () {
      var data = JSON.parse(this.response);
      //console.log(data);
	  var country=data.filter(function (d){
		  if(d.population<200000){
		  console.log(d.name);
		  return d.name;
		  }
	  });
	  //console.log(country);
    };
    xhr.send();
        
        3) Print the following details name, capital, flag using forEach function 
        Solution:-
        var xhr = new XMLHttpRequest();
    xhr.open("GET", "https://restcountries.eu/rest/v2/all");
    xhr.onload = function () {
      var data = JSON.parse(this.response);
      //console.log(data);
	  data.forEach(d=>{
		  console.log(d.name +", "+d.capital+", "+d.flag);
	  });
    };
    xhr.send();
        
        4) Print the total population of countries using reduce function 
        Solution-
        
        
        5) Print the country which use US Dollars as currency.
         Solution:-
         
         
         
