<script>
	import Button from "../utils/Button.svelte";
	import Separator from "../utils/Separator.svelte";
	import Input from "../Form/Input.svelte";
	import Select from "../Form/Select.svelte";
	import Textarea from "../Form/Textarea.svelte";
	import Checkbox from "../Form/Checkbox.svelte";
	import Radio from "../Form/Radio.svelte";
	import Card from "../utils/Card.svelte";
</script>

<main>
	<div class=" flex justify-center min-h-screen bg-gray-200">
		<div class=" bg-white shadow-xl min-h-full w-full md:w-10/12 lg:w-3/4 xl:w-2/3 2xl:w-1/2">
			<div class="p-10 text-center">
				<div class="text-4xl font-sans antialiased tracking-wider">
					<span class="font-extrabold underline">Twój</span>
					<strong class="text-indigo-600  ">panel administracyjny</strong>
				</div>
				<div class="my-5 antialiased">
					zbudowany za pomocą <strong>Tailwind CSS</strong> i <strong>Svelte</strong> <br/>
					na podstawie książki <em>Tailwind CSS. Projektowanie stron WWW i podejście utility-first</em>, <br/>
					wydanej nakładem wydawnictwa Helion
				</div>

				<Separator/>

				<div class="p-10 mb-5">
					<div class="flex flex-col">
						<h2 class="text-3xl">Nasze przyciski</h2>
						<div class="text-center my-5">
							<Button className={""} tekst={"Przycisk bazowy"}/>
						</div>
						<div class="grid grid-cols-2 md:grid-cols-3 xl:grid-cols-5 gap-2">
							<Button className={"success"} tekst={"Zapisz"}/>
							<Button className={"danger"} tekst={"Usuń"}/>
							<Button className={"info"} tekst={"Zobacz"}/>
							<Button className={"primary"} tekst={"Edytuj"}/>
							<Button className={"warning"} tekst={"Sprawdź"}/>
						</div>
					</div>
				</div>

				<Separator/>

				<div class="p-10 my-5">
					<div class="flex flex-col">
						<h2 class="text-3xl mb-5">Pola formularza</h2>

						<div class="grid grid-cols-1 gap-4 text-left">
							<Input type={"text"} label={"Pole tekstowe"} placeholder={"Wprowadź krótki tekst"}/>
							<Select label={"Lista rozwijana"} options={[
								{value: "pierwsza", option: "Pierwsza opcja"},
								{value: "druga", option: "Druga opcja"},
								{value: "trzecia", option: "Trzecia opcja"}
							]}/>
							<Textarea label={"Pole tekstu rozszerzonego"} placeholder={"Wprowadź długi tekst"}/>
							<Checkbox name={"checkbox"} label={"Wybierz tę opcję"}/>
							<Radio name={"radio"} label={"Zaznacz tę opcję"}/>
						</div>
					</div>
				</div>

				<Separator/>

				<div class="p-10 my-5">
					<Card title={"Sprawdź nasz szablon"}>
						<div class="flex justify-center space-x-2">
							<Button className={"success"} tekst={"Zaloguj się"}/>
							<Button className={"primary"} tekst={"Zarejestruj"}/>
						</div>
					</Card>
				</div>
			</div>
		</div>
	</div>
</main>
