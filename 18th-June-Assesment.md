1. create your own resume data in JSON format
Answer - 
  	var resume ={ name: "NEHA SINHA", 
			   age:25 , 
			   email:"nehaassinha@gmail.com", 
			   mobile:"9611246412", 
			   address:{{"Om Sai ram PG for Girl"}{"6th Cross, Bellandur"}{"Bangalore -560102, Karnataka"}},
			   objective:"To work with an organization where I can continuously learn in pursuit of achieving functional excellence which will enable me to apply my thoughts and continuously learn, create, innovate and simultaneously contribute towards the growth of organization with the best of my capabilities.",
			  profileSummary:
					{
						{"2.0+ Years of experience in the IT industry in Software Development using Java, J2EE, Spring MVC, Collection Framework, SAP Hybris Commerce with Cargill projects."}
						{"Good Exposure to complete SDLC."}
						{"Experience in Agile Scrum Methodology."}
						{"Knowledge in Core Java, J2EE, Spring MVC, SAP Hybris Commerce."}
						{Good knowledge in RDBMS concepts Oracle (PL/SQL).}
					},
			  softwareSkills:
					{
						{"Languages: C, C++, Core Java, J2EE, PL/SQL, Spring MVC, Hibernate, Collection Framework, Data Structure."}
						{"Database: Oracle (PL/SQL)"}
						{"Operating System: Windows"}
					},
			   professionalExperience:"Working with Accenture (ACC), Bengaluru as a Software Developer from November 2017- till Now.",
			   educationalQualification:"M.C.A (Master of Computer Application)",
			};

2. how to compare two JSON have the same properties without order?
        var obj1 = { name: "Person 1", age:5 };
        var obj2 = { age:5, name: "Person 1" };
Answer - 
    console.log(_.isEqual(obj1, obj2));
