<script>
    import ProjectCard from "./ProjectCard.svelte";

    import sitePreview from '../assets/img/portfolio-preview.jpg';
</script>

<section>
    <h1>Projects</h1>
    <ProjectCard
        projName="Portfolio site"
        projDesc="The very site you're on! This was made using SvelteKit built as a static site."
        projLink="https://boundothewitch.github.io/"
        projImg={sitePreview}
        projImgAlt="Small preview of the portfolio site"
    />
</section>

<style>

</style>