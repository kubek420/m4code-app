<script>
	let y;
	let topBtn;
	const tak = () => {
		if(y > 150){
			topBtn.style.bottom = "10px";
		} else {
			topBtn.style.bottom = "-100px";
		}
	}
</script>


<main>
	<nav>
		<img src="logom4.png" alt="">
		<div class="menuList">
			<a href="#main">M4CODE.PL</a>
			<a href="#oferta">Oferta</a>
			<a href="https://discord.gg/epYgNzyHbR" target="_blank">Discord</a>
			<a href="#kontakt">Kontakt</a>
		</div>
	</nav>
	<header id="main"><h1>M4CODE.PL</h1></header>
	<section id="oferta">
		<div class="card">
			<h1>Pakiet 1</h1>
			<ul>
				<li>- tickety</li>
				<li>- weryfikacja</li>
				<li>- powitania</li>
				<li><s>- antylink</s></li>
				<li><s>- komendy moderacyjne</s></li>
				<li><s>- konkursy</s></li>
				<li><s>- komendy 4fun</s></li>
				<li><s>- system propozycji</s></li>
			</ul>
			<h3>20zł/na zawsze</h3>
			<button
				data-sellix-product="62237047dda12"
				type="submit"
				alt="Buy Now with sellix.io"
				class="kup"
			>
				Zakup
			</button>
		</div>
		<div class="card">
			<h1>Pakiet 2</h1>
			<ul>
				<li>- tickety</li>
				<li>- weryfikacja</li>
				<li>- powitania</li>
				<li>- antylink</li>
				<li>- komendy moderacyjne</li>
				<li><s>- konkursy</s></li>
				<li><s>- komendy 4fun</s></li>
				<li><s>- system propozycji</s></li>
			</ul>
			<h3>30zł/na zawsze</h3>
			<button
				data-sellix-product="6223794f72a63"
				type="submit"
				alt="Buy Now with sellix.io"
				class="kup"
			>
				Zakup
			</button>
		</div>
		<div class="card">
			<h1>Pakiet 3</h1>
			<ul>
				<li>- tickety</li>
				<li>- weryfikacja</li>
				<li>- powitania</li>
				<li>- antylink</li>
				<li>- komendy moderacyjne</li>
				<li>- konkursy</li>
				<li>- komendy 4fun</li>
				<li>- system propozycji</li>
			</ul>
			<h3>40zł/na zawsze</h3>
			<button
				data-sellix-product="62237964d5357"
				type="submit"
				alt="Buy Now with sellix.io"
				class="kup"
			>
				Zakup
			</button>
		</div>
	</section>
	<footer id="kontakt">
		Dołącz na discord:&nbsp; <a href="https://discord.gg/epYgNzyHbR"> discord.gg/epYgNzyHbR</a>
	</footer>
	<button class="topBtn" bind:this={topBtn} on:click={() => {window.scrollTo(0, 0);}}><img src="arrow-up.svg" alt=""></button>
</main>

<svelte:window bind:scrollY={y} on:scroll={tak}/>

<style>
	footer{
		width: 100%;
		height: calc(2800px - 1200px - 800px);
		display: flex;
		justify-content: center;
		align-items: flex-end;
		padding: 30px;
		font-size: 30px;
		color:rgb(202, 202, 202);
	}
	section{
		width: 100%;
		height: 1200px;
		padding: 100px 200px;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.card h3{
		color:rgb(202, 202, 202);
		bottom: 35px;
		position: absolute;
	}
	.card ul{
		width: 80%;
		padding: 20px;
		font-size: 115%;
		color:rgb(202, 202, 202);
		list-style: none;
	}
	.card .kup{
		width: 150px;
		height: 50px;
		background-color: #fff;
		border-radius: 12px;
		color:#24252A;
		position: absolute;
		bottom: -25px;
		left: 0; right: 0;
		margin: auto;
		display: flex;
		align-items: center;
		justify-content: center;
		font-weight: bold;
		font-size: 24px;
		cursor: pointer;
	}

	section .card{
		width: 400px;
		height: 500px;
		background-color:#24252A;
		border-radius: 20px;
		position: relative;
		display: flex;
		padding: 20px;
		flex-direction: column;
		align-items: center;
	}
	.card h1{
		color: rgb(233, 233, 233);
		font-size: 40px;
		margin-top: 15px;
	}
	.topBtn{
		position: fixed;
		bottom: -100px;
		right: 10px;
		width: 50px;
		height: 50px;
		transition: .5s;
		background-color: #fff;
		border: 0;
		border-radius: 12px;
		-webkit-box-shadow: 0px 0px 25px -8px rgba(66, 68, 90, 0.5);
		-moz-box-shadow: 0px 0px 25px -8px rgba(66, 68, 90, 0.5);
		box-shadow: 0px 0px 25px -8px rgba(66, 68, 90, 0.5);
		cursor: pointer;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.topBtn img{
		height: 40px;
	}
	main {
		width: 100%;
		min-height: 2800px;
		display: flex;
		flex-direction: column;
	}
	header{
		width: 100%;
		height: 800px;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	header h1{
		color:#24252A;
		font-size: 80px;
	}
	nav{
		display: flex;
		width: 100%;
		height: 80px;
		justify-content: space-between;
		align-items: center;
		position: fixed;
		top: 0;
		left: 0;
		background-color: white;
		padding: 0 30px;
		-webkit-box-shadow: 0px 0px 25px -8px rgba(66, 68, 90, 0.5);
		-moz-box-shadow: 0px 0px 25px -8px rgba(66, 68, 90, 0.5);
		box-shadow: 0px 0px 25px -8px rgba(66, 68, 90, 0.5);
		z-index: 999;
	}
	nav img{
		height: 60px;
	}
	.menuList{
		display: flex;
		height: 80px;
		justify-content: space-between;
		align-items: center;
		width: 400px;
		font-size: 20px;
	}
	nav a{
		color: #24252A;
		transition: .5s;
	}
	nav a:hover{
		color: #39f;
		text-decoration: none;
	}
</style>