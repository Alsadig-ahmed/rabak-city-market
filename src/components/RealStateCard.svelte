<script>
export let Image ='';
export let landOwner ='';
export let location ='';
export let description ='';
</script>

<section>
		<div class="flex card">
			<h2 class="img">صورة {Image}</h2>
			<div class="">
				<p>المالك : {landOwner}</p>
				<h2>وصف لقطعة الارض : {description}</h2>
				<h2>الموقع : {location}</h2>
			</div>
		</div>
</section>

<style>
	.flex {
		display: flex;
	}
	.card {
		border: 1px solid rgba(0, 0, 0, 0.13);
		text-align: center;
		margin: 0.5rem auto;
		border-radius: 2rem;
		box-shadow: 0 0 12px 0px rgba(0, 0, 0, 0.616);
	}
	.img {
		width: 50%;
		height: 12rem;
		border-radius: 2rem;
		background-color: rgb(211, 236, 209);
		margin-inline: 2rem;
	}
</style>
