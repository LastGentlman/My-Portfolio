<section class="my-work" id="projects">
    <h2 class="section__title">My Projects</h2>
    <p class="section__subtitle">Selection of Projects</p>
    
    <div class="portfolio">
        <!-- My Weather Web App -->
        <a href="weather" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/main/src/assets/imgs/weatherPic.png" alt="My Weather Web App" class="portfolio__img">
        </a>
        
        <!-- My Paint Board -->
        <a href="paint" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="My Paint Board" class="portfolio__img">
        </a>
        
        <!-- My Meme Generator -->
        <a href="meme" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="My Meme Generator" class="portfolio__img">
        </a>
        
        <!-- Rock Paper Scissors Game -->
        <a href="rpsgame" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="Rock, Paper & Scissors Game" class="portfolio__img">
        </a>

        <!-- My Recipes -->
        <a href="../views/recipes" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="My Recipes App" class="portfolio__img">
        </a>

        <!-- My Brilliant Idea -->
        <a href="story" target="_blank" class="portfolio__item">
            <img src="https://raw.githubusercontent.com/LastGentlman/My-Portfolio/template/src/assets/imgs/01.png" alt="My Brilliant Idea" class="portfolio__img">
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