<script>
	import Preloader from './Preloader.svelte'
	export let name
</script>

<main>
	<Preloader />
	<section class="container-fluid main-container container-home">
    <div class="color-block d-none d-lg-block"></div>
    <div class="row home-details-container align-items-center">
        <div class="col-lg-4 bg position-fixed d-none d-lg-block"></div>
        <div class="col-12 col-lg-8 offset-lg-4 home-details text-left text-sm-center text-lg-left">
            <div>
								<!-- svelte-ignore a11y-img-redundant-alt -->
								<img src="image-3-square.jpeg" class="img-fluid main-img-mobile d-none d-sm-block d-lg-none" alt="profile picture" />	
                <h1 class="text-uppercase poppins-font">I'm {name}.<span>software dev</span></h1>
                <p class="open-sans-font">I'm an Indonesian based software developer focused on building back-end side. I am passionate about building excellent software that improves the lives of those around me.</p>
								<a class="button" href="/">
									<span class="button-text">more about me</span>
									<span class="button-icon fa fa-arrow-right"></span>
								</a>
            </div>
        </div>
    </div>
	</section>
</main>

<style>
	
	.bg {
		background-image: url(/image-3.jpeg);
		background-size: cover;
		background-repeat: no-repeat;
		background-position: top;
		height: calc(100vh - 80px);
		z-index: 111;
		border-radius: 30px;
		left: 40px;
		top: 40px;
		box-shadow: 0 0 7px rgba(0,0,0,.9);
	}
</style>