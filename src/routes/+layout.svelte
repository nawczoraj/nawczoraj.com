<script>
	import '../app.css';

	let { children } = $props();
</script>


<div class="flex h-full w-full flex-col items-center dark:text-white">
	<video
		class="brightness-50 absolute -z-10 h-full w-full object-cover"
		poster="/hero.png"
		muted
		autoplay
		loop
		playsinline
		disablepictureinpicture
	>
		<source src="/hero.webm" type="video/webm" />
	</video>
	{@render children()}
</div>