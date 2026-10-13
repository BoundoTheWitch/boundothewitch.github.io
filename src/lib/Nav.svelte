<nav>
    <ul>
        <li><a href="#about">Who Am I?</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
    </ul>
</nav>

<style>
    nav {
        position: fixed;
        left: 0;
        top: 0;
        width: 100%;
        backdrop-filter: blur(5px);
        padding: 10px;
        background-color: rgba(0, 0, 0, 0.1);
        font-size: 1.25rem;
        display: grid;
        place-items: center;

        ul {
            display: flex;
            a {
                color: var(--clr-white);
                text-decoration: none;
                text-shadow: 2px 2px 0 black;
                transition: color 100ms linear;
                &:hover {
                    color: var(--clr-blue);
                }
            }
            li {
                display: inline-block;
                margin: 0 10px;
                &:first-child {
                    margin-left: 0;
                    margin-right: 10px;
                }
                &:last-child {
                    margin-left: 10px;
                    margin-right: 0;
                }
            }
        }
    }
</style>
