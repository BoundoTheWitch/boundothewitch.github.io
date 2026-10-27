<script>
    import Nav from "./lib/Nav.svelte";
    import Hero from "./lib/Hero.svelte";
    import About from "./lib/About.svelte";
    import Skills from "./lib/Skills.svelte";
    import Projects from "./lib/Projects.svelte";
    import { ExternalLink, LucideExternalLink } from "@lucide/svelte";
</script>

<Nav />
<main class="center">
    <Hero />
    <About />
    <Skills />
    <Projects />
    <footer>
        <p>&copy; 2026 Ash Chapman</p>
        <p>This site was built using <a href="https://svelte.dev/" target="_blank">Svelte<ExternalLink size="12" rel="noreferrer nofollow" /></a> with <a href="https://vite.dev/" target="_blank" rel="noreferrer nofollow">Vite<ExternalLink size="12" /></a></p>
    </footer>
</main>

<style>
    footer {
        a:link, a:visited {
            text-decoration: underline;
        }
    }
</style>