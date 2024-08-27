<script>
	import logoMain from '$lib/images/logo.png';
	import logoSub from "$lib/images/awd.png";
	import background from "$lib/images/background.png";


	// import Counter from './Counter.svelte';
	// import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>THE VOCALOID MASTER - 2024秋</title>
	<meta name="description" content="とろサー主催" />
</svelte:head>

<section>
	<img class="Background" src={background} alt="" />
	<div class="Top">
		<img class="Welcome" src={logoMain} alt="welcome" />
		<!--! Sub Logo  -->
		<!-- <img class="Welcome" src={logoSub} alt="welcome" /> -->

		<span>ボーカロイドonly event</span>
		<span style="font-size: 2em;">「THE VOCALOiD MASTER５７」</span>
		<span style="font-size: 1em;"><br>略称は「<b>ボーマス</b>」です。</span>
		<span style="font-size: 1em;">※入場は同日同会場開催で共通となります。</span>
	</div>

	<div class="Event-Desc">
		<a href="https://twitter.com/awd_vocaloid">イベント概要</a>
	</div>

	<div class="Notification-Widget">
		<table class="Notification-Table">
			<tbody>
				<tr>
					<td>お知らせ</td>
					<td><br><br>[2024/08/28] サイト更新しました。THE VOCALOiD MASTER５７サークル参加募集中。</td>
				</tr>
			</tbody>
		</table>
	</div>


	<!-- <h1>THE VOCALOID MASTER - 2024秋</h1>
	<h2>9/21 & 9/22</h2> -->
<!--
	<h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/png" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

		<!-- to your new<br />SvelteKit app -->
	<!-- </h1> -->

	<!-- <Counter /> -->
</section>

<style>
	section {
		.Background {
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			z-index: -1;
		}

		.Top {
			position: relative;
			height: auto;
			padding-bottom: 64px;
			display: flex;
			flex-direction: column;
			align-items: center;
			flex: 1;
			border-radius: 64px;
			background-color: #FFFFFF80;
			box-shadow: 0 8px 8px #00000080;
			text-shadow: 0 1px 2px #9e563a;



			.Welcome {
				width: 40%;
				aspect-ratio: 1.75 / 1;
			}

			span {
				position: relative;
				top: 32px;
				font-size: 1.2vw;
				font-weight: 600;
				color: #101010;
			}
		}

		.Event-Desc {
			position: relative;
			top: 32px;

			display: flex;
			flex-direction: column;
			align-items: center;

			border-radius: 64px;
			background-color: #FFFFFF80;
			box-shadow: 0 8px 8px #00000080;

			a {
				font-size: 32px;
			}
		}

		.Notification-Widget {
			position: relative;
			top: 64px;
			display: flex;
			justify-content: center;
			font-weight: 800;

			.Notification-Table {
				position: relative;
				width: 75%;
				font-size: 16px;
				border: thick double #404040;
				background-color: #F0FFFF;

				td:first-child {
					font-size: 2em;
				}
			}
		}

	}

	h1 {
		font-size: 4vw;
		font-weight: 400;
	}

	h2 {
		position: relative;
		top: -64px;
		font-size: 2vw;
		font-weight: 600;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
