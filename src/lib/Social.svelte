<script>
	import Icon from '@iconify/svelte';
	import Link from './Link.svelte';

	/** @type{any & {
	 * platform: "youtube" | "discord" | "tiktok" | "facebook",
	 * children?: import("svelte").Snippet,
	 * }}
	 * */
	let { url, icon, children, ...others } = $props();
</script>

<Link newTab={true} {url}>
	{#if children}
		{@render children()}
	{:else}
		<Icon {icon} {...others} />
	{/if}
</Link>