<section class="my-services" id="services">
    <h2 class="section__title section__title--services">What I do</h2>

    <div class="services">

        <div class="service">
            <h3>Design + Development</h3>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil, commodi cupiditate. Voluptates et mollitia omnis distinctio voluptatum repellendus possimus animi pariatur suscipit ut. Soluta doloribus fuga qui quidem aliquid magni.</p>
        </div>
        
        <div class="service">
            <h3>E-Comerce</h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Alias corrupti quia laudantium ipsa rerum quidem deleniti officiis, laboriosam quasi autem nisi! Deserunt mollitia quia voluptatem, accusantium temporibus fugiat. Consectetur, fuga.</p>
        </div>
        
        <div class="service">
            <h3>Refactoring / Debugging</h3>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat hic possimus autem nulla quasi, id ex impedit natus sequi debitis quae officia nihil pariatur quo nesciunt cum quos libero culpa.</p>
        </div>
    </div>
    
    <a href="#projects" class="btn">See My Projects</a>
</section>

<style>
    .my-services {
        background-color: var(--clr-dark);
        color: var(--clr-light);
        text-align: center;
    }

    .section__title--services {
        color: var(--clr-label);
        position: relative;
    }

    .section__title--services::after {
        content: '';
        display: block;
        width: 2em;
        height: 1px;
        margin: 0.25em auto 1em;
        background: var(--clr-light);
        opacity: 0.25;
    }

    .service {
        max-width: 500px;
        margin: 0 auto;
    }

    .services {
        margin-bottom: 3em;
    }

    .btn {
        display: inline-block;
        padding: .5em 2.5em;
        background: var(--clr-label);
        color: var(--clr-dark);
        text-decoration: none;
        cursor: pointer;
        font-size: .8rem;
        text-transform: uppercase;
        letter-spacing: 2px;
        font-weight: var(--fw-bold);
        transition: transform 200ms ease-in-out;
        border-radius: 3px;
    }

    .btn:hover {
        transform: scale(1.1);
    }

    .btn:active {
      color: var(--clr-light);
    }

    @media (min-width:768px) {
        .services {
            display: flex;
            max-width: 1000px;
            margin-right: auto;
            margin-left: auto;
        }
        .service + .service {
            margin-left: 2em;
        }
    }
</style>