+++
template = "homepage.html"
+++

<style>
    .home {
        font-family: monospace;
    }

    .hero-title {
        font-size: 3rem;
    }

    p {
        font-size: 1.2rem;
        text-align: justify;
    }

    .intro {
        display: inline;
    }

    .highlight, .exp {
        color: var(--primary-color);
    }

    .hire {
        color: white;
        font-size: 1.2rem;
        background-color: var(--primary-color);
    }

    @media screen and (max-width: 768px) {
        p {
            font-size: 1.2rem;
            text-align: left;
        }
        .intro {
            display: block;
        }
    }
</style>

<div class="home">
    <p class="hero-title">
        Hello,
        <span class="intro">I'm <span class="highlight">Y (Wai).</span></span>
    </p>
    <p>
        I'm a fullstack engineer based in Thailand with over <span
            class="exp">seven years</span> of experience in building effective
        user interfaces and performant systems.
    </p>
    <p>
        My expertise lies in designing robust frontend systems in <span
            class="highlight">React</span>, and architecting scalable API platforms
        with languages such as <span class="highlight">Go</span>, <span
            class="highlight">Java</span>, and <span class="highlight">Python</span>.
    </p>
    <p>
        I'm a fan of strongly-typed languages, neovim enthusiast and a staunch supporter of
        hand-crafted software that is <span class="highlight">built to last.</span>
    </p>
    <span class="hire">I'm available for hire!</span>
</div>
