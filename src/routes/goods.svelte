<script>
</script>

<section>
	<img class="shoppers-img" src="../../src/bags-imgs/shoppers-img.png" alt="اشخاص يتسوقون" />
	<ul>
		<li><a href="/goods/bags"> متجر الشنط  <i class="shopping-bag"></i></a></li>
		<li><a href="/goods/chitchenware"> متجر الاواني المنزلية </a></li>
		<li><a href="/goods/shoes"> متجر الاحزية </a></li>
		<li><a href="/goods/clothes"> متجر الملابس </a></li>
	</ul>
</section>

<!-- <ul>
	<li><a href="/goods"> سوق السلع </a></li>
	<li><a href="/"> المعالم السيا حية </a></li>
</ul> -->
<style lang="scss">
	.shopping-bag{
		display: inline-block;
		padding: 1.3rem;
		background-image: url("../../src/bags-imgs/shopping-bag.png");
		background-position: center;
		background-size: contain;
		background-repeat: no-repeat;
	}
	
	.shoppers-img {
		width: 50%;
	}
	section {
		text-align: center;
		font-size: 2rem;
	}
	ul {
		// display: flex;
		// justify-content: space-around;

		li {
			list-style-position: inside;
			list-style-type: none;
			font-size: 3rem;
			font-weight: 500;
			margin: 0.1rem;
			border-radius: 1rem;
			background-color: rgb(229, 226, 226);
			&:hover {
				color: rgb(219, 197, 218);
				background-color: rgb(129, 124, 124);
			}
			a {
				text-decoration: none;
				color: rgb(53, 49, 53);
				padding: 0.5rem;
				&:hover {
					color: rgb(219, 197, 218);
				}
			}
		}
	}
</style>
