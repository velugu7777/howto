###How to declare variables
	 var i;
	 var sum;
###Variable scope
	*variable declare outside the function body thant can use any ware in page
	*variable declare inside the function body that is private
###Data types
	String
	Numbers
	Date
	Null
	Undefined
	Booleans
###How to declare Strings
	var myName = "anji";
###How to Assign Numbers
```js
   var a = 19;
	var b = 20;
```
###How to declare Booleans
	status:true/false
##How to declare Arrays
```js
	var myArray = [];
	var scores = ["20","30","40","50"];
```
###How to find arrays length
```js
		var colors = ["green","white","red","yellow"];
		var len = colors.length;
		colors[1]; //It output dispalys white
```
		Notes
			fisrt declare variable colors name
			find array length
			displays output(white)
###How to use toString()
```js
				var colors = ["green","white","red","yellow"];
				var k = colors.toString();
				colors.toString(); //	It dispalys output  green , white,red,yellow
```
###How to use slice()
```js
					var numbers =[1,2,3,4,5];
					numbers.slice(2);
					// output displays start from [3,4,5]
```
###How to use push()
```js
				var colors = ["red","white"];
				colors.push("green","blue"); // adding two other colors
				//output dispalys [red,white,green,blue]
```
###how to splice()
				var colors = ["red","white","blue","green"];
				var del = colors.splice(0,1);	 					
###Operators
	operators there types
	1.Arthamatic
		=,+,-,*,/,%
	2.Logical
		AND &&
		OR ||
		NOT !
##Decision Making -The if and switch statements
###if Statement
```js
	if (a > b){
	//write the code here
	}
```
	//(a>b)....this test conditon
	// if .. test condtion true then excuete
	//	 all the code inside curyly braces
###else Statement
```js
	if (myAge > 0 && myAge < 30){
		console.log("myAge is between 0 and 30");
	} else {
		console.log("myAge is not between 0 and 30");
	}
```
###else if statement
```js
	if (a - b){
		//some code here
		} else if(b - c){
			// some code here
	}
```
### switch Statement
	switch statement has four important elements
	1.The test experssion
	2.The case statements
	3.The break statements
	4.The default statement
```js
	switch (myName)
	case "anji":
		//some code
		break;
	case "velugu":
		// some other code
		break;
	default:
		// default code
		break;
```
##Looping -The for And while Statements
##for Statement
```js
	for (i =0; i < 10; i++){
		console.log("i");
	}
```
	1.initialize i to 0;
	2.check each time that i less than 10;
	3.increment i for each loop after the first
##while statement
```js
	while(i ! = 10){
		// some code here
	}
```
		condition - keep looping while this condition
						is till true
##do while staement
```js
	do{
		// some code here

	}
	while(tset condtion);
```
###How to create functions
	function calc(){
		// write some code here
	}
###How to call functions
```js
	function calc(){
		//some code here
	}
		var k = calc();
		console.log(k);
```
##Objects
###How to create objects
```js
	var person = {
			name: "anji",
			age: 25,
			job: "software",
			sayName: function(){
				console.log(this.name);
		 }
	};
```

   1.This example creates an object called person
		that has three properties (name, age and job)and
		one method that is sayName(); this method dispaly value of this.name
	2.here the property called name is created and value of "anji" is assigned
###constructor Object pattern
```js
	fubction Person ("name,age,job"){
	this.name = name;
	this.age = age;
	this.job = job;
	this.sayName = function(){
		console.log(this.name);
	  };
	  }

		var person1 = new person("anji","25","software");
		var person2 = new person("velugu","25",software);
```
###The prototype
	Each function is created with a prototype property,
	which is an object containing properties and methods.
```js
		function Person(){
		}
			Person.prototype.name = "anji";
			Person.prototype.age = 25;
			Person.prototype.job = "software";
			person.prototype.sayName =function() {
			console.log(this.name);
		};
			var person1 = new Person();
			person1.sayName();
```
###Alternative syntax
```js
	function Person(){
	}
	Person.prototype ={
	name : "anji",
	age : 25,
	job : "software",
	sayName : function(){
		console.log(this.name);
	 }
	};
```
