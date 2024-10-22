<script>
	import Unit from "$lib/Unit.svelte";
</script>

<div class="header">
	<a class="hover-underline-animation">Dashboard</a>
	<a class="hover-underline-animation">My Coruses</a>
	<a class="hover-underline-animation">Mission</a>
	<a class="hover-underline-animation">Contribute</a>
</div>
<div class="content">
	<div class="sidebar">
		<div class="coruse">
			<p>Programing</p>
		</div>
		<div class="units">
			<Unit name="Unit 1">
				<div class="lessonLinks">
					<a class="lessonLink">hey</a>
					<a class="lessonLink">hey</a>
					<a class="lessonLink">hey</a>
					<a class="lessonLink">hey</a>
					<a class="lessonLink">hey</a>
				</div>
			</Unit>
			<Unit name="Unit 2">
			
			</Unit>
		</div>
	</div>
	<div class="main">
		<div class="lessonContainer">
			<div class="lessonHeader">
				<div class="lessonName">
					<p>Lesson 1; Penis Studies, Quiz</p>
				</div>
				<div class="navigation">
					<button>Next</button>
				</div>
			</div>
			<div class="lesson">
				<p>lesson</p>
			</div>
		</div>
	</div>
</div>

<style>


.lessonLinks {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.lessonLink{
  font-size: initial;
  background: #00000024;
  border-radius: 10px;
  padding: 5px;
  width: 95%;
  margin: 3px;
}
	.hover-underline-animation {
		display: inline-block; /* Display inline block */
		position: relative; /* Set position relative */
	}

	.hover-underline-animation:after {
		content: ''; /* Add content after the element */
		position: absolute; /* Position absolute for pseudo-element */
		width: 100%; /* Full width */
		transform: scaleX(0); /* Initial scale of 0 for underline effect */
		height: 2px; /* Height of the underline */
		bottom: 0; /* Align to bottom */
		left: 0; /* Align to left */
		background-color: #000000; /* Background color of the underline */
		transform-origin: bottom right; /* Set transform origin */
		transition: transform 0.25s ease-out; /* Transition effect for the underline */
	}

	.hover-underline-animation:hover:after {
		transform: scaleX(1); /* Scale the underline on hover */
		transform-origin: bottom left; /* Set transform origin */
	}
	a {
		cursor: pointer;
	}
	p,a {
		font-size: x-large;
		padding: 0px;
		margin: 0px;
	}

	.coruse {
		background: rgb(2, 0, 36);
		background: linear-gradient(
			137deg,
			rgba(35, 27, 170, 0.59) 0%,
			rgba(122, 121, 185, 0) 0%,
			rgba(19, 19, 126, 0.78) 100%
		);
		width: 100%;
		padding: 10px;
		border-radius: 15px;
		aspect-ratio: 4/3;
		display: flex;
		align-items: end;
	}
	.header {
		padding: 25px;
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 80px;
	}
	.lessonContainer {
		height: 100%;
		gap: 10px;
		display: flex;
		flex-direction: column;
	}
	.content {
		height: 100%;
		display: flex;
		flex-direction: row;
		margin: 30px;
		margin-top: 0px;
	}

	.sidebar {
		max-width: 245px;
		flex-direction: column;
		width: 30%;
		margin: 25px;
		border-radius: 10px;
		display: flex;
		align-items: flex-start;
		justify-content: center;
		gap: 10px;
		margin-top: 0px;
	}

	.units {
		background: #b7b0dc8a;
		width: 100%;
		height: 100%;
		padding: 10px;
		border-radius: 15px;
	}
	.main {
		width: 100%;
		padding: 25px;
		background: #b7b0dc8a;
		border-radius: 10px;
		margin: 25px;

		margin-top: 0px;
	}
	.lessonHeader {
		display: flex;
		gap: 10px;
		align-content: center;
		align-items: center;
	}
	.lesson {
		width: 100%;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		background: white;
		border-radius: 10px;
	}
	.lessonContainer {
		height: 100%;
	}
	button {
		padding: 7px;
		justify-content: center;
		align-items: center;
		display: flex;
		background: black;
		border-radius: 6px;
		color: white;
		border: none;
		cursor: pointer;
	}
	.navigation {
		display: flex;
		align-items: center;
		justify-content: center;
	}
</style>
