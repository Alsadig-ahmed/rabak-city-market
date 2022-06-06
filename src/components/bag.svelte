<script>
	import b from '../../src/bags-imgs/IMG-20210823-WA0000.jpg';
	export let img = b;
	export let price;
	export let description;
    
	let infostutus = true;
	const toggle = () => {
		infostutus ? (infostutus = false) : (infostutus = true);
	};
</script>

<div class="bag">
	<img alt="صورة الحقيبة" id="photo" src={img} />
	<p>{description}</p>
	<div id="properties" />
	<div>
		<div id="info">
			<h3>
				{#if infostutus}
					<h3><slot name="price" /> سعر الحقيبة :  {price} جنية</h3>
					<h3><slot name="delivery" /></h3>
					<!-- <p>رقم الهاتف :0963003102</p>
					<p>رقم حساب بنكك : 2723330</p> -->
				{/if}
			</h3>
		</div>
		<button on:click={toggle}><h4>معلومات الشراء</h4></button>
		<!-- <button on:click={()=>{infostutus ? infostutus = false: infostutus = true}}><h4>معلومات الشراء</h4></button> -->
	</div>
</div>

<style>
	.bag {
		background-color: #eee;
		margin: 0.3rem;
	}
	button {
		width: 100%;
		border-radius: 35px 35px;
		background-color: #333;
		color: white;
		font-size: 1em;
	}
	img {
		width: 70%;
		border-radius: 35px 35px;
	}
</style>
