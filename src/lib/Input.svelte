<script>
    export let typeText = 'text';
    export let placeholder = '';
    export let title = '';
</script>

<div class="input">
    <label for="">{title}</label>
    <input class="personalizedInput" type={typeText} placeholder={placeholder}>
</div>

<style>
    .input{
        display: flex;
        width: 100%;
        justify-content: left;
        align-items: flex-start;
        flex-wrap: wrap;
        gap: 8px;
    }

    label {
        width: 100%;
        text-align: left;
        font-size: 18px;
        color: #656060;
    }

    input{
        width: 100%;
        height: 40px;
        border: none;
        border-radius: 5px;
        padding: 0 8px;
        font-size: 14px;
        background-color: var(--color-gris);
        opacity: 0.38;
        color: var(--color-grisFuerte);
    }
</style>