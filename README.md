1. objectar nota references þannig ef þú býrð til einn object með einhvað value og býrð svo til annan object sem hefur sama value-ið þá ertu enðá bara með eitt value, þeir kalla bara báðir á það, ef maður breytir value-inu í einum object þá breytir það líka því í hinum.

2. lína 1 býr til fall að nafni book sem tekur við breytu 
   lína 2 gefur fallinu varible þar sem this(fallið Book).isbn hefur sama value og breytan sem fallið tekur við.
   lína 3 býr til fall sem notar fallið book sem parent og nær í breytuna sem skilgreind var í því falli.
   lína 4 þegar kallað er á Book.getIsbn þá fær maður return value sem sýnir okkur isbin breytuna sem skilgreind var í fyrsta fallinu.
   lína 5 notar fallið Book og býr til book að nafni bookObject sem hefur isbn-in 12345

3.	
	function spaceship(n, s, l) {
		this.name = n,
		this.speed = s,
		this.life = l
	};

	let f1 = new spaceship("David", 300, 100);
	let f2 = new spaceship("Harold", 500, 70);
	let f3 = new spaceship("Jess", 700, 50);

	spaceship.prototype.fly = function(){
		this.speed += 1;
	};

	f1.prototype.setLife = function(){
		this.life += 1;
	};

prototype geymir allar uplisýsingar um parent fallsins eða objectsins

5. 
