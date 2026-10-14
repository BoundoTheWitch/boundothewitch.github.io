<script>
    let { projName, projDesc, projImg, projImgAlt, projLink, projSrc } = $props();
    import { ExternalLink } from "@lucide/svelte";
</script>

<div class="card">
    <img src={projImg} class="card-image" alt={projImgAlt} />
    <div>
        <h2 class="card-title">{projName}</h2>
        <p class="card-desc">{projDesc}</p>
            <p class="card-links">
                {#if projLink}
                <a href={projLink}>Website <ExternalLink size="12" /></a>
                {/if}
            </p>
            <p class="card-links">
                {#if projSrc}
                <a href={projSrc}>Source <ExternalLink size="12" /></a>
                {/if}
            </p>
    </div>
</div>

<style>
    .card {
        display: flex;
        align-items: flex-start;
        margin: 1.5rem 0;
            font-size: 0.9rem;


        div {
            margin-left: 20px;
            display: grid;
        }

        .card-title {
            line-height: 0;
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

        .card-image {
            width: 200px;
            aspect-ratio: 16/9;
            background-color: grey;
        }

        .card-links {
            margin: 0.5rem 0;
        }
    }

    @media (min-width: 320px) and (max-width: 849px) {
        .card {
            flex-flow: column-reverse;
            place-items: center;
            margin-left: 0;

            div {
                margin-left: 0;
            }
        }
    }
</style>