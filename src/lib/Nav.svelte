<nav>
    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
    </ul>
</nav>

<style>
    nav {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        backdrop-filter: blur(5px);
        z-index: 1;
        padding: 1rem 0;
        display: grid;
        place-items: center;
        border-bottom: 1px solid rgba(255,255,255,0.1);
        
        ul {
            width: 576px;
            display: flex;
            justify-content: space-around;
            align-items: center;
            font-size: 1.5rem;
            font-family: var(--fnt-header);
            li {
                margin: 0 15px;
                
                a {
                    color: var(--clr-white);
                    text-decoration: none;
                    transition: color 250ms;
                    &:visited {
                        color: var(--clr-white);
                    }
                    &:hover {
                        color: var(--clr-blue);
                    }
                }
            }
        }
    }

    @media (min-width: 320px) and (max-width: 575px) {
        nav {
            ul {
                width: 100%;
            }
        }
    }
</style>