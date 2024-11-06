<script>
    import "../../public/main.css";
    import Nav from "../../component/Nav.svelte";
    import Card from "../../component/Card.svelte";
    let events = [{
        "title": "Business Events",
        "desc" : "Explore insights into the world of business, networking, and innovation.",
        "link" : "https://docs.google.com/forms/d/e/1FAIpQLScJzDO0MyrJQVtvmCkiVpC_OfH1da4TCWQiCck2Z1UYyqfYGQ/viewform",
    },{
        "title": "Technical Events",
        "desc" : "Dive into the latest tech trends and advancements with hands-on experiences.",
        "link" : "/event/engineering",
    },{
        "title": "Psychology Events",
        "desc" : "Gain understanding and insights into human behavior and mental wellness.",
        "link" : "/event/pscyh",
    },{
        "title": "Cultural Events",
        "desc" : "Celebrate diversity through art, music, and traditions from around the world.",
        "link" : "/event/arch",
    },{
        "title": "Debate",
        "desc" : "Engage in thought-provoking debates and sharpen your persuasive skills.",
        "link" : "/event/arch",
    },
    {
        "title": "Design Events",
        "desc" : "Unleash creativity with workshops and challenges in various design fields.",
        "link" : "/event/arch",
    },
    {
        "title": "Accommodation",
        "desc" : "Convenient and comfortable lodging options for event attendees.",
        "link" : "/event/arch",
    }]
</script>

<div class="about-div">
    <div class="bg-bubble"></div>
    <Nav />
    <div class="about-info">
        <h1>
            Our Events
        </h1>
        <!-- Brochure download link -->
        <div class="brochure-link">
            <a href="src/assets/magnovite brochure.pdf" download="Event_Brochure.pdf" class="download-btn">
                Click here for Brochure
            </a>
        </div>
        <div class="brochure-link" style="margin-top: -3rem;">
            <a href="https://linktr.ee/magnovite24christkengeri"  class="download-btn" >
                Register now
            </a>
        </div>
        <p>
            Welcome! Register now to secure your spot at our upcoming events. Don’t miss out on unique experiences designed for learning, enjoyment, and connection. Select your event below and register today!
        </p>
        <div class="about-grid">
            {#each events as event}
                <Card title={event.title} description={event.desc} link={event.link} />
            {/each}
        </div>
       
       
    </div>
</div>