<script>
	import DTlogo from '$assets/dt-logo.svelte';
	import DTbtnIcon from '$assets/dt_btn_icon.svelte';
</script>

<svelte:head>
	<title>Sign Up</title>
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
			<a href="/login">Sign in now</a>
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
				<span class="dt-text uppercase">Step 1 to 3</span>
				<div class="back-arrow__wrapper visually-hidden">
					<img src="./assets/dt-back-arrow-icon.svg" alt="" />
				</div>
			</div>

			<div class="content-text__wrapper align-center">
				<h1 class="dt-text-heading-1 w-90">Create your DataTools Account</h1>
				<p class="dt-text-xl w-75">
					One DataTools account is all you need to access all your services.
				</p>
			</div>
		</div>

		<div class="form__wrapper">
			<div class="two-col__wrapper">
				<div class="input-text__wrapper">
					<input type="text" id="input-name" required="required" />
					<label for="input-name">First name<span class="required-text">*</span></label>
				</div>
				<div class="input-text__wrapper">
					<input type="text" id="input-lastname" required="required" />
					<label for="input-lastname">Last name<span class="required-text">*</span></label>
				</div>
			</div>
			<div class="input-text__wrapper">
				<input type="text" id="input-email" required="required" />
				<label for="input-email">Email address<span class="required-text">*</span></label>
			</div>

			<div class="input-check__wrapper">
				<input type="checkbox" id="checkbox-marketing" />
				<label class="dt-text-sm" for="checkbox-marketing"
					>I agree to receive exclusive content, early access, special offers and other
					communications from DataTools Pty Ltd.</label
				>
			</div>

			<div class="input-check__wrapper">
				<input type="checkbox" id="checkbox-TOC" />
				<label class="dt-text-sm" for="checkbox-TOC"
					>By ticking the box, I agree to
					<a href="">DataTools Terms of Service</a>,
					<a href="">Payments Terms of Service and Anti-Discrimination Policy</a>
					and <a href="">acknowledge the Privacy Policy.</a>
				</label>
			</div>

			<button class="dt-btn dt-btn--disabled" disabled>
				<span>Continue</span>
				<DTbtnIcon />
			</button>
		</div>
	</div>
</section>
