<script>
    import { page } from '$app/state';
	import Link from '$lib/Link.svelte';

    let status = page.status;
</script>
  
<div id="content">
<h1 class="text-3xl font-bold text-center mt-10">
    <Link url="https://http.cat/{status}" newTab={true}>{status}</Link>
</h1>
</div>

<style>
    #content {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 100vh;
    }

    h1 {
        font-size: 2rem;
        font-weight: bold;
        margin-bottom: 1rem;
    }
</style>
