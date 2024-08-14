<script>
	import DTLoginImage from '$assets/dt-login-image.svelte';
	import DTbtnIcon from '$assets/dt_btn_icon.svelte';
</script>

<svelte:head>
	<title>Login</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="main__section h-100 full-page">
	<div class="main__container pink-shadow">
		<div class="content-top__wrapper">
			<DTLoginImage />

			<div class="content-text__wrapper align-center">
				<h1 class="dt-text-heading-1">DataTools Account</h1>
				<p class="dt-text-xl">
					One account for everything DataTools. Sign in to securely access all your DataTools
					services.
				</p>
			</div>
		</div>

		<div class="form__wrapper">
			<div class="input-text__wrapper">
				<input type="text" id="input-email" required="required" />
				<label for="input-email">Email address</label>
			</div>

			<div class="input-text__wrapper">
				<input type="password" id="input-password" required="required" />
				<label for="input-password">Password</label>
				<div>
					<img src="./assets/dt-password-show-icon.svg" alt="" />
				</div>
			</div>

			<button class="dt-btn">
				<span>Sign In</span>
				<DTbtnIcon />
			</button>
		</div>

		<div class="content-bottom__wrapper">
			<div class="input-check__wrapper">
				<input type="checkbox" id="remember-me" />
				<label for="remember-me">Remember me</label>
			</div>

			<a href="">Forgot password?</a>
		</div>
	</div>
</section>
