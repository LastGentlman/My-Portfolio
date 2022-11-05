<section class="about" id="about">
    <header>
        <h2 class="section__title section__title--about">Who I'am</h2>
        <p class="section__subtitle section__subtitle--about">Polyfacetic Software Engineer</p>
    </header>

    <div class="about-me__body">
        <p>I Truly belive that its posible to develop a better world trough code, offcourse not only code is needed to make a positive impact on our planet, we need love in our hearths, because a person with love in its hearth wont commit acts that threaten the peace and health of other individuals</p>
        <p><a href="https://www.16personalities.com/infj-personality">INFJ-A</a> as Result of the <a href="https://www.16personalities.com/free-personality-test">16 personality test</a></p>
    </div>
    
    <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/main/src/assets/imgs/photo.jpeg" alt="nice looking engineer">
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