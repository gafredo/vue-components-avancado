<template>
	<section>
		<h2>Falling Snowflake</h2>
		<div class="set">
			<div><img src="../assets/floco1.png" alt="1" /></div>
			<div><img src="../assets/floco2.png" alt="2" /></div>
			<div><img src="../assets/floco3.png" alt="3" /></div>
			<div><img src="../assets/floco4.png" alt="4" /></div>
			<div><img src="../assets/floco1.png" alt="5" /></div>
			<div><img src="../assets/floco2.png" alt="6" /></div>
			<div><img src="../assets/floco3.png" alt="7" /></div>
			<div><img src="../assets/floco4.png" alt="8" /></div>
			<div><img src="../assets/floco1.png" alt="9" /></div>
			<div><img src="../assets/floco2.png" alt="10" /></div>
			<div><img src="../assets/floco3.png" alt="11" /></div>
			<div><img src="../assets/floco4.png" alt="12" /></div>
			<div><img src="../assets/floco1.png" alt="13" /></div>
			<div><img src="../assets/floco2.png" alt="14" /></div>
			<div><img src="../assets/floco3.png" alt="15" /></div>
			<div><img src="../assets/floco4.png" alt="16" /></div>
		</div>
	</section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Poppins:200,300,400,500,600,700,800,900&display=swap');

* {
	font-family: 'Poppins';
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
section {
	position: relative;
	width: 100%;
	height: 100vh;
	background: radial-gradient(rgb(252, 252, 252), rgb(163, 197, 248));
	overflow: hidden;
	display: flex;
	justify-content: center;
	align-items: center;
}
section h2 {
	color: rgb(63, 106, 245);
	font-size: 7em;
	text-transform: uppercase;
}
section .set {
	position: absolute;
	width: 100%;
	height: 100%;
	top: 0;
	left: 0;
	pointer-events: none;
}
section .set div {
	position: absolute;
	display: block;
}
section .set div img {
	width: 25%;
}
section .set div:nth-child(1) {
	left: 20%;
	animation: animate 15s linear infinite;
	animation-delay: -7s;
}
section .set div:nth-child(2) {
	left: 50%;
	animation: animate 20s linear infinite;
	animation-delay: -5s;
}
section .set div:nth-child(3) {
	left: 70%;
	animation: animate 20s linear infinite;
	animation-delay: 0s;
}
section .set div:nth-child(4) {
	left: 0%;
	animation: animate 15s linear infinite;
	animation-delay: -5s;
}
section .set div:nth-child(5) {
	left: 85%;
	animation: animate 18s linear infinite;
	animation-delay: -10s;
}
section .set div:nth-child(6) {
	left: 0%;
	animation: animate 12s linear infinite;
}
section .set div:nth-child(7) {
	left: 15%;
	animation: animate 14s linear infinite;
}
section .set div:nth-child(8) {
	left: 60%;
	animation: animate 15s linear infinite;
}

section .set div:nth-child(9) {
	left: 20%;
	animation: animate 15s linear infinite;
	animation-delay: -7s;
}
section .set div:nth-child(10) {
	left: 50%;
	animation: animate 20s linear infinite;
	animation-delay: -5s;
}
section .set div:nth-child(11) {
	left: 70%;
	animation: animate 20s linear infinite;
	animation-delay: 0s;
}
section .set div:nth-child(12) {
	left: 0%;
	animation: animate 15s linear infinite;
	animation-delay: -5s;
}
section .set div:nth-child(13) {
	left: 85%;
	animation: animate 18s linear infinite;
	animation-delay: -10s;
}
section .set div:nth-child(14) {
	left: 0%;
	animation: animate 12s linear infinite;
}
section .set div:nth-child(15) {
	left: 15%;
	animation: animate 14s linear infinite;
}
section .set div:nth-child(16) {
	left: 60%;
	animation: animate 15s linear infinite;
}

@keyframes animate {
	0% {
		opacity: 0;
		top: -10%;
		transform: translateX(20px) rotate(0deg);
	}
	10% {
		opacity: 1;
	}
	20% {
		transform: translateX(-20px) rotate(45deg);
	}
	40% {
		transform: translateX(-20px) rotate(90deg);
	}
	60% {
		transform: translateX(20px) rotate(180deg);
	}
	80% {
		transform: translateX(-20px) rotate(180deg);
	}
	100% {
		top: 110%;
		transform: translateX(-20px) rotate(225deg);
	}
}
</style>
