<script>
    import {
        SiHtml5,
        SiCss,
        SiJavascript,
        SiNodedotjs,
        SiSvelte,
        SiTypescript,
        SiReact,
        SiPython,
        SiPhp,
        } from "@icons-pack/svelte-simple-icons";
</script>

<section>
    <h1>Skills</h1>
    <p>I know how to do some of these things:</p>
    <ul>
        <li><span><SiHtml5 /></span>HTML</li>
        <li><span><SiCss /></span>CSS</li>
        <li><span><SiJavascript /></span>JavaScript</li>
        <li><span><SiNodedotjs /></span>Node.js</li>
        <li><span><SiSvelte /></span>Svelte</li>
    </ul>
    <p>Things that I've touched but I am willing to learn more:</p>
    <ul>
        <li><span><SiTypescript /></span>TypeScript</li>
        <li><span><SiReact /></span>React</li>
        <li><span><SiPython /></span>Python</li>
        <li><span><SiPhp /></span>PHP</li>
    </ul>
</section>

<style>
    ul {
        display: flex;
        justify-content: space-around;
        align-items: center;

        li {
            display: flex;
            align-items: center;
            color: var(--clr-black);
            background-color: var(--clr-white);
            padding: 1rem;
            border-radius: 20px;

            span {
                margin-right: 5px;
            }

            &::selection {
                text-shadow: none;
            }
        }
    }
</style>