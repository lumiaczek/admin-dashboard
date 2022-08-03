<script>
    import Logo from "../../components/utils/Logo.svelte";
    import Separator from "../../components/utils/Separator.svelte";
    import Button from "../../components/utils/Button.svelte";
    import Input from "../../components/form/Input.svelte";
</script>

<div class="flex items-center justify-center min-h-screen bg-blue-900 flex-column">

    <div>
        <div class="w-full flex justify-center">
            <Logo/>
        </div>
        <div class="w-full mt-3">
            <form action="" class="overflow-hidden bg-white rounded-lg shadow-xl">
                <div class=" px-10 pt-8 pb-6 text-center ">
                    <h1 class="text-xl font-bold">
                        Zarejestruj się
                    </h1>
                    <h2 class="text-xl">
                        w panelu <strong>administracyjnym</strong>
                    </h2>
                    <Separator/>
                    <div class="flex flex-col space-y-4 text-left">
                        <Input label={"Login"} class={"border px-3 py-2 rounded-lg w-full "}/>
                        <Input label={"Email"} type={"email"} class={"border px-3 py-2 rounded-lg w-full "}/>
                        <Input label={"Hasło"} type={"password"} class={"border px-3 py-2 rounded-lg w-full "}/>
                        <Input label={"Powtórz hasło"} type={"password_repeat"} class={"border px-3 py-2 rounded-lg w-full "}/>
                    </div>
                </div>
                <footer class=" flex items-center justify-center space-x-2 px-10 py-4 bg-gray-100 border-t border-gray-200">

                    <a href="/admin">
                        <Button className={"success"} tekst={"Zarejestruj"}/>
                    </a>

                    <a href="/auth/Login">
                        <Button className={"info"} tekst={"Masz już konto?"}/>
                    </a>

                </footer>
            </form>
        </div>
    </div>
</div>