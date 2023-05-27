<script lang="ts">
    export let title: string;
    export let description: string;
    export let src: string;
    export let alt: string;

    interface Icon {
        iconClass: string;
        href: string;
        title: string;
    }

    export let icons: Icon[]; // icon class: href
</script>

<div id="container">
        <img {src} {alt} />

        <div id="text">
            <h3>{title}</h3>
            <p>{description}</p>

        </div>

        <br>

        <div id="icons">
            {#each icons as icon}
                <a title="{icon.title}" href="{icon.href}"><i class="{icon.iconClass}"></i></a>
            {/each}
        </div>

</div>

<style>
    #container {
        border: 1px solid var(--color-light-grey);
        border-radius: 10px;
    }

    #text {
        padding: 10px;
    }
    
    #icons {
        display: flex;
        justify-content: center;
        align-items: center;
        padding-bottom: .4em;
    }

    #icons a {
        padding: .4rem;
    }

    img {
        display: block;
        border-radius: 10px 10px 0 0;
        width: 100%;
        max-height: 10em;
        min-height: 10em;
        object-fit: cover;
    }

    a {
        display: block;
        color: white;
        text-decoration: none;
    }

    a:hover {
        color: var(--color-accent);
        transition: 0.2s ease-in-out; 
    }
</style>