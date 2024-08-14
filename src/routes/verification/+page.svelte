<script>
	import DTlogo from '$assets/dt-logo.svelte';
	import DTbtnIcon from '$assets/dt_btn_icon.svelte';
</script>

<svelte:head>
	<title>Confirm Account</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="header__section">
	<div class="header__wrapper">
		<div class="header-left__wrapper">
			<a href="/login"><DTlogo /></a>
		</div>

		<div class="dt-progress-tracker dt-container">
			<div class="dt-progress-tracker-item__container --active">
				<div class="dt-progress-tracker__item --active">1</div>
				<span class="dt-text-sm">Create DataTools Account</span>
			</div>
			<div class="dt-progress-tracker-item__container">
				<div class="dt-progress-tracker__item">2</div>
				<span class="dt-text-sm">Enter Password</span>
			</div>
			<div class="dt-progress-tracker-item__container">
				<div class="dt-progress-tracker__item">3</div>
				<span class="dt-text-sm">Confirm Account</span>
			</div>

			<div class="dt-progress-tracker__center-line"></div>
		</div>

		<div class="header-right__wrapper">
			<span>Already have an account?</span>
			<a href="">Sign in now</a>
		</div>
	</div>

	<div class="dt-line-progress-tracker">
		<div class="dt-line-progress-tracker__bar"></div>
	</div>
</section>

<section class="main__section">
	<div class="main__container pink-shadow">
		<div class="content-top__wrapper">
			<div class="content-text__wrapper--row-between">
				<div class="back-arrow__wrapper clickable">
					<img src="./assets/dt-back-arrow-icon.svg" alt="" />
				</div>
				<span class="dt-text uppercase">Step 3 to 3</span>
				<div class="back-arrow__wrapper visually-hidden">
					<img src="./assets/dt-back-arrow-icon.svg" alt="" />
				</div>
			</div>

			<div class="content-text__wrapper align-center">
				<h1 class="dt-text-heading-1">Confirm your account?</h1>
				<p class="dt-text-xl w-75">
					We sent a 6-digit verification code to your email
					<strong>nicholas@datatools.com.au</strong>
				</p>
			</div>
		</div>

		<div class="form__wrapper">
			<label for="input-number"
				><span class="dt-text-heading-4">Enter the code to continue</span></label
			>
			<div class="verification-input_wrapper">
				<div class="square-input-text__wrapper">
					<input type="text" id="input-number" required="required" />
				</div>
				<div class="square-input-text__wrapper">
					<input type="text" id="input-number" required="required" />
				</div>
				<div class="square-input-text__wrapper">
					<input type="text" id="input-number" required="required" />
				</div>
				<div class="square-input-text__wrapper">
					<input type="text" id="input-number" required="required" />
				</div>
				<div class="square-input-text__wrapper">
					<input type="text" id="input-number" required="required" />
				</div>
				<div class="square-input-text__wrapper">
					<input type="text" id="input-number" required="required" />
				</div>
			</div>

			<div class="dt-btn">
				<span>Confirm Account</span>
				<DTbtnIcon />
			</div>

			<button class="dt-btn dt-btn--ghost" onclick="location='sign-up-1.html'">
				<span>Didn't receive the code? <a href="">Resend code</a></span>
			</button>
		</div>
	</div>
</section>
