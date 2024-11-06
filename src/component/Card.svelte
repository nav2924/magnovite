<script>
    export let title = '';
    export let description = '';
    export let link = '#';
</script>
<div class="card-component">
    <h2>{title}</h2>
    <p>{description.length > 100 ? description.slice(0, 100) + '...' : description}</p>
    <span aria-label="{link}"><button style="
        margin-top: 1rem;
        border-radius: 2rem; 
        background-color: #4CAF50; 
        color: white; 
        padding: 10px 20px; 
        font-size: 1rem;
        border: none;
        cursor: pointer;"><a href="https://linktr.ee/magnovite24christkengeri">Register now</a></button></span>
</div>