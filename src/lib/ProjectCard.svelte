<script>
    let { projName, projDesc, projImg, projImgAlt } = $props();
</script>

<div class="card">
    <img src={projImg} class="card-image" alt={projImgAlt} />
    <div>
        <h2 class="card-title">{projName}</h2>
        <p class="card-desc">{projDesc}</p>
    </div>
</div>

<style>
    .card {
        display: flex;
        margin: 1.5rem 0;

        div {
            margin-left: 20px;
            display: grid;
        }

        .card-title {
            line-height: 0;
        }

        .card-image {
            width: 200px;
            aspect-ratio: 16/9;
            background-color: grey;
        }
    }
</style>