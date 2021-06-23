1. 
aa = (f,s,t) => {
 //let f,s,t;  already declared
 console.log(f,s,t);
 if(f>s &&f>t){
 console.log(f)}
 else if(s>f && s>t){
 console.log(s)}
 else{
 console.log(t)}
}
aa(1,2,3);

2.
let n=123;
console.log(add(n));
function add(n)
{
	n=n.toString();
let sum = 0;
for(var i=0;i<n.length;i++){
 sum+=  +n[i]
 }
 return sum;
}

3.
 const arr = [9,8,5,6,4,3,2,1];
(function() {
 let sum = 0;
 for (var i = 0; i < arr.length; i++){
 sum += +arr[i];
 }
 console.log(sum);
 return sum;
})();

4. 
var arr = ["guvi", "geek","zen", "fullstack"];
var ano = function(arro) {
 for (var i = 0; i<arro.length;i++) {
 console.log(arro[i][0].toUpperCase() + arro[i].substr(1));
 }
}
ano(arr);

5.
const newArray=[1,3,2,5,10];

const myPrime=newArray.filter(num=>{
    let count=0;
 for(let i=2;i<=num;i++){
 if(num%i===0)
 {
     count++;
 }
 }
 if(count===1) return num;
});
console.log(myPrime);

6.
const num = [10, 20, 30, 40,50,60,70,80,90,100] 
const sum = (a, b) =>
 a + b
let sum1 = num.reduce(sum)
console.log(sum1);

7.

var arr = [1, 2, 3, 6, 8, 6, 1, 9, 10, 12, 13];
var k = 3;
k = arr.length % k;
(function() {
 //arr = {};
 out = arr.slice(k + 1, arr.length);
 var count = out.length;
 for (var i = 0; i < k + 1; i++) {
 out[count] = arr[i];
 count += 1;
 }
 console.log(out);
    
})();

8.

var arr = ["guvi", "geek", "zen", "fullstack"];
(function() {
 for (var i = 0; i <arr.length; i++) {
 console.log(arr[i][0].toUpperCase() + arr[i].substr(1));
 }
})();

9.

var arr = [1, 2, 3, 5, 7, 79, 7, 2, 6, 9, 4];
(function() {
 for (var i = 0; i < arr.length; i++) {
 if (arr[i] % 2 !== 0) {
 console.log(arr[i]);
 }}
})();

10.
(function(str){
 str1 = str.split("").reverse().join("");
 console.log(str1); 
})("abcd")

11.
var res = function(arr){
     newArr = [];
 for(var i=0; i < arr.length; i++){
 if(newArr.indexOf(arr[i]) == -1) {
 newArr.push(arr[i]);
 } }
 console.log(newArr)
}
res(["guvi", "geek","guvi", "duplicate", "geeK"])

12.

var array =[
    [["firstname","Vasanth"],["lastname","Raja"],["age",24],["role","JSWizard"]],
    [["firstname","Sri"],["lastname","Devi"],["age",28],["role", "Coder"]]
    ];
var final=[]
while(array.length!==0)
{
 var outer_remove = array.shift();
 var new_object=[];
 while(outer_remove.length!==0)
 {
 var inner_remove = outer_remove.shift()
 var key = inner_remove[0]
 var value =inner_remove[1]
 new_object[key]=value
 }
 final.push(new_object)
}
console.log(final);
  //end-here
});

13.

var as=[12,34,5,6,2,56,6,2,1];
var s=as.reduce(function(a,c){
    //console.log(a,c);
 if(c%2!==0)
 {
 return a+c;
 }
 return a;},0);  
console.log(s);

14.
aa = data=>{
 var a=data;
  var l='';
for(i=0;i<a.length-1;i++){

 var s=a[i+1]
 var b=a[i]
 l+=s
 l+=b
 i=i+1
}
if((a.length%2)!==0){
 l+=a[a.length-1]
}
console.log(l);
}
aa("1234");

15.




