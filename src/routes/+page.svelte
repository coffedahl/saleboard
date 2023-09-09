<script lang="ts">
	import Goal from './goal.svelte';

	let today = new Date();
</script>

<h1>Säljdata</h1>

<section>
	<div class="title">
		<h1>Todays goals</h1>
		<p>{today.toLocaleDateString()}</p>
	</div>
	<div class="goal-container">
		<div class="goal">
			<Goal title="Sales" data="19 456 kr" />
		</div>
		<div class="goal">
			<Goal title="ID-Rate" data="70%" />
		</div>
		<div class="goal">
			<Goal title="Multiline" data="27,5%" />
		</div>
		<div class="goal">
			<Goal title="GPPT" data="151 kr" />
		</div>
	</div>
</section>
}

<style lang="scss">
	.title {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;

		h1,
		p {
			margin: 0;
		}
	}
	.goal-container {
		display: flex;
		align-items: center;
		justify-content: space-evenly;
		.goal {
			width: 20vw;
			background-color: grey;
		}
	}
</style>
