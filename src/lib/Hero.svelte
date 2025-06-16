<script>
	import Section from './Section.svelte';
	import Social from './Social.svelte';
</script>

<Section border={false} class="gap-8 select-none animate-fade-in, motion-safe, transition-">
    <div class="flex flex-col items-center justify-center gap-6 text-center [&>*]:hover:scale-110 [&>*]:transition [&>*]:duration-1000">
        <div class="invert-100">
        <img class="h-16" src="/logo.png" alt="" />
        </div>
        <nav aria-roledescription="Links to socials" class="flex items-center min-w-30 w-full justify-evenly">
            <Social url="/discord" icon="fa-brands:discord" class="text-xl" />
            <Social url="https://github.com/nawczoraj" icon="fa-brands:github" class="text-xl" />
            <Social url="https://linkedin.com/company/nawczoraj" icon="fa-brands:linkedin" class="text-xl" />
        </nav>
    </div>
</Section>