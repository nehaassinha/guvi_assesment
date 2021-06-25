    Q1. https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md
    Solution:-
    a.
    class Movie {
     constructor(title, studio, rating) {
     this.title = title;
     this.studio = studio;
     this.rating = rating;
     }
    }
    var movie=new Movie("ABCD2","BALAJI","4.5");
    console.log(movie)
  
    b.
    class Movie{
     constructor(title, studio, rating='PG') {
     this.title = title;
     this.studio = studio;
     this.rating = rating;
     }
    }
    var movie=new Movie("ABCD2","BALAJI");
    console.log(movie)
    
    c.
    class Movie{
     constructor(title, studio, rating='PG') {
     this.title = title;
     this.studio = studio;
     this.rating = rating;
     }
     getPG(arr_movie){
         let arr_mv=[];let c=0;
         //let arr_mv = arr_movie.filter(car => arr_movie.rating === "PG");
         for(let i=0;i<arr_movie.length;i++){
             if(arr_movie[i].rating==='PG'){
                 arr_mv[c++]=arr_movie[i];
             }
         }
         return arr_mv;
     }
    }
    var mv=[new Movie("ABCD2","BALAJI1","qwer"),
        new Movie("ABCD","BALAJI"),
        new Movie("ABCD3","Alt","4.5"),
        new Movie("DDLG","BALAJI3","PG")
    ]
    console.log(new Movie().getPG(mv));
    
    d. 
    new Movie("Casino Royale","Eon Productions","PG13")
    //console.log(new Movie("Casino Royale","Eon Productions","PG13"));
    
    Q2. https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md
    Solution:-
    class Circle{
      radius=1.0;
      color='red';
      //constructor(){}
     // constructor(radius){this.radius=radius}
      constructor(radius=1.0, color='red') {
       this.radius = radius;
       this.color = color;
      }
      getRadius(){ return this.radius;}
      setRadius(radius){ this.radius;}
      getColor(){ return this.color;}
      setColor(color){ this.radius;}
      toString(){return (this.radius+" "+this.color);}
      getArea()
        {
              return +(2*(22/7)*(this.radius)*(this.radius));
        }
      getCircumference(){return 2*22/7*this.radius;}
      
    }
    var circle=new Circle(2,'orange');
    console.log(circle);
    console.log(circle.radius, circle.color);
    console.log(circle.getArea());
    console.log(circle.getCircumference());
    console.log(circle.getRadius());
    console.log(circle.getColor());
    console.log(circle.toString());
    
    3.
    Write a person class to hold all details.
    instances. The returned array need not be full.
    class Person {
    constructor(fname='unknown',lname='unkonwn',age=0) 
    {
        this.fname = fname;
        this.lname = lname;
        this.age = age;
    }
    getFname(){return this.fname}
    setFname(fname){this.fname=fname;}
    getLname(){return this.lname}
    setLname(lname){this.lname=lname;}
    getAge(){return this.age}
    setAge(age){this.age=age;}
    toString(){return this.fname+" "+this.lname+" Age :"+this.age;}
    }
     var p = new Person("Neha","Sinha",25);
    console.log(p);
    console.log(p.getFname());
    console.log(p.getLname());
    console.log(p.getAge());
    console.log(p.toString());
    p.setAge(10);
    console.log(p.getAge());
    
    
    4. write a class to calculate uber price.
    Solution-
    class Uber {
    constructor(distance=0,price_p_km=99.89) 
    {
        this.distance = distance;
        this.price_p_km = price_p_km;
    }
    getDistance(){return this.distance}
    setDistance(distance){this.distance=distance;}
    getRate_p_km(){return this.price_p_km}
    setRate_p_km(price_p_km){this.price_p_km=price_p_km;}
    getPrice(){
        return this.distance*this.price_p_km;
    }
    }
    var p = new Uber(10);
    console.log(p);
    console.log(p.getDistance());
    console.log(p.getRate_p_km());
    console.log(p.getPrice());
    
    4) write a class to calculate uber price.
    class Calculator{
    constructor(x=0,y=0){
        this.x=x;
        this.y=y;
    }
    add(){
        return this.x+this.y;
    }
    sub(){
        return this.x-this.y;
    }
    mul(){
        return this.x*this.y;
    }
    div(){
        return this.x/this.y;
    }
    }
    var cal=new Calculator(4,5);
    console.log(cal.add(),cal.sub(),cal.mul(),cal.div())
    
