<nav>
    <ul>
        <li>Who Am I?</li>
        <li>Skills</li>
        <li>Projects</li>
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
        background-color: rgba(0,0,0,0.1);
        font-size: 1.25rem;
        display: grid;
        place-items: center;
        ul li {
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
</style>