<div class="card">
    <h2>Project name</h2>
    <div class="card-image"></div>
    <p>Project description</p>
</div>

<style>
    .card {
        width: 250px;
        display: grid;
        grid-template-rows: repeat(3, auto);
        place-items: center;
        border: 2px solid var(--clr-white);
        border-radius: 20px;
        .card-image {
            width: 200px;
            height: 100px;
            background: grey;
        }


    }
</style>