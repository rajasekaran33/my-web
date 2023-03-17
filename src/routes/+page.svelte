<script lang="ts">
	import { text } from "svelte/internal";

	// my skill set
	const skills = ['Teach', 'Talk', 'Programming'];
	const links = [
		{
			name: 'Facebook',
			url: 'https://facebook.com',
            icon:'https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Facebook_Logo_%282019%29.png/1024px-Facebook_Logo_%282019%29.png'
		},
		{
			name: 'LinkedIn',
			url: 'https://linkedin.com',
            icon: 'https://cdn4.iconfinder.com/data/icons/social-media-icons-the-circle-set/48/linkedin_circle-512.png'
		}
	];
</script>

<div class="p-4 space-y-3">
	<!-- svelte-ignore a11y-img-redundant-alt -->
	<img
		class='rounded-full w-32 h-32 border-4 border-red-600 shadow-2xl'
		src='https://avatars.githubusercontent.com/u/6880254?v=4'
		alt='image of rajasekaran'
	/>
	<h1 class='text-black text-3xl font-semibold'>Rajasekaran S</h1>
	<p class='text-gray-500'>I am a professor</p>
</div>

<div class='w-fit hover:cursor-pointer hover:bg-yellow-600 rounded-xl bg-red-200 p-6 flex flex-col space-y-5'>
    <div class="space-y-2">
    <img
    class='rounded-lg border-4 w-16 h-16 shadow-2xl'
    src='https://avatars.githubusercontent.com/u/6880254?v=4'
    alt='image of rajasekaran'
/>
<h5 class='text-lg font-medium'>Jhon Wick</h5>
<a class='text-gray-500' href="https://linkedin.com">https://linkedin.com</a>
    </div>
    <button class='w-fit bg-blue-500 text-white px-3 py-[1.5px] rounded-lg'>Support</button>
</div>

{#each skills as item}
	<p>{item}</p>
{/each}
{#each links as item}
	<h5>{item.name}</h5>
	<a href={item.url}>{item.url}</a>
{/each}
