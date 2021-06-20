1. create your own resume data in JSON format
Answer - 
  var resume = { name: "NEHA SINHA", 
                 age:25 , 
                 email:"nehaassinha@gmail.com",
                 Mobile:"9611246412",
                 };

2. how to compare two JSON have the same properties without order?
        var obj1 = { name: "Person 1", age:5 };
        var obj2 = { age:5, name: "Person 1" };
Answer - 
    console.log(_.isEqual(obj1, obj2));
