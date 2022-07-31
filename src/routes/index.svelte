<script>
	import { slide } from 'svelte/transition';

	const dashboard = [
		{ label: 'Home', href: '/' },
		{ label: 'About', href: 'about' },
		{ label: 'Gallery', href: 'gallery' },
		{ label: 'Contact', href: 'contact' }
	]

	let openToggle = false;
</script>

<header>
	<nav class="navbar">
		<div class="icon">
			<img src="img/IconLogo.svg" alt="" />
		</div>
		<div class="ToggleMenu">
			<div class="menus" on:click={() => (openToggle = !openToggle)} class:change={openToggle} >
				<img src="img/IconBurgers.svg" alt="" />
			</div>
			<div class="sideToggle" class:open={openToggle} >
				<!-- <a href="#a" class="closebtn" on:click={() => (openToggle = !openToggle)}>&times;</a> -->
				<ul>
					{#each dashboard as db}
						<li>
							<a href={db.href}>{db.label}</a>
						</li>
					{/each}
				</ul>
			</div>
		</div>
		
	</nav>
</header>
<section class="topContainer">
	<div class="topContent">
		<div class="leftTop">
			<h1>Scale Fintech</h1>
			<h2>Safe And Secure</h2>
			<p>
				Ship your fintech products to your customers with fast and reliable processes. Secure and
				highly customizable. Rise Finance is the best partner for you if you want to scale your
				finance products worldwide.
			</p>
			<button class="btnTop">Consultation</button>
		</div>
		<div class="rightTop">
			<img class="imgBig" src="img/cardbig.svg" alt="" />
			<img class="imgSm" src="img/cardsm.svg" alt="" />
		</div>
	</div>
	<div class="logoIpsum">
		<img src="logo/logoIpsum1.svg" alt="" />
		<img src="logo/logoIpsum2.svg" alt="" />
		<img src="logo/logoIpsum3.svg" alt="" />
		<img src="logo/logoIpsum4.svg" alt="" />
	</div>
</section>

<section class="middleOneContainer">
	<h1 class="oneHeader">consulting for startups in fintech</h1>
	<p class="oneTxt">
		Our Team consists of proven experts from finance, tech and science. This mix makes it possible
		for our team to deliver the best results to all our clients.
	</p>
	<img src="img/screenmiddle.svg" alt="" />
</section>

<section class="middleTwoContainer">
	<h1 class="midTwoHeader">Delivering value in every step of production</h1>
	<div class="midTwoContent">
		<div class="midTwoImg">
			<img src="img/midImg.svg" alt="" />
		</div>
		<div class="midTwoContext">
			<p class="title">The Process</p>
			<p class="subtitle">
				Strategic phrases we run through with every client make it possible to implement highly
				efficinet processes, even in high pace startups that like to scale as fast as possible.
			</p>
			<div class="midCard">
				<div class="cardContent">
					<img src="/img/analytic.svg" alt="" />
					<p class="cardTxt">Analysis</p>
					<h1 class="cardHeader">1</h1>
				</div>
				<div class="cardContent">
					<img src="/img/growth.svg" alt="" />
					<p class="cardTxt">Growth Phase</p>
					<h1 class="cardHeader">2</h1>
				</div>
				<div class="cardContent">
					<img src="/img/profit.svg" alt="" />
					<p class="cardTxt">Profit</p>
					<h1 class="cardHeader">3</h1>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="middleThreeContainer">
	<h1 class="ThreeHeader">Case Study</h1>
	<p class="txtMiddleTri">Some results from our clients</p>
	<div class="midThreeContext">
		<div class="threeCard">
			<div class="contentTri">
				<h2 class="titleTri">Coruma Finance</h2>
				<p class="txtTri">
					Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
					invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
				</p>
				<button class="btnMidTri">read more about this client</button>
			</div>
			<div class="imgTri">
				<img src="/logo/triLogo.svg" alt="" />
				<img class="phoneTri" src="/img/phoneScreen.svg" alt="" />
				<div class="phoneCard1">
					<p class="phoneCardTxt">Accquired 8 long time customers</p>
				</div>
				<div class="phoneCard2">
					<p class="phoneCardTxt">300% Growth in first year</p>
				</div>
				<div class="phoneCard3">
					<p class="phoneCardTxt">hired 24 talented developers</p>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="middleFourContainer">
	<h1 class="fourTitle">Coruma Finance</h1>
	<p class="fourSubtitle">
		Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt
		ut labore et dolore magna aliquyam erat, sed diam voluptua.
	</p>
	<div class="fourImg">
		<img src="/img/imac.svg" alt="" />
		<div class="imacCard1">
			<p class="phoneCardTxt">Accquired 8 long time customers</p>
		</div>
		<div class="imacCard2">
			<p class="phoneCardTxt">300% Growth in first year</p>
		</div>
		<div class="imacCard3">
			<p class="phoneCardTxt">hired 24 talented developers</p>
		</div>
	</div>
</section>

<footer>
	<div class="footerContainer">
		<div class="icon">
			<img src="logo/logoFooter.svg" alt="" />
		</div>
		<div class="footerList">
			<div class="footerContent">
				<div class="services">
					<ul>
						Services
						<li>Web Hosting</li>
						<li>Domains</li>
						<li>Premium Hosting</li>
						<li>Private Server</li>
						<li>E-mail Hosting</li>
					</ul>
				</div>
				<div class="supports">
					<ul>
						Support
						<li>Pricing Plan</li>
						<li>Documentation</li>
						<li>Guide</li>
						<li>Tutorial</li>
					</ul>
				</div>
				<div class="companies">
					<ul>
						Company
						<li>About</li>
						<li>Blog</li>
						<li>Join Us</li>
						<li>Press</li>
						<li>Partners</li>
					</ul>
				</div>
				<div class="legals">
					<ul>
						Legal
						<li>Claim</li>
						<li>Privacy</li>
						<li>Terms</li>
					</ul>
				</div>
			</div>

			<div class="footerSubs">
				<div>
					<ul>
						Subcribe to our newsletter
						<li>Funding freemium long tail hypotheses first mover advantage assets ownership</li>
					</ul>
				</div>
			</div>
		</div>
		<p class="footerText">Design with love © TanahAirStudio 2020. All right reserved</p>
	</div>
</footer>

<style>
	header {
		max-width: 100%;
	}

	.navbar {
		position: fixed;
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 20px 50px;
		z-index: 50;
		background: linear-gradient(177.23deg, #423ee0 -13.49%, #812de2 109.75%);
	}

	.icon {
		cursor: pointer;
		width: 100%;
	}

	.ToggleMenu {
		/* background-color: blue; */
		position: relative;
		width: 100%;
		cursor: pointer;
		margin: auto;
		display: flex;
		align-items: center;
		box-sizing: border-box;
	}

	.menus {
		width: 100%;
		display: flex;
		justify-content: end
	}

	

	.sideToggle {
		position: fixed;
		top: 85px;
		right: 0;
		width: 0;
		/* padding: 10px; */
		border-radius: 20px;
		background: linear-gradient(177.23deg, #423ee0 -13.49%, #812de2 109.75%);
		transition: top 2000ms ease-in-out;
	}

	.sideToggle ul {
		text-align: center;
	}

	.sideToggle a {
		color: white;
		text-decoration: none;
	}

	.closebtn {
		position: absolute;
	}

	.open {
			width: 10%;
		}

	.topContainer {
		position: relative;
		width: 100%;
		padding: 200px 50px;
	}

	.topContainer::before {
		content: '';
		z-index: -1;
		width: 509px;
		height: 509px;
		border-radius: 50%;
		position: absolute;
		/* top: 0; */
		/* right: 0; */
		bottom: -150px;
		left: -120px;
		background: linear-gradient(177.23deg, #423ee0 -13.49%, #812de2 109.75%);
		filter: blur(100px);
		opacity: 0.2;
		transition: opacity 0.3s;
	}

	.topContainer::after {
		content: '';
		z-index: -1;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: inherit;
	}

	.topContent::before {
		content: '';
		z-index: -1;
		width: 350px;
		height: 350px;
		border-top-left-radius: 50%;
		border-bottom-left-radius: 50%;
		position: absolute;
		top: -100px;
		right: 0px;
		/* bottom: -200px;
		left: -150px; */
		background: linear-gradient(177.23deg, #423ee0 -13.49%, #812de2 109.75%);
		filter: blur(100px);
		opacity: 0.2;
		transition: opacity 0.3s;
	}

	.topContent::after {
		content: '';
		z-index: -1;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: inherit;
	}

	.topContent {
		width: 100%;
		display: flex;
		justify-content: space-between;
		/* align-items: center; */
	}

	.leftTop {
		padding-top: 100px;
		width: 100%;
	}

	.leftTop h1 {
		font-size: 90px;
		line-height: 99px;
	}

	.leftTop h2 {
		font-size: 82px;
		line-height: 90px;
	}

	.leftTop p {
		margin-top: 20px;
		font-size: 21px;
		line-height: 28.6px;
	}

	.btnTop {
		text-transform: uppercase;
		margin-top: 20px;
		border-width: 4px;
		background: transparent;
		color: var(--pure-white);
		font-size: 18px;
		font-weight: 600;
		padding: 10px;
		width: 274px;
		border-style: solid;
		border-image: linear-gradient(to right, #812de2, #3a49f9) 1;
		cursor: pointer;
		opacity: 0.7;
		transition: 0.5s;
	}

	.btnTop:hover {
		opacity: 1;
	}

	.rightTop {
		width: 100%;
		position: relative;
	}

	.imgBig {
		width: 100%;
	}

	.imgSm {
		position: absolute;
		top: 220px;
		right: 50px;
	}

	.logoIpsum {
		width: 100%;
		display: flex;
		justify-content: space-around;
		margin-top: 50px;
		/* padding: 20px 100px; */
	}

	.middleOneContainer {
		width: 100%;
		display: flex;
		flex-direction: column;
		padding: 50px;
		background-color: var(--pure-white);
		align-items: center;
		justify-content: center;
	}

	.oneHeader, .midTwoHeader, .ThreeHeader, .fourTitle {
		font-size: 50px;
		line-height: 70px;
		font-weight: 600;
		text-transform: capitalize;
		width: 100%;
		text-align: center;
		padding: 1rem 20rem;
	}

	.oneTxt {
		color: var(--black);
		width: 60%;
		padding: 50px 150px 0px 150px;
		font-size: 22px;
		line-height: 28.6px;
		font-weight: 500;
		text-align: center;
		/* text */
		/* margin-top: 50px; */
	}

	.middleOneContainer img {
		width: 80%;
	}

	.middleTwoContainer {
		position: relative;
		width: 100%;
		padding: 50px 50px 150px 50px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.middleTwoContainer::before {
		content: '';
		z-index: -1;
		width: 459px;
		height: 459px;
		/* border-radius: 50%; */
		border-top-left-radius: 30%;
		border-bottom-left-radius: 80%;
		position: absolute;
		top: 0;
		right: 0;
		/* bottom: -200px;
		left: -150px; */
		background: linear-gradient(177.23deg, #423ee0 -13.49%, #812de2 109.75%);
		filter: blur(100px);
		opacity: 0.3;
		transition: opacity 0.3s;
	}

	.middleTwoContainer::after {
		content: '';
		z-index: -1;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: inherit;
	}


	.midTwoContent {
		width: 100%;
		margin-top: 100px;
		display: flex;
		/* justify-content: space-evenly; */
	}

	.midTwoImg {
		width: 40%;
		padding-left: 50px;
		position: relative;
		/* box-shadow: inset 0 0 12px 12px linear-gradient(177.23deg, #423EE0 -13.49%, #812DE2 109.75%), inset 0 0 3px 2px linear-gradient(177.23deg, #423EE0 -13.49%, #812DE2 109.75%); */
	}

	

	.midTwoImg img {
		width: 70%;
	}

	.midTwoImg::before {
		content: '';
		z-index: -1;
		width: 80%;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: linear-gradient(177.23deg, #423ee0 -13.49%, #812de2 109.75%);
		filter: blur(20px);
		opacity: 0.5;
		transition: opacity 0.3s;
	}

	.midTwoImg::after {
		content: '';
		z-index: -1;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: inherit;
	}

	.midTwoContext {
		width: 60%;
		/* margin-top: 50px; */
		padding: 50px 110px;
	}

	.title {
		font-size: 30px;
		line-height: 30px;
		font-weight: 600;
		margin-bottom: 50px;
	}

	.subtitle {
		font-size: 22px;
		line-height: 28.6px;
		width: 100%;
	}

	.midCard {
		position: relative;
		width: 100%;
		display: flex;
		justify-content: space-between;
		margin-top: 80px;
	}

	.cardContent {
		padding: 2px;
		margin: 0;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 150px;
		height: 138px;
		border: solid 1px transparent;
		border-radius: 30px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
	}

	.cardTxt {
		margin-top: 15px;
		text-align: center;
	}

	.cardHeader {
		position: absolute;
		top: 100px;
		font-size: 90px;
		font-weight: 500;
		line-height: 117px;
	}

	.middleThreeContainer {
		position: relative;
		width: 100%;
		display: flex;
		flex-direction: column;
		padding: 80px 50px;
		background-color: var(--pure-white);
		align-items: center;
		justify-content: center;
	}

	

	.txtMiddleTri {
		color: var(--black);
		width: 50%;
		padding: 50px 150px 0px 150px;
		font-size: 22px;
		line-height: 28.6px;
		font-weight: 500;
		text-align: center;
		/* text */
		/* margin-top: 50px; */
	}

	.midThreeContext {
		width: 100%;
		padding-top: 50px;
	}

	.threeCard {
		position: relative;
		display: flex;
		align-items: center;
		width: 60%;
		height: 817px;
		border-radius: 10px;
		border: 1px solid #15123e;
		background-color: #15123e;
		padding: 50px;
	}

	.titleTri {
		width: 100%;
		font-size: 30px;
		line-height: 30px;
		font-weight: 600;
		margin-bottom: 50px;
	}

	.txtTri {
		width: 100%;
		/* padding: 0px 100px 0px 0px; */
		font-size: 22px;
		line-height: 28.6px;
		letter-spacing: 2px;
	}

	.imgTri {
		position: relative;
		width: 40%;
		padding: 50px 150px 50px 0px;
	}

	.btnMidTri {
		text-transform: uppercase;
		margin-top: 20px;
		border-width: 4px;
		background: transparent;
		color: var(--pure-white);
		font-size: 18px;
		font-weight: 600;
		padding: 20px;
		width: 80%;
		border-style: solid;
		border-image: linear-gradient(to right, #812de2, #3a49f9) 1;
		transition: 0.5s;
		opacity: 0.6;
		cursor: pointer;
	}

	.btnMidTri:hover {
		opacity: 1;
	}

	.phoneTri {
		position: absolute;
		top: 120px;
		right: -250px;
		z-index: 1;
	}

	.phoneCard1 {
		position: absolute;
		top: 200px;
		right: -550px;
		/* z-index: -1; */
		border: solid 3px transparent;
		border-radius: 10px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
		height: 80px;
		width: 320px;
	}

	.phoneCard2 {
		position: absolute;
		top: 365px;
		right: -550px;
		/* z-index: -1; */
		border: solid 3px transparent;
		border-radius: 10px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
		height: 80px;
		width: 320px;
	}

	.phoneCard3 {
		position: absolute;
		top: 525px;
		right: -550px;
		/* z-index: -1; */
		border: solid 3px transparent;
		border-radius: 10px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
		height: 80px;
		width: 320px;
	}

	.phoneCardTxt {
		text-align: center;
		margin-top: 25px;
	}

	.threeCard::before {
		content: '';
		z-index: 0;
		width: 600px;
		height: 600px;
		border-top-right-radius: 50%;
		border-bottom-right-radius: 50%;
		position: absolute;
		/* top: 0;
		right: 0; */
		bottom: 0;
		left: 0;
		background: linear-gradient(177.23deg, #423EE0 -13.49%, #812DE2 109.75%);
		filter: blur(100px);
		opacity: 0.3;
		transition: opacity 0.3s;
	}

	.middleThreeContainer::before {
		content: '';
		z-index: 1;
		width: 500px;
		height: 500px;
		border-top-left-radius: 50%;
		border-bottom-left-radius: 50%;
		position: absolute;
		/* top: 0; */
		right: 0;
		bottom: -250px;
		/* left: 0; */
		background: linear-gradient(177.23deg, rgba(66, 62, 224, 0.71) -13.49%, #4829A5 109.75%);
		filter: blur(100px);
		opacity: 0.5;
		transition: opacity 0.3s;
	}

	.middleThreeContainer::after {
		content: '';
		z-index: -1;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: inherit;
	}

	.middleFourContainer {
		position: relative;
		background-color: #15123e;
		width: 100%;
		padding: 50px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.middleFourContainer::before {
		content: '';
		z-index: 0;
		width: 800px;
		height: 800px;
		border-radius: 50%;
		position: absolute;
		/* top: 0;
		right: 0; */
		bottom: -100px;
		left: -200px;
		background: linear-gradient(177.23deg, #423EE0 -13.49%, #812DE2 109.75%);
		filter: blur(100px);
		opacity: 0.2;
		transition: opacity 0.3s;
	}

	/* .middleFourContainer::after {
		content: '';
		z-index: -1;
		position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		background: inherit;
	} */



	

	.fourSubtitle {
		font-size: 22px;
		line-height: 28.6px;
		text-align: center;
		width: 60%;
	}

	.fourImg {
		position: relative;
		margin-top: 50px;
		display: flex;
		justify-content: center;
		width: 100%;
	}

	.imacCard1 {
		position: absolute;
		top: 0;
		right: 250px;
		/* z-index: -1; */
		border: solid 1px transparent;
		border-radius: 10px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
		height: 80px;
		width: 320px;
	}

	.imacCard2 {
		position: absolute;
		top: 170px;
		left: 212px;
		/* z-index: -1; */
		border: solid 1px transparent;
		border-radius: 10px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
		height: 80px;
		width: 320px;
	}

	.imacCard3 {
		position: absolute;
		top: 360px;
		right: 250px;
		/* z-index: -1; */
		border: solid 1px transparent;
		border-radius: 10px;
		background-image: linear-gradient(#1c1a50, #1c1a50),
			linear-gradient(94.28deg, #812de2 0%, #3a49f9 100%);
		background-origin: border-box;
		background-clip: content-box, border-box;
		height: 80px;
		width: 320px;
	}

	footer {
		max-width: 100%;
		background: #121139;
	
		z-index: 1;
	}

	.footerContainer {
		width: 100%;
		display: flex;
		flex-direction: column;
		padding: 100px 150px;
	}

	.footerList {
		display: flex;
		margin-top: 20px;
		/* justify-content: space-between; */
		width: 100%;
		padding-bottom: 50px;
		border-bottom: 2px solid #71777d;
	}

	.footerContent {
		width: 60%;
		display: flex;
		justify-content: space-between;
	}

	.footerSubs {
		width: 40%;
		margin-left: 200px;
	}

	ul {
		color: #92989f;
		font-size: 18px;
		line-height: 24px;
		font-weight: 600;
	}

	li {
		margin-top: 10px;
		color: #ffffff;
		list-style: none;
		font-weight: 400;
		cursor: pointer;
	}

	li:hover {
		text-decoration: underline;
	}

	.footerText {
		text-align: center;
		font-size: 12px;
		color: #92989f;
		margin-top: 20px;
	}
</style>
