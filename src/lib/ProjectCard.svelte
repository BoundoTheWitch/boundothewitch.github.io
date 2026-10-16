<script>
    let { projName, projLink = '', projSrc = '', children } = $props();
    import { ExternalLink } from "@lucide/svelte";
</script>

<div class="card">
    <h2 class="card-title">{projName}</h2>
    {@render children?.()}
    <div class="card-links">
        {#if projLink !== ''}
        <p class="card-link">
            <a href={projLink} target="_blank">Website <ExternalLink size="12" /></a>
        </p>
        {/if}
        {#if projSrc !== ''}
        <p class="card-link">
            <a href={projSrc} target="_blank">Source <ExternalLink size="12" /></a>
        </p>
        {/if}
    </div>
</div>

<style>
    .card {
        display: flex;
        flex-flow: column;
        justify-content: center;
        color: var(--clr-white);
        box-sizing: border-box;
        background-color: var(--purple-300);
        padding: 12px;
        width: 400px;
        border-radius: 20px;
        font-size: 0.9rem;

        h2 {
            margin: 0;
            text-align: center;
        }

        a {
            color: var(--clr-white);
            text-decoration: none;
            transition: color 200ms;
            &:visited {
                color: var(--clr-white);
            }
            &:hover {
                color: var(--clr-blue);
            }
        }

        .card-links {
            display: flex;
            justify-content: space-around;
        }

        .card-link {
            margin: 0.5rem 0;
        }
    }

    @media (min-width: 320px) and (max-width: 849px) {
        .card {
            width: 100%;
        }
    }
</style>