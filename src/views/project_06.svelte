<script>
    import Footer from '../lib/Footer.svelte'
    import ProjectCard from '../lib/ProjectCard.svelte'

    let props = {
        title: 'My',
        titleBold: 'Recipes',
        subtitle: 'Web app to look for recipes',
        pic: '../src/assets/imgs/06.png' ,
        p1: 'Full-Stack Web App',
        // picBody: '../' ,
        p2: '(What do i learn and how it went to do this project?)',
        p3: 'You Are Wellcome to play the <a href="" >live demo</a> and take a look at the <a href="">repository</a>',
    }
</script>

<ProjectCard {...props}/>
<Footer />