June 17, 2021
Task
    1)
    var obj = [
          { person: "Name 1", age: "2", company: "GUVI" },
          { person: "Name 2", age: "5", company: "GUVI geek" },
          { person: "Name 3", age: "8", company: "GUVI geek network" },
        ]
    use the above JSON to iterate over all for loops (for, for in, for of, forEach)
	
	Answer:-
	a. for loop
		
		for (let i=0;i<obj.length;i++) {
			for (var j in obj[i]) {
				console.log(j + ':'+obj[i][j]);
			}
		}
		
	
	b. for in loop
		
				
		for (var i in obj) {
			for (var j in obj[i]) {
				console.log(j + ':'+obj[i][j]);
			}
		}
		
	c. for of loop
		
				
		for (let i=0;i<obj.length;i++) {
			for (const key of Object.keys(obj[i])) {
				console.log(key+" : "+ obj[i][key]);
			}
		}

	
	d. forEach loop
		
		for (let i=0;i<obj.length;i++) {
			Object.keys(obj[i]).forEach(function(key) {
					console.log(key+" : "+ obj[i][key]);
			});
		}
	
    2)
        var xhr = new XMLHttpRequest();
        xhr.open("GET", "https://restcountries.eu/rest/v2/all");
        xhr.onload = function () {
          var data = JSON.parse(this.response);
          console.log(data);
        };
        xhr.send();
    use the restcountries API url ->  https://restcountries.eu/rest/v2/all
    and diplay all the country flags in console
	
	Answer:-
	    index.html --------------------- html file
		
			<!doctype html>
				<html>
					<head>
						<title>Test</title>
					</head>
					<body>
						<script type="text/javascript" src="test_flag.js"></script>
					</body>
				</html
	
		test_flag.js  ------------------- js file
		
		var xhr = new XMLHttpRequest();
        xhr.open("GET", "https://restcountries.eu/rest/v2/all");
        xhr.onload = function () {
          var data = JSON.parse(this.response);
          //console.log(data);
		  for(let i in data){
			  // console.log(data[i]);
			
			  for(let j in data[i]){
				  if(j=='flag')
			   console.log(data[i][j]);
				//console.log(data[i]['flag']);
			  }
		    }
        };
        xhr.send();
    3) 
    use the same restcountries and print all countries name, region, sub region and population.
	
	Answer:-
	
		index.html --------------------- html file
		
			<!doctype html>
				<html>
					<head>
						<title>Test</title>
					</head>
					<body>
						<script type="text/javascript" src="test_flag.js"></script>
					</body>
				</html
	
		test_flag.js  ------------------- js file
		
		var xhr = new XMLHttpRequest();
        xhr.open("GET", "https://restcountries.eu/rest/v2/all");
        xhr.onload = function () {
          var data = JSON.parse(this.response);
          //console.log(data);
		  for(let i in data){
			  for(let j in data[i]){
					console.log("Name:"+data[i]['name']+",Region:"+data[i]['region']+",SubRegion:"+data[i]['subregion']+",Population:"+data[i]['population']);
			  }
		    }
        };
        xhr.send();
	
    4) read about the difference between window, screen and document in javascript
	
	Answer
	Window is the main JavaScript object root, aka the global object in a browser, and it can also be treated as the root of the document object model. You can access it as window.

	window.screen or just screen is a small information object about physical screen dimensions.

	window.document or just document is the main object of the potentially visible (or better yet: rendered) document object model/DOM.

	Since window is the global object, you can reference any properties of it with just the property name - so you do not have to write down window. - it will be figured out by the runtime.
	
	https://stackoverflow.com/questions/9895202/what-is-the-difference-between-window-screen-and-document-in-javascript
	