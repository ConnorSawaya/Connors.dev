<script lang="ts">
</script>

<svelte:head>
	<title>About - Connor Sawaya</title>
</svelte:head>

<main>
	<div class="container">
		<header class="page-header">
			<h1>About Me</h1>
		</header>

		<div class="content">
			<div class="photo-container">
				<img src="/photo of me.jpg" alt="Connor Sawaya" class="profile-photo" />
				<div class="easter-egg">
					<p>
						Fun fact: When I'm not coding, I'm usually rebuilding the engine on my CR85. 
						Check out my mechanical and hardware builds on 
						<a href="/projects" style="color: rgb(176, 135, 255) !important;">my projects page</a>.
					</p>
				</div>
			</div>
			
			<div class="text-section">
				<p>
					Hey, I'm Connor. I'm a high school freshman and developer focused on building software that solves real-world problems. From winning Best UI/UX at Stang Hacks to developing full-stack tools for underserved communities, I love the challenge of turning complex ideas into functional code.
				</p>
				<p>
					I specialize in Python and Java, with a background in building everything from AI-powered health scanners to custom Minecraft utility mods. Beyond the terminal, I’m into mechanical engineering, DIY electronics, and finding ways to make technology more accessible.
				</p>
				<p>
					Take a look at my recent hackathon wins and technical builds on my <a href="/projects" style="color: rgb(176, 135, 255) !important;">projects page</a>.
				</p>
			</div>
		</div>
	</div>
</main>

<style>
/* Keeping your existing CSS structure as it's solid for this layout */
	main {
		min-height: 100vh;
		padding: 100px 24px 80px;
		background: #f8f9fa;
	}

	.container {
		max-width: 800px;
		margin: 0 auto;
	}

	.page-header {
		text-align: center;
		margin-bottom: 48px;
	}

	.page-header h1 {
		font-size: 3rem;
		font-weight: 700;
		margin: 0;
		color: #000000;
	}

	.content {
		background: #ffffff;
		border: 2px solid #000000;
		border-radius: 16px;
		padding: 48px;
		box-shadow: 4px 4px 0px #000000;
		display: flex;
		gap: 40px;
		align-items: flex-start;
	}

	.photo-container {
		position: relative;
		flex-shrink: 0;
		width: 350px;
	}

	.profile-photo {
		width: 100%;
		height: auto;
		border: 3px solid #000000;
		box-shadow: 4px 4px 0px #000000;
		transition: all 0.3s ease;
		display: block;
	}

	.profile-photo:hover {
		transform: translate(-2px, -2px);
		box-shadow: 6px 6px 0px #000000;
	}

	.easter-egg {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background: rgba(255, 208, 116, 0.98);
		border: 3px solid #000000;
		box-shadow: 4px 4px 0px #000000;
		padding: 24px;
		display: flex;
		align-items: center;
		justify-content: center;
		opacity: 0;
		pointer-events: none;
		transition: opacity 0.3s ease;
	}

	.easter-egg p {
		text-align: left;
		font-weight: 600;
		font-size: 0.95rem;
		line-height: 1.6;
		margin: 0;
		color: #000000;
	}

	.photo-container:hover .easter-egg {
		opacity: 1;
		pointer-events: auto;
	}

	.easter-egg a {
		color: #000000;
		text-decoration: underline;
		text-underline-offset: 2px;
		font-weight: 700;
	}

	.text-section {
		flex: 1;
		min-width: 0;
	}

	.text-section a {
		color: rgba(176, 135, 255, 1) !important;
		text-decoration: underline;
		font-weight: 600;
	}

	.content p {
		font-size: 1.25rem;
		line-height: 1.8;
		color: #000000;
		margin: 0 0 24px 0;
		font-weight: 500;
	}

	@media (max-width: 768px) {
		.content {
			flex-direction: column;
		}
		.photo-container {
			width: 100%;
			max-width: 350px;
			margin: 0 auto;
		}
	}
</style>
