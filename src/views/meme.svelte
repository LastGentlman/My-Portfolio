<script>
    import Footer from '../lib/Footer.svelte'
    import ProjectCard from '../lib/ProjectCard.svelte'

    let props = {
        title: 'My',
        titleBold: 'Meme Generator',
        subtitle: 'Web App to Create Memes',
        pic: '../src/assets/imgs/03.png' ,
        p1: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste rem porro ab hic id consequuntur sequi deserunt repudiandae ducimus, mollitia doloribus harum est tenetur similique numquam culpa ipsum! Sit, officiis!',
        // picBody: '../' ,
        p2: '(What do i learn and how it went to do this project?)',
        p3: 'You Are Wellcome to play the <a href="" >live demo</a> and take a look at the <a href="">repository</a>',
    }
</script>

<ProjectCard {...props}/>
<Footer />