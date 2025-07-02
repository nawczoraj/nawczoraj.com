<script>
	import '../app.css';

	let { children } = $props();
</script>


<div class="flex h-full w-full flex-col items-center dark:text-white">
	<img src="/hero.png" alt="" class="absolute -z-10 h-full w-full object-cover" />
	{@render children()}
</div>