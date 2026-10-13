<script>

</script>

<section id="skills">
    <h1>Skills</h1>
    <p>I know how to do these things:</p>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>Node.js</li>
        <li>Svelte</li>
    </ul>
    <p>Things that I've touched but I am willing to learn more:</p>
    <ul>
        <li>TypeScript</li>
        <li>React</li>
        <li>Python</li>
        <li>PHP</li>
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