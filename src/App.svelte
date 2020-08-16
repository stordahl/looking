<script>
	import { fade } from 'svelte/transition';

	let src = '/water.mp4';
</script>

<main>
	<video autoplay muted loop id="video" >
		<source src="{ src }" type="video/mp4">
	</video>

	<div>
		<h3>l o o k i n g &nbsp;out over the ocean,</h3> 
		<h3>i forgot where I thought I was going</h3>
	</div>
</main>

<style>
	main{
		width:100vw;
		height:100vh;
		animation: fadeIn 10s linear;
		
	}
	#video {
		position: absolute;
		margin: auto;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		height: 100vh;
		width: 100vw;
		scale:0.8;
		z-index: -1;
		
	}
	div{
		position: absolute;
  		margin: auto;
  		top: 0;
  		right: 0;
  		bottom: 0;
	    left: 0;
		background-color:#16202d;
		opacity: 95%;
		width:max-content;
		height:max-content;
		max-height:100px;
		padding: 5vw;
    	display: flex;
    	flex-direction: column;
    	align-content: center;
		justify-content: center;
		/* animation: fadeIn 5s linear; */
	}
	h3{
		color:rgb(186, 206, 223);
		width:max-content;
		font-family: 'Cormorant Garamond', serif;
		font-size:3vw;
		line-height:1.4;
		margin:0;
	}
	@keyframes fadeIn {
		from{
			opacity:0;
		}
		to{
			opacity:1;
		}
	}
	@keyframes fadeOut {
		from{
			opacity:1;
		}
		to{
			opacity:0;
		}
	}
</style>