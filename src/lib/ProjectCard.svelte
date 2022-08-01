<script>
    export let title = "The Title";
    export let titleBold = "of My Project";
    export let subtitle = "Subtitle of project";
    export let pic = "../src/assets/imgs/01.png";
    export let p1 = "First Paragraph";
    export let picBody = "../src/assets/imgs/01-01.jpg"
    export let p2 = "Second Paragraph";
    export let p3 = "Third Paragraph";
</script>

<section class="intro" id="home">
    <h1 class="section__title section__title--intro">
        {title} <strong>{titleBold}</strong>
    </h1>
    <p class="section__subtitle section__subtitle--intro">{subtitle}</p>
    <img class="pic" src={pic} alt="" />
</section>

<main>
    <p>{p1}</p>
    
    <img src={picBody} alt="" />
    
    <p>{p2}</p>
    
    <p>{p3}</p>
</main>

<style> 
    .intro {
        position: relative;
    }
    
    .section__subtitle--intro {
        display: inline-block;
    }
    
    .pic {
        box-shadow: var(--shadow);
        width: 249px;
        height: 249px;
    }

    img {
        display: block;
        max-width: 100%;
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

        .pic {
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

    main {
        padding: 0 2em 2em;
        max-width: 1000px;
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        gap: 0.75em;
    }

    main p {
        max-width: 600px;
        margin-left: auto;
        margin-right: auto;
    }

</style>