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
    <About />
    <Skills />
    <Projects />
    <footer>
        <p>&copy; 2026 Ash Chapman</p>
        <p>AI was <strong>NOT</strong> used in the making of this site.</p>
    </footer>
</main>