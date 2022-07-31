<footer>
    <a href="mailto:IngGarciaRodrigoArt@gmail.com" class="footer__link">Hello@IngRoy.com</a>

    <ul class="social-list">
        <li class="social-list__item">
            <a class="social-list__link" href="https://github.com/LastGentlman">
                <i class="fa-brands fa-github"></i>
            </a>
        </li>
        <li class="social-list__item">
            <a class="social-list__link" href="https://www.twitter.com/1ngRoy">
                <i class="fa-brands fa-twitter"></i>
            </a>
        </li>
        <li class="social-list__item">
            <a class="social-list__link" href="https://www.linkedin.com/in/IngRoy">
                <i class="fa-brands fa-linkedin"></i>
            </a>
        </li>
        <li class="social-list__item">
            <a class="social-list__link" href="https://www.instagram.com/1ngroy">
                <i class="fa-brands fa-instagram"></i>
            </a>
        </li>
        <li class="social-list__item">
            <a class="social-list__link" href="https://www.youtube.com/channel/UC7HAWuPFULMnigoHHp6EOmA">
                <i class="fa-brands fa-youtube"></i>
            </a>
        </li>
    </ul>
</footer>

<style>
    footer {
        background: #111;
        color: var(--clr-label);
        text-align: center;
        padding: 2.5em 0;
        font-size: var(--fs-h3);
    }

    footer a {
        color: inherit;
        text-decoration: none;
    }

    .footer__link {
        font-weight: var(--fw-bold);
    }

    .social-list {
        display: flex;
        justify-content:center;
        margin: 0.25em 0;
    }

    .social-list__link {
        padding: .3em;
    }

    .footer__link:hover, .social-list__link:hover {
        opacity: .7;
    }

    .footer__link:hover {
        text-decoration: underline;
    }
</style>