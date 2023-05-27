<script>
    import Card from './Card.svelte';

    const autoMinecartIcons = [
        { iconClass: "fab fa-github", href: "https://github.com/tisleo/AutoMinecart", title: "View on GitHub" },
        { iconClass: "fas fa-globe", href: "https://www.spigotmc.org/resources/autominecart.101327/", title: "View on Spigot"},
        { iconClass: "fas fa-globe", href: "https://hangar.papermc.io/TisLeo/AutoMinecart", title: "View on Hangar"}
    ]

    const boredBotIcons = [
        { iconClass: "fab fa-github", href: "https://github.com/TisLeo/Bored-Bot", title:  "View on GitHub" },
        { iconClass: "fab fa-discord", href: "https://canary.discord.com/api/oauth2/authorize?client_id=959141306205081610&permissions=2147601472&scope=applications.commands%20bot", title: "Invite to Discord"}
    ]

    const mBBIcons = [
        { iconClass: "fab fa-github", href: "https://github.com/TisLeo/More-Beautiful-Buttons-Mod", title: "View on GitHub" },
        { iconClass: "fas fa-globe", href: "https://www.curseforge.com/minecraft/mc-mods/more-beautiful-buttons-fabric", title: "View on CurseForge"},
    ]
</script>

<section id="projects">
    <h2>Projects</h2>
    <p>The good stuff. More to come Soon<span id="tm">TM</span></p>

    <br>

    <div id="cards">
        <Card 
            title="Auto Minecart" 
            description="A useful Minecraft plugin that mimics Terraria minecarts." 
            src="../assets/auto_minecart.png" alt="Auto Minecart plugin logo"
            icons={autoMinecartIcons}
        />
        <Card 
            title="Bored Bot" 
            description="A Discord bot to get something to do when you're bored!" 
            src="./src/assets/bored_bot.png" alt="Bored bot logo"
            icons={boredBotIcons}
        />
        <Card 
            title="More Beautiful Buttons" 
            description="Over 200 vanilla Minecraft blocks craftable into buttons!" 
            src="./src/assets/buttons.png" 
            alt="Minecraft buttons"
            icons={mBBIcons}
        />    
    </div>
</section>

<style>
    #cards {
        gap: 2rem;
        display: flex;
        width: 100%;
        justify-content: space-evenly;
    }

    #tm {
        vertical-align: super;
        color: var(--color-light-grey);
        font-size: .5rem;
    }

    @media only screen and (max-width: 640px) {
        #cards {
            gap: 2rem;
            display: flex;
            flex-direction: column;
            width: 100%;
            justify-content: space-evenly;
        }
    }
</style>