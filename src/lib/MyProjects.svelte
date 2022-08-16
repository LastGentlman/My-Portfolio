<section class="my-work" id="projects">
    <h2 class="section__title">My Projects</h2>
    <p class="section__subtitle">Selection of Projects</p>
    
    <div class="portfolio">
        <!-- Portfolio item 01 -->
        <a href="project01" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/main/src/assets/imgs/weatherPic.png" alt="" class="portfolio__img">
        </a>
        
        <!-- Portfolio item 02 -->
        <a href="project02" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="" class="portfolio__img">
        </a>
        
        <!-- Portfolio item 03 -->
        <a href="project03" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="" class="portfolio__img">
        </a>
        
        <!-- Portfolio item 04 -->
        <a href="project04" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="" class="portfolio__img">
        </a>

        <!-- Portfolio item 05 -->
        <a href="project05" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="" class="portfolio__img">
        </a>

        <!-- Portfolio item 06 -->
        <a href="project06" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="" class="portfolio__img">
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
        object-fit: inherit;
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