<section class="my-work" id="projects">
    <h2 class="section__title">My Projects</h2>
    <p class="section__subtitle">Selection of Projects</p>
    
    <div class="portfolio">

        <!-- TODO: agregar imagenes y links a proyectos -->
        <!-- Portfolio item 01 -->
        <a href="#" class="portfolio__item">
            <img src="../src/assets/Rectangle3.png" alt="" class="portfolio__img">
        </a>
        
        <!-- Portfolio item 02 -->
        <a href="#" class="portfolio__item">
            <img src="../src/assets/Screenshot1.png" alt="" class="portfolio__img">
        </a>
        
        <!-- Portfolio item 03 -->
        <a href="#" class="portfolio__item">
            <img src="../src/assets/Screenshot2.png" alt="" class="portfolio__img">
        </a>
        
        <!-- Portfolio item 03 -->
        <a href="#" class="portfolio__item">
            <img src="../src/assets/Screenshot3.png" alt="" class="portfolio__img">
        </a>
    </div>
</section>
<style>
    .my-work {
        background: var(--clr-dark);
        color: var(--clr-light);
        text-align: center;
    }

    .portfolio {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px,1fr));
    }

    .portfolio__item {
        background: var(--clr-label);
        overflow: hidden;
    }

    .portfolio__img {
        transition:
            transform 750ms cubic-bezier(.5, 0, .5, 1),
            opacity 250ms linear;
    }

    .portfolio__item:focus {
        position: relative;
        z-index: 2;
    }

    .portfolio__img:hover, .portfolio__item:focus .portfolio__img {
        transform: scale(1.1);
        opacity: .5;
    }
</style>