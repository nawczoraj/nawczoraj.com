<script>
	let { children, id = '', border = true, class: classes = '' } = $props();
	const borderTop = border ? 'border-t-2 border-t-(--color-outline)' : '';
</script>

<section
	{id}
	class="
    {borderTop} relative
    flex w-full grow flex-col items-center
    justify-center {classes}
    "
>
	{@render children()}
</section>