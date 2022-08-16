<script>
    import Footer from '../lib/Footer.svelte'
    import ProjectCard from '../lib/ProjectCard.svelte'

    let props = {
        title: 'My',
        titleBold: 'Weather App',
        subtitle: 'Weather Aplication',
        pic: 'https://raw.githubusercontent.com/LastGentlman/My-Portfolio/main/src/assets/imgs/weatherPic.png' ,
        p1: 'Project created with ReactJS I use the <a href="http://weatherapi.com">weatherapi</a> to use geolocaltion with google maps, with Micro-Front Ends and Behavior Driven Development Methodology',
        picBody: 'https://raw.githubusercontent.com/LastGentlman/My-Portfolio/main/src/assets/imgs/weather.png' ,
        p2: `With this project, I Learned About: <br/>
            &emsp;-The creation and implementation of CSS Loading <br/>
            &emsp;-Using Geolocation with google maps <br/>
            &emsp;-API data manipulation`,
        p3: 'You are Wellcome to see the <a href="http://https://myweatherapp.up.railway.app/">Live Demo</a> and <a href="http://https://github.com/LastGentlman/My-Weather-App">The GitHub Repo</a> of this project',
    }
</script>

<ProjectCard {...props}/>
<Footer />