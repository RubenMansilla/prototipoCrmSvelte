<script>
    let isActive = false;

    function toggle() {
        isActive = !isActive;
    }
</script>

<style>
    .toggleBtn {
        width: 70px;
        background-color: #ffffff;
        border-radius: 25px;
        padding: 3px;
        border: 1.6px solid black;
        outline: none;
    }
    .toggleBtn__sphere {
        height: 25px;
        aspect-ratio: 1/1;
        background-color: var(--color-azul);
        border-radius: 100%;
        transition: all 0.3s ease;
    }
    .toggleBtn.isActive .toggleBtn__sphere {
        transform: translateX(35px);
        background-color: white;
        
    }
    .toggleBtn.isActive  {
        background-color: var(--color-azul);
        
    }
</style>

<button class="toggleBtn" on:click={toggle} class:isActive>
    <div class="toggleBtn__sphere"></div>
</button>
