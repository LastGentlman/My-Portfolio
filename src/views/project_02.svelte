<script>
    import Footer from '../lib/Footer.svelte'
    import ProjectCard from '../lib/ProjectCard.svelte'

    let props = {
        title: 'My title',
        titleBold: 'of my Project',
        subtitle: 'Short Subtitle',
        pic: '../src/assets/imgs/02.png' ,
        p1: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste rem porro ab hic id consequuntur sequi deserunt repudiandae ducimus, mollitia doloribus harum est tenetur similique numquam culpa ipsum! Sit, officiis!',
        // picBody: '../' ,
        p2: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nisi corporis optio eligendi harum, deleniti eveniet sit nesciunt impedit distinctio facilis necessitatibus vero deserunt dolores, id illum quos, quibusdam ipsa consectetur.',
        p3: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe tempora quidem harum nulla voluptates quae iusto. Iure ipsam, nesciunt omnis, recusandae, est obcaecati tempore ex aperiam et voluptatibus vitae. Earum!',
    }
</script>

<ProjectCard {...props}/>
<Footer />