<script>
	import Header from './Header.svelte';
	import '../app.css';

	const headerLinks = [
		"トップページ",
		"イベント概要",
		"サークル参加要項",
		"みみけん（受理確認）",
		"チラシ、業者搬入、企業出展、取材に関して",
		"問合せ",
		"主催ケットコム",
		"サークルリスト"
	];
</script>

<div class="app">
	<!-- <Header /> -->
	<header>
		{#each headerLinks as link}
			<span>[</span>
			<a href="https://svelte.dev">{link}</a>
			<span>]</span>
		{/each}
	</header>

	<main>
		<slot />
	</main>

	<footer>
		<!-- <p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p> -->
		<span>※VOCALOID（ボーカロイド）はヤマハ株式会社の登録商標です。</span>
		<span>※なお、バナー画像を除く、このホームページに掲載されている全ての画像・文字情報・その他の一部または全部を転載・掲載することは禁止です。</span>
		<span>但し、ネットの他の掲示板、同人誌、ペーパー、その他で「こんなイベントがあるよー。」程度の引用なら構いません。その際に告知アドレスhttps://ketto.com/tvm/を記載（サイトの場合リンク）してください。</span>
		<a href="https://ketto.com/kojin.htm">個人情報保護法</a>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		/* max-width: 64rem; */
		margin: 0 auto;
		box-sizing: border-box;

	}

	footer {
		font-size: 12px;

		a {
			font-weight: bold;
		}
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
