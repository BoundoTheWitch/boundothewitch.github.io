<script>
    import logo from '../assets/img/logo.svg';
</script>

<section class="hero">
    <div>
        <img src={logo} alt="Ash Chapman's logo" />
        <p>Freelance Front-End Web Developer</p>
    </div>
</section>

<style>
    .hero {
        display: grid;
        place-items: center;
        height: 40dvh;
        margin-top: 5rem;
        text-align: center;
        p {
            font-size: 1.25rem;
        }

        img {
            width: clamp(192px, 30vw, 384px);
            aspect-ratio: 5/3;
        }
    }
</style>
