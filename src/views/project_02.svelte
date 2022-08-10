<script>
    import Footer from '../lib/Footer.svelte'
    import ProjectCard from '../lib/ProjectCard.svelte'

    let props = {
        title: 'My',
        titleBold: 'Paint Board',
        subtitle: 'Short Subtitle',
        pic: '../src/assets/imgs/02.png' ,
        p1: 'Web App created using only JavaScript, HTML and CSS',
        // picBody: '../' ,
        p2: 'It Was a fun and interesting proyect, you can paint and create pixel art like portraits',
        p3: 'You Are Wellcome to play the <a href="https://lastgentlman.github.io/ETCH-A-SKETCH/" >live demo</a> and take a look at the <a href="http://https://github.com/LastGentlman/ETCH-A-SKETCH">repository</a>',
    }
</script>

<ProjectCard {...props}/>
<Footer />