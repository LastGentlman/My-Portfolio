<section class="about" id="about">
    <header>
        <h2 class="section__title section__title--about">Who I'am</h2>
        <p class="section__subtitle section__subtitle--about">Software Engineer & Designer</p>
    </header>

    <div class="about-me__body">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit perferendis nemo, ipsum alias quibusdam fugiat totam, tempore in doloremque dolorem sit autem odit deleniti architecto temporibus excepturi aut voluptatibus odio.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit perferendis nemo, ipsum alias quibusdam fugiat totam, tempore in doloremque dolorem sit autem odit deleniti architecto temporibus excepturi aut voluptatibus odio.</p>
    </div>
    
    <!-- TODO: agregar foto de mi leyendole a la muchacha -->
    <img src="../src/assets/imgs/photo.jpeg" alt="nice looking engineer">
</section>

<style>
    .about {
        max-width: 1000px;
        margin: 0 auto;
    }

    img {
        box-shadow: var(--shadow);
        display: none;
    }

    @media (min-width: 600px) {
        .about {
            display: grid;
            grid-template-columns: 1fr 200px;
            grid-template-areas:
                "title img"
                "subtitle img"
                "text img";
        }

        .section__title--about {
            grid-area: title;
        }

        .section__subtitle--about {
            grid-column: 1 / -1;
            grid-row: 2;
            position: relative;
            z-index: 1;
            left: -1em;
            width: calc(100% + 11em);
            padding-left: 0.75em;
            padding-right: calc(200px + 1.5em);
        }

        img {
            display: inline;
            grid-area: img;
            position: relative;
            z-index: 2;
        }
    }
</style>