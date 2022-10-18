<script>
    import Footer from '../lib/Footer.svelte'
    import ProjectCard from '../lib/ProjectCard.svelte'

    let props = {
        title: 'My',
        titleBold: 'Brilliant Idea',
        subtitle: 'app like story book but for ideas',
        pic: '../src/assets/imgs/05.png' ,
        p1: 'Project created with ',
        // picBody: '../' ,
        p2: '(What do i learn and how it went to do this project?)',
        p3: 'You Are Wellcome to use it <a href="" >live demo</a> and take a look at the <a href="">repository</a>',
    }
</script>

<ProjectCard {...props}/>
<Footer />