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
						Beyond software, I'm usually at the workbench. I find that a solid understanding of hardware and physical systems always makes for better code.
						<br /><br />
						Check out my builds on 
						<a href="/projects" style="color: rgb(176, 135, 255) !important;">my projects page</a>.
					</p>
				</div>
			</div>
			
			<div class="text-section">
				<p>
					Hi, I'm Connor. I’m a freshman at Bellarmine College Preparatory, specializing in software and hardware systems. 
				</p>
				<p>
					Much of my work originates from competitive hackathons. I created <strong>Ride2Rider</strong> at Stang Hacks, where it earned the award for Best UI/UX. I also developed <strong>GlobalBridge Connect</strong> during Lancer Hacks. I’ve always enjoyed the fast-paced challenge of bringing an idea to life in a single weekend.
				</p>
				<p>
					Beyond individual software, I am an active member of <strong>FTC Robotics Team 23230</strong> and a <strong>Life Scout</strong> in the BSA, currently working toward the rank of <strong>Eagle Scout</strong>. 
				</p>
				<p>
					I find that the practical experience gained in a workshop is as essential to my engineering process as the time spent at a code editor. Take a look at my recent hackathon wins and technical builds on my <a href="/projects" style="color: rgb(176, 135, 255) !important;">projects page</a>.
				</p>
			</div>
		</div>
	</div>
</main>

<style>
	main {
		min-height: 100vh;
		padding: 100px 24px 80px;
		background: #f8f9fa;
	}

	.container {
		max-width: 900px; /* Slightly wider to accommodate the formal text better */
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
		width: 300px;
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
		flex-direction: column;
		align-items: center;
		justify-content: center;
		opacity: 0;
		pointer-events: none;
		transition: opacity 0.3s ease;
		z-index: 10;
	}

	.easter-egg p {
		text-align: left;
		font-weight: 600;
		font-size: 0.9rem;
		line-height: 1.5;
		margin: 0;
		color: #000000;
	}

	.photo-container:hover .easter-egg {
		opacity: 1;
		pointer-events: auto;
	}

	.text-section {
		flex: 1;
		min-width: 0;
	}

	.text-section strong {
		font-weight: 700;
		color: #000000;
	}

	.text-section a {
		color: rgba(176, 135, 255, 1) !important;
		text-decoration: underline;
		font-weight: 700;
	}

	.content p {
		font-size: 1.15rem; /* Adjusted for formal readability */
		line-height: 1.7;
		color: #000000;
		margin: 0 0 20px 0;
		font-weight: 500;
	}

	@media (max-width: 850px) {
		.content {
			flex-direction: column;
			padding: 32px;
		}
		.photo-container {
			width: 100%;
			max-width: 300px;
			margin: 0 auto 24px;
		}
		.page-header h1 {
			font-size: 2.5rem;
		}
	}
</style>
