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
