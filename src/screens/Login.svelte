<script>
    import Button from "../lib/Button.svelte";
    import Toggle from "../lib/Toggle.svelte";
    import Input from "../lib/Input.svelte";
</script>

<main>

    <div class="login">
        <h1>TecniMotor</h1>
        <img src="../../public/img/logo.png" alt="Logo">
        <p>Inicio de sesión</p>
    </div>

    <div class="loginFormulario">
        <div class="inputCont">
            <Input typeText="text" placeholder="correo@gmail.com" title="Email"/>
            <Input typeText="password" placeholder="contraseña" title="Contraseña"/>
        </div>
        <a class="forgot" href="">¿Olvidaste la contraseña?</a>
        <Button/>
        <div class="rememberMe">
            <p>Recuérdame</p>
            <Toggle />
        </div>
    </div>

</main>

<style>

    main {
        height: 680px;
        width: 350px;
        background-color: white;
        color: black;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        border: 3px solid black;
        border-radius: 10px;
        padding: 10px;
    }

    .arrowBtnCont {
        width: 100%;
        align-items: start;
        display: flex;
        justify-content: start;
        margin-top: 50px;
    }

    .login {
        width: 100%;
        height: 35%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 25px;   
        margin-top: 30px;
    }

    img{
        width: 180px;
    }

    h1 {
        width: 100%;
        font-size: 40px;
    }

    p {
        width: 100%;
        font-size: 22px;
        font-weight: 500;
    }

    .loginFormulario {
        height: 60%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }

    .inputCont {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 25px;
    }

    .forgot {
        width: 100%;
        color: var(--color-azul);
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .rememberMe {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-top: 20px;
    }

    .rememberMe p {
        width: fit-content;
        font-size: 18px;
        padding: 0;
    }
</style>
