<section class="hero">
    <h1>Boundo the Witch</h1>
</section>


<style>
    .hero {
        h1 {
            line-height: 0.5;
            margin: 1rem;
        }
        opacity: 0;
        box-sizing: border-box;
        font-size: clamp(1rem, 3.5vw, 2.5rem);
        height: 40dvh;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-flow: column;
        text-shadow: 3px 3px 0px #000;
        animation: fade-in 1s forwards;
        animation-timing-function: cubic-bezier(0.33, 1, 0.68, 1);
        animation-delay: 300ms;
    }

    @keyframes fade-in {
        0% {
            opacity: 0;
            transform: translateY(30px);
        }
        100% {
            opacity: 1;
            transform: translateY(0px);
        }
    }
</style>