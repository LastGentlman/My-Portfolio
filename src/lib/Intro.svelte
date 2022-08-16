<section class="intro" id="home">
    <h1 class="section__title section__title--intro">
        Hi, I'm <strong>Rodrigo F.</strong>
    </h1>
    <p class="section__subtitle section__subtitle--intro">SOFTWARE ENGINEER</p>
    <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/main/src/assets/imgs/photo.jpeg" alt="nice looking dude" />
</section>

<style>
    .intro {
        position: relative;
    }

    .section__subtitle--intro {
        display: inline-block;
    }

    img {
        box-shadow: var(--shadow);
        width: 249px;
        height: 249px;
    }

    @media (min-width:600px) {
        .intro {
            display: grid;
            grid-template-areas: 
                "img title"
                "img subtitle";
            grid-template-columns: min-content max-content;
            column-gap: 1em;
            width: min-content;
            margin: 0 auto;
        }

        img {
            grid-area: img;
            min-width: 250px;
            position: relative;
            z-index: 2;
        }   

        .section__subtitle--intro {
            align-self: start;
            grid-column: -1 / 1;
            grid-row: 2;
            text-align: right;
            position: relative;
            z-index: 1;
            left: -1.5em;
            width: calc(100% + 1.5em)
        }
    }
</style>