<section>
    <h1>TisLeo</h1>
    <h2 style="color: white;">Welcome to my <span id="strike">average</span> portfolio!</h2>
    <p id="egg">(can you tell I'm amazing at webdev?)</p>

    <br><br>

    <h3>Hi! My name is Leo, but I go by TisLeo online. 
        I’m currently a computer science student and I love to code small projects in my spare time. I typically
        prefer backend, but I like to dabble in frontend too (sometimes). I know that this portfolio isn’t too large or crazy, but I hope to change that in the future!</h3>    
</section>

<style>
    section {
        margin-top: 2rem;
    }

    @media only screen and (max-width: 640px) {
        section {
            margin-top: 8rem;
        }
    }

    h1 {
        background: linear-gradient(45deg, #1582D0, #6EBBF3);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        font-family: 'Courgette', sans-serif;
        padding: 0 2em 0 2em;
    }

    h2 {
        color: var(--color-accent)
    }

    h3 {
        text-align: center;
    }

    #strike {
        text-decoration: line-through;
    }

    #egg {
        color: var(--color-light-grey);
    }
</style>