<script>
    import Nav from "./lib/Nav.svelte";
    import Hero from "./lib/Hero.svelte";
    import About from "./lib/About.svelte";
    import Skills from "./lib/Skills.svelte";
    import Projects from "./lib/Projects.svelte";
</script>

<Nav />
<main class="center">
    <Hero />
    <div class="break">
        <About />
        <Skills />
    </div>
    <Projects />
</main>
<footer class="center">
    <p>&copy;2026 Boundo the Witch</p>
    <p>AI was <strong>NOT</strong> used in making this site.</p>
</footer>
