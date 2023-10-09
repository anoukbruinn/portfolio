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

<div class="about">
	<div class="information">
		<h2 class="about-me">About me</h2>
	</div>

	<div class="information-story">
		<p class="story">
			I'm Anouk, a frontend developer student at <br /> HvA College. Right now I'm in my last year.
			I'm 22 years old <br /> and i live in Castricum. I work in a restaurant at a retirement home
		</p>
	</div>
</div>

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
		color: black;
		text-align: center;
		margin-bottom: 1em;
		font-size: 50px;
		font-family: avenir;
		padding-top: 3rem;
	}

	.about {
		text-align: center;
		padding-left: 50px;
		background-color: rgb(245, 239, 239);
		border-radius: 20px;
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
