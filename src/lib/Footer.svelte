<footer>
    <img src="./src/assets/leo_logo.png" alt="TisLeo Logo">
    <p>© TisLeo 2023</p>
    <br>
    <div id="items">
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="#tech">Tech</a></li>
            <li><a href="#projects">Projects</a></li>
        </ul>
    </div>
</footer>

<style>
    footer {
        background-color: black;
        height: 12rem;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    img {
        border: 2px solid var(--color-light-grey);
        border-radius: 50px;
        height: 4em;
        width: 4em;
    }

    p {
        color: var(--color-light-grey);
    }

    #items li:not(:last-child), #items li:not(:first-child) {
        padding: 0 .5em 0 .5em;
    }

    a {
        display: block;
        color: white;
        text-decoration: none;
        width: 100%;
        height: 100%;
    }

    a:hover {
        color: var(--color-accent);
        transition: 0.2s ease-in-out; 
    }

    li {
        display: inline-block;
    }
</style>