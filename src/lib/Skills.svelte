<script>
    import {
        SiHtml5,
        SiCss,
        SiNodedotjs,
        SiJavascript,
        SiTypescript,
    } from "@icons-pack/svelte-simple-icons";
</script>

<section class="skills">
    <h1>Skills</h1>
    <p>Currently I am skilled in...</p>
    <ul>
        <li><span><SiHtml5 /></span>HTML5</li>
        <li><span><SiCss /></span>CSS3</li>
        <li><span><SiNodedotjs /></span>Node.js</li>
        <li><span><SiJavascript /></span>JavaScript</li>
        <li><span><SiTypescript /></span>TypeScript</li>
    </ul>
    <p>
        If a project requires me to learn something I don't have strong
        knowledge in then I will invest time to learn!
    </p>
</section>

<style>
    .skills {
        text-align: center;
    }

   ul {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    li {
        text-shadow: 2px 2px 0 black;
        padding: 0 1rem;
        height: 3rem;
        margin: 0.2rem;
        display: inline-flex;
        align-items: center;
        background-color: var(--purple-600);
        border-radius: 20px;

        span {
            margin-right: 10px;
        }
    }
</style>
