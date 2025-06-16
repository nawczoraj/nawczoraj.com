<script>
	import Section from './Section.svelte';
	import Social from './Social.svelte';
</script>

<Section border={false} class="gap-8 select-none">
    <div class="flex flex-col items-center justify-center gap-8 text-center [&>*]:hover:scale-110 [&>*]:transition [&>*]:duration-1000">
        <div class="invert-100">
        <img class="h-48" src="/logo.png" alt="" />
        </div>
        <nav aria-roledescription="Links to socials" class="flex items-center w-56 justify-between [&>*]:text-4xl">
            <Social url="/discord" icon="fa-brands:discord" class="text-4xl" />
            <Social url="https://github.com/nawczoraj" icon="fa-brands:github" />
            <Social url="https://linkedin.com/company/nawczoraj" icon="fa-brands:linkedin" />
        </nav>
    </div>
</Section>