<script>
    import ProjectCard from "./ProjectCard.svelte";
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
            projName="My Mother's Site (A-Star)"
            projDesc="My mother's website for her service dog training business. No framework was used, just plain HTML, CSS, and some JavaScript. For privacy reasons I will share an offline version of the site with private info stripped out."
            projLink="https://boundothewitch.github.io/moms-site"
            projSrc="https://github.com/BoundoTheWitch/moms-site"
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