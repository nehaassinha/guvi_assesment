    Jun 21, 2021
    Task
    1) Do the below programs in anonymous function & IIFE (Immediately Invoked Function Expression )
    a. Print odd numbers in an array
		
		 let arr=[1,2,5,6,8,4,12,11,77];
		 let a= (function(){
					var s=[];var c=0;
					for(let i=0;i<arr.length;i++)
					{
						if(arr[i]%2===0) s[c++]=arr[i];
					}
				return s;
				});
		console.log(a());
		
    IIFE Function:-
		let arr=[1,2,5,6,8,4,12,11,77];
		(function()
			{
					var s=[];var c=0;
					for(let i=0;i<arr.length;i++)
					{
						if(arr[i]%2===0) s[c++]=arr[i];
					}
				console.log(s);
			}
		)();
		
    b. Convert all the strings to title caps in a string array
		
		let str="My name is Neha";
		let a= (function(){
					var s="";
					for(let i=0;i<str.length;i++)
					{
						s+=str[i].toUpperCase();
					}
				return s;
				});
		console.log(a());
		
    IIFE Function-
    
      let str="My name is Neha";
		  (function(){
					var s="";
					for(let i=0;i<str.length;i++)
					{
						s+=str[i].toUpperCase();
					}
			console.log(s);
		  })();
    
    c. Sum of all numbers in an array
		
		let arr=[1,2,5,6,8,4,12,11,77];
		let a= (function(){
					var s=0;
					for(let i=0;i<arr.length;i++)
					{
						s+=arr[i]
					}
				return s;
				});
		console.log(a());
		
    IIFE Function-
    
       let arr=[1,2,5,6,8,4,12,11,77];
		  (function(){
					var s=0;
					for(let i=0;i<arr.length;i++)
					{
						s+=arr[i]
					}
				console.log(s);
		  })();
    
    d. Return all the prime numbers in an array
		
		let arr=[1,2,5,6,8,4,12,11,77];
		let a= (function(){
					var s=[];var c=0;
					for(let i=0;i<arr.length;i++)
					{	let count=0;
						for(let j=1;j<=arr[i];j++)
						{
							if(arr[i]%j===0) count++;
						}
						if(count===2 && arr[i]!==1) 
							s[c++]=arr[i];	
					}
				return s;
			});
		console.log(a());
		
    IIFE Function-
     
     let arr=[1,2,5,6,8,4,12,11,77];
		 (function(){
					var s=[];var c=0;
					for(let i=0;i<arr.length;i++)
					{	let count=0;
						for(let j=1;j<=arr[i];j++)
						{
							if(arr[i]%j===0) count++;
						}
						if(count===2 && arr[i]!==1) 
							s[c++]=arr[i];	
					}
				console.log(s);
			})();
     
    e. Return all the palindromes in an array
		
		let arr=[12,22,151,10];
		let a= (function(){
					var s=[];var c=0;
					for(let i=0;i<arr.length;i++)
					{	
						let str=arr[i].toString().split("").reverse().join("");
						if(arr[i]===+str){ s[c++]=arr[i];}
					}
				return s;
			});
		console.log(a());
		
    IIFE Function-
    
     let arr=[12,22,151,10];
		 (function(){
					var s=[];var c=0;
					for(let i=0;i<arr.length;i++)
					{	
						let str=arr[i].toString().split("").reverse().join("");
						if(arr[i]===+str){ s[c++]=arr[i];}
					}
				console.log(s);
			})();
    
    f. Return median of two sorted arrays of same size 
		
		let arr1=[10,12,15,22,151];
		let arr2=[1,2,3,4,5];
		let a= (function(){
				let arr = [...arr1, ...arr2];
				arr.sort((a,b) => a-b);
				//console.log(arr);
				let l=arr.length/2;
				let s= (arr[l]+arr[l-1])/2;
			return s;
		});
		console.log(a());
		
    IIFE Function-
    
      let arr1=[10,12,15,22,151];
		  let arr2=[1,2,3,4,5];
		  (function(){
				let arr = [...arr1, ...arr2];
				arr.sort((a,b) => a-b);
				//console.log(arr);
				let l=arr.length/2;
				let s= (arr[l]+arr[l-1])/2;
			  console.log(s);
		  })();
    
    g. Remove duplicates from an array
		
		let chars = ['A', 'B', 'A', 'C', 'B'];
		let uniqueChars = (function(){
			let str=[];
				for(c of chars) {
					if (!str.includes(c)) {str.push(c);}
				}
				return str;
			});
      console.log(uniqueChars());
		
    IIFE Function-
      let chars = ['A', 'B', 'A', 'C', 'B'];
		  (function(){
			let str=[];
				for(c of chars) {
					if (!str.includes(c)) {str.push(c);}
				}
				console.log(str);
			})();
    
    h. Rotate an array by k times 
		
		let a=[1,2,3,4,5,6,7,8,9,10];
		let k=2;
		let rotateArr = (function(){
			for(let i=0;i<k;i++){
				let temp=a[a.length-1];
					for(let j=a.length-1;j>0;j--){
						a[j]=a[j-1];
					}
				a[0]=temp;
			}
		return a;
		});
		console.log(rotateArr());
		
    IIFE Function-
    
      let a=[1,2,3,4,5,6,7,8,9,10];
		  let k=2;
		  (function(){
			for(let i=0;i<k;i++){
				let temp=a[a.length-1];
					for(let j=a.length-1;j>0;j--){
						a[j]=a[j-1];
					}
				  a[0]=temp;
			  }
		  console.log(a);
		  })();
    
    2) https://medium.com/@reach2arunprakash/guvi-zen-class-javascript-warm-up-programming-problems-15973c74b87f  (for practice)
    a. var num = 10;
    function addFive(num) {
			return num+5;
    }
    var result = addFive(num)
	   
    b. 
    var num=5;   
    function getOpposite(num) {
    	if(Number.isInteger(num)){
       		return -1*num;
    	}
    	else{
        	return -1;
    	}
    }
    var result = getOpposite(num);
    console.log(result);
    
    c.  var min = 5;
	function toSeconds(min) {
        	return 60*min;
	}
	var secs = toSeconds(min); 
    	console.log(secs);
    
    d.  var mystr = "5";
	function toInteger(mystr) {
		return +mystr;
	}
	var myint = toInteger(mystr)
    	console.log(myint);
    
    e.  var myint = 0;
	function nextNumber(myint) {
		return ++myint;
	}
	var myNextint = nextNumber(myint)
    	console.log(myNextint);
	
    f.  var arr = [1, 2, 3];
	function getFirstElement(arr) {
		return arr[0];
	}
	var data = getFirstElement(arr)
    	console.log(data);
	
    g. var hr = 2;
	function hourToSeconds(hr) {
   		 return 60*60*hr;
	}
	var data = hourToSeconds(hr)
	console.log(data);
	
    h. function findPerimeter(num1,num2) {
    		return (2*num1+2*num2);
	}
	var peri = findPerimeter(6,7)
    	console.log(peri);
    
    i. function lessThan100(num1,num2) {
    		 if(num1+num2 >100) return false;
    		 else    return true;
	}
	var res = lessThan100(22,15)
	console.log(res);
    
    j. function remainder(num1,num2) {
        return +(num1%num2);
	}
	var res = remainder(1,3)
	console.log(res);
    
    k.function CountAnimals(tur,horse,pigs) {
   	 return tur*2+horse*4+pigs*4;
    	}
	var legs = CountAnimals(2,3,5);
	console.log(legs);
    
    l. function frames(num1,num2) {
    		return num1*num2*60;
	}
	var fps = frames(1,2);
	console.log(fps);
    
    m. function divisibleByFive(num1) {
   	if(num1%5===0) {return true;}
   	 else {return false;}
	}
	var divisible = divisibleByFive(5)
	console.log(divisible);
    
    n.  function isEven(num){
	 if(Number.isInteger(num)){
 	  if(num%2===0)    return true;
  	  else    return false; 
  	 }
	 else{ return -1;}
	}
	var even = isEven(5);
	console.log(even);
    
    o. function areBothOdd(num1, num2){
    	 if(num1%2!==0 && num2%2!==0)  console.log("true");
   	  else    console.log("false");
	}
	areBothOdd(1, 3);
    
    p. function getFullName(firstName, lastName){
    	 console.log(firstName+lastName);
	}
	getFullName(“GUVI”,“GEEK”);
    
    q. function getLengthOfWord(word1){
	console.log(word1);
	if(isNaN(word1))
    	console.log(word1.length); 
	else
 	console.log("-1");  
	}
	getLengthOfWord("abc");
    
    r. function isSameLength(word1, word2){
     		if(word1.length === word2.length){
			return true;
		}
		else  return false;
	}
    	console.log(isSameLength("GUVI", "GEEK"));
	
    s.  console.log(getDistance(100, 100, 400, 300));
	function getDistance(x1, y1, x2, y2)
	{
 		let d=Math.sqrt(((x2-x1)*(x2-x1)) + ((y2-y1)*(y2-y1)));
		return d;
	}

    t. 	console.log(getNthElement([1, 3, 5], 1));
    	function getNthElement(array,n){
 	return array[n];
	}


    u. 
    console.log(getLastElement([1, 3, 5]));
    function getLastElement(array){
	return array[array.length-1];
	 }
    
    v.  var obj = {
 	mykey: “value”
	};
	function getProperty(obj, key) {
			return obj.key;
	}
    	console.log(getProperty(obj,'mykey'));
	
    w.  var obj = {
 	mykey: "value"
	};
	function getProperty(obj, key) {
			return obj[key];
	}
    	console.log(getProperty(obj,'mykey'));
    
    x.  var obj = {
	 mykey: "value"
	};
	function addProperty(obj, key){
		obj[key]=true;
        console.log(obj);  
	}
	addProperty(obj, "key");
	
    y. 
    	removeProperty(obj, "name");
    	var obj = {
	 mykey: "value",
	 name:"Neha Sinha"
	};
	function removeProperty(obj, key){
		delete obj.key;
        console.log(obj);  
	}
	
    z. 
    	var arr = [-5, 10, -3, 12, -9, 5, 90, 0, 1];
	var ar2 = function countPositivesSumNegatives(arr) {
		let ar=[];let count =0;let s=0;
 		for(let i=0;i<arr.length;i++){
			if(arr[i]>-1){
				count++;
			}
			else{
				s+=arr[i];
			}
		}
		ar[0]=count;
		ar[1]=s;
		return ar;
	}
	console.log(ar2(arr));
	
	A.
	function getPositives(ar)
	{	let arr=[];let count =0;
		for(let i=0;i<ar.length;i++){
			if(ar[i]>-1){
				arr[count++]=ar[i];
			}
		}
		return arr;
	}
	var ar = [-5, 10, -3, 12, -9, 5, 90, 0, 1];
	var ar2 = getPositives(ar);
	console.log(ar2);
	
	B.
	var ar=powersOfTwo(2);
	console.log(ar);
	function powersOfTwo(n){
  		let res=[];
		for(let i=0;i<=n;i++){
			res[i]=Math.pow(2,i);
		}
  	return res;
	}
	
	
	C.
	function findMax(ar)
	{
		let max=ar[0];
		for(let i=0;i<ar.length;i++){
			if(max<ar[i]) max=ar[i];
		}
		return max;
	}
	var ar = [-5, 10, -3, 12, -9, 5, 90, 0, 1];
	var max = findMax(ar);
	console.log("Max: ", max);
	
	D.
	printPrimes(100);
	// Function prints the first nPrimes numbers
	function printPrimes(nPrimes)
	{
	 	var n = 0;var i = 2;
 		while(n < nPrimes)
 		{
 			if (isPrime(i))
 			{
	 			console.log(n, " → ", i);
 				n++;
 			}
 		i++;
 		}
	}
	// Returns true if a number is prime
	function isPrime(n)
	{	let c=0;
		for(let i=1;i<=n;i++){
			if(n%i===0) c++
		}
		if(c===2 && n!==1)  return true;
		else  return false;
	}
	
	E.
	console.log(getPrimes(10, 100));
	function getPrimes(nPrimes, startAt)
	{	let ar=[];let c=0;
		while(c<nPrimes){
			if(isPrime(++startAt)) {
				ar[c++]=startAt;
			}
		}
		return ar;
	}
	function isPrime(n)
	{
		let c=0;
		for(let i=1;i<=n;i++){
			if(n%i===0) c++
		}
		if(c===2 && n!==1)  return true;
		else  return false;
	}
	
	
	F.
	var s = reverseString("JavaScript");
	console.log(s);
	function reverseString(s)
	{
 	  return s.split("").reverse().join(""); 
	}
	
	G.
	var ar1 = [1, 2, 3];
	var ar2 = [4, 5, 6];
	var ar = mergeArrays(ar1, ar2);
	console.log(ar);
	function mergeArrays(ar1, ar2)
	{
 		var result = [];
		//this will add the first array to the result array
		for(let el of ar1)
 		{
 		result.push(el);
 		}
		//this will add the second array to the result array
		for(let el of ar2)
 		{
 			result.push(el);
 		}
 		return result;
	}	
	
	H.
	
	console.log(sumCSV("1.5, 2.3, 3.1, 4, 5.5, 6, 7, 8, 9, 10.9"));
	function sumCSV(s)
	{	let arr=s.split(",");let sum=0;
 	 	for(let el of arr)
 		{
			sum+=(+el);
 		}
		return sum;
	}
    
    3) Do the below programs in arrow functions
        a. Print odd numbers in an array 
		
		let a=[1,2,3,4,5,6,7,8,9,10];
		let odd=(arr)=>{
				let s=[],c=0;
				arr.forEach((i) => { if(i%2!==0)s[c++]=i;});
				return s;
		};
		console.log(odd(a));
		
		
        b. Convert all the strings to title caps in a string array
        
		let str="My name is Neha";
		let cap_str=(s)=>{
				let s1="";
				s.forEach((i) => { s1+=i.toUpperCase();});
				return s1;
		};
		console.log(cap_str(str.split("")));
		
		
		c. Sum of all numbers in an array
        
		let a=[1,2,3,4,5,6,7,8,9,10];
		let sum=(arr)=>{
				let s=0;
				arr.forEach((i) => { s+=i;});
				return s;
		};
		console.log(sum(a));
		
		d. Return all the prime numbers in an array
        
		let arr=[1,2,5,6,8,4,12,11,77];
		let prime_arr= (arr)=>{
		var s=[];var c=0;
		arr.forEach((i)=>
			{	let count=0;
				for(let j=1;j<=i;j++)
				{
				     if(i%j===0) count++;
				}
				if(count===2 && i!==1) s[c++]=i;
				
			});return s;
		};
		console.log(prime_arr(arr));
		
		e. Return all the palindromes in an array
		
		let arr=[12,22,151,10];
		let pal_arr= (a)=>{
			var s=[];var c=0;
				a.forEach((i)=>
				{
					let str=i.toString().split("").reverse().join("");
					if(i===+str){ s[c++]=i;}
				});
			return s; 
		};
		console.log(pal_arr(arr));
