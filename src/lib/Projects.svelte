<script>
    import ProjectCard from "./ProjectCard.svelte";
</script>

<section id="projects">
    <h1>Projects</h1>
    <p>At the moment I mostly do personal projects and ocassionally a project for others.</p>
    <div class="cards">
        <ProjectCard
            projName="Portfolio site"
            projLink="https://boundothewitch.github.io/"
            projSrc="https://github.com/BoundoTheWitch/boundothewitch.github.io">
            <p>The very site you're on! This was made using Svelte and Vite built as a static site.</p>
        </ProjectCard>
        <ProjectCard
            projName="My Mother's Site (A-Star)"
            projLink="https://boundothewitch.github.io/moms-site"
            projSrc="https://github.com/BoundoTheWitch/moms-site">
            <p>My mother's website for her service dog training business. Eleventy/11ty was used to generate the site, with ssome JavaScript for being able to zoom into pictures. For privacy reasons I will share an offline version of the site with private info stripped out.</p>    
    </ProjectCard>
        <ProjectCard
            projName="Isabelle Bot"
            projSrc="https://github.com/BoundoTheWitch/isabellebot">
                <p>Isabelle Bot is a Discord bot developed for a friend's Discord server that provided interactive functions and audit capabilities. More info can be found on the GitHub repo.</p>
        </ProjectCard>
    </div>
</section>

<style>
    .cards {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 10px;
        place-items: stretch;
        

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
            align-items: stretch;
        }
    }
</style>