<script>
    let { projName, projDesc, projImg, projImgAlt, projLink } = $props();
</script>

<div class="card">
    <img src={projImg} class="card-image" alt={projImgAlt} />
    <div>
        <h2 class="card-title">
            <a href={projLink}>{projName}</a>
            <div class="icon"></div>
        </h2>
        <p class="card-desc">{projDesc}</p>
    </div>
</div>

<style>
    .card {
        display: flex;
        align-items: flex-start;
        margin: 1.5rem 0;

        div {
            margin-left: 20px;
            display: grid;
        }

        .card-title {
            line-height: 0;
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

            .icon {
                display: inline-block;
                margin: 0;
                width: 1.12rem;
                height: 1.12rem;
                background-image: url('data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6"><path stroke-linecap="round" stroke-linejoin="round" d="M13.5 6H5.25A2.25 2.25 0 0 0 3 8.25v10.5A2.25 2.25 0 0 0 5.25 21h10.5A2.25 2.25 0 0 0 18 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25" /></svg>');
                filter: invert(100%);
            }
        }

        .card-image {
            width: 200px;
            aspect-ratio: 16/9;
            background-color: grey;
        }
    }
</style>