<header>
	<nav>
		<h1>BRUIN</h1>
		<ul>
			<li><a href="#home">Home</a></li>
			<li><a href="#Work">Work</a></li>
			<li><a href="#contact">Contact</a></li>
			<li><a href="#src/routes/+about.sveltet">About</a></li>
		</ul>
	</nav>
</header>

<div class="loader" />

<h1 class="anouk">ANOUK</h1>
<h1 class="bruin">BRUIN</h1>

<div class="pictures">
	<img class="photo-1" src="/src/assets/profile-picture.JPG" alt="profilepicture" />
</div>

<section class="my-story">


<div class="about">
	

	<div class="information-story">
		<h2 class="about-me">22</h2>
		
	</div>
	<p class="story">
		I'm Anouk, a frontend developer student at HvA College. Right now I'm in my last year.
		I'm 22 years old and i live in Castricum. I work in a restaurant at a retirement home
	</p>
</div>
</section>

<section class="slider">

<div class="slide"> 
	
	<div class="img1"><img class="minnie1" src="src/assets/minnie.jpeg" alt="minnie"></div>
	<div class="img2"><img class="ski" src="src/assets/ski.png" alt="ski"></div>
	<div class="img3"><img class="minnie1" src="src/assets/minnie.jpeg" alt="minnie"></div>

</div>

</section>
<body />

<!--  <-----------------------------------------------STYLING-------------------------------------------------------------- >  -->

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	body {
		background-color: rgb(33, 33, 33);
	}

	.loader {
		position: relative;
		width: 100%;
		height: 4px;
		background: #000;
		border-radius: 10px;
		justify-content: center;
	}

	/* <--------------- ANIMATIE BALK START ---------------> */
	.loader::before {
		content: '';
		position: absolute;
		width: 100%;
		height: 100%;
		background: white;
		transform-origin: left;
		animation: slider 8s linear infinite;
	}

	@keyframes slider {
		0%,
		20% {
			transform: scaleX(0);
		}
		40% {
			transform: scaleX(1);
			transform-origin: left;
		}
		40.000001% {
			transform: scaleX(1);
			transform-origin: right;
		}
		80%,
		100% {
			transform: scaleX(0);
			transform-origin: right;
		}
	}

	/* <--------------- ANIMATIE BALK EINDE ---------------> */

	/* ---profile--- */

	p {
		font-family: Avenir;
		font-size: 25px;
		
	}

	p.story {
		margin-left: 35em;
		width: 20em;
		margin-top: -55em;
	}

	section.my-story {
		width: 100%;
		height: 100%;
		padding: 1em 1em 0;
		border-radius: 1em;
	}
	.information-story {
		margin-bottom: 2em;
		background-image: url(/src/assets/background.jpg);
		border-radius: 20px;
		width: 100%;
		height: 100%;
	
	}

	
	.story {
		text-align: left;
		margin-right: 0.2em;

		
	}
	H1.anouk {
		font-size: 370px;
		float: left;
		display: inline;
		margin-left: 50px;
		margin-top: -20px;
	}

	h1.bruin {
		font-size: 370px;
		float: right;
		display: inline;

		margin-right: 50px;
	}

	img.photo-1 {
		width: 400px;
		margin-left: 100px;
		border-radius: 90px;
		height: auto;
		box-shadow: 20px;
		border-color: white;
		margin-bottom: 50px;
	}

	.about-me {
		color: rgb(182, 182, 182);
		text-align: left;
		margin-bottom: 2em;
		font-size: 30em;
		font-family: avenir;
		padding-top: 3rem;
		margin-left: 0.1em;
	}

	.about {
		text-align: right;
		border-radius: 20px;
		width: 100%;
		height: 100%;
		padding: 1em 1em 0;
		border-radius: 1em;
	}

	/* PICTURES */

	section.cats {
		border-radius: 20px;
		width: 100%;
		height: 100%;
		padding: 1em 1em 0;
		border-radius: 1em;
	}

	img.minnie1 {
		margin-top: 17em;
		width: 100%;
		height: 100%;
		padding: 1em 1em 0;
		border-radius: 2em;
	}

	img.ski {
		/* margin-top: 17em; */
		width: 100%;
		height: 100%;
		padding: 1em 1em 0;
		border-radius: 2em;
	}

	/* ---NAVBAR--- */

	h1 {
		color: white;
		font-family: kirang haerang;
		font-size: 40px;
		margin-left: 12px;
		display: inline;
		outline: 0;
	}

	a {
		color: rgb(33, 33, 33);
		font-size: 24px;
		font-family: apercu;
	}

	ul {
		list-style-type: none;
		margin: 0;
		padding: 0;
		display: inline;
	}

	li {
		display: inline;
		float: right;
		padding: 8px;
	}

	/* <-----------------ANIMATIE SLIDEINLEFT START ----------------> */

	@keyframes slideinleft {
		from {
			transform: translateX(-300px);
		}
		to {
			transform: translateY(0);
		}
	}

	H1.anouk {
		animation-name: slideinleft;
		animation-duration: 0.5s;
		animation-timing-function: ease-in;
		animation-delay: 0s;
		animation-iteration-count: 1;
		animation-direction: normal;
		animation-fill-mode: none;

		transform: translateX((-150px));
	}

	h1.bruin {
		animation-name: slideinleft;
		animation-duration: 0.5s;
		animation-timing-function: ease-in;
		animation-delay: 0s;
		animation-iteration-count: 1;
		animation-direction: normal;
		animation-fill-mode: none;

		transform: translateX((-150px));
	}
</style>
