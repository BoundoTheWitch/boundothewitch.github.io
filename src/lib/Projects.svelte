<script>
    import ProjectCard from "./ProjectCard.svelte";

    // Images
    import sitePreview from '../assets/img/portfolio-preview.jpg';
</script>

<section>
    <h1>Projects</h1>
    <p>At the moment I mostly do personal projects and ocassionally a project for others.</p>
    <div class="cards">
        <ProjectCard
            projName="Portfolio site"
            projDesc="The very site you're on! This was made using SvelteKit built as a static site."
            projLink="https://boundothewitch.github.io/"
            projSrc="https://github.com/BoundoTheWitch/boundothewitch.github.io"
        />
                <ProjectCard
            projName="Portfolio site"
            projDesc="The very site you're on! This was made using SvelteKit built as a static site."
            projLink="https://boundothewitch.github.io/"
            projSrc="https://github.com/BoundoTheWitch/boundothewitch.github.io"
        />
    </div>
</section>

<style>
    .cards {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 10px;
        place-items: center;

    }
    @media (min-width: 320px) and (max-width: 849px) {
        .cards {
            width: 100%;
        }
    }

    @media (min-width: 320px) and (max-width: 679px) {
        .cards {
            display: flex;
            flex-flow: column;
            justify-content: center;
            align-items: center;
        }
    }
</style>