<script lang="ts">
	// my skill set
	const skills = ['Teach', 'Talk', 'Programming'];
	const links = [
		{
			name: 'Facebook',
			url: 'https://facebook.com'
		},
		{
			name: 'LinkedIn',
			url: 'https://linkedin.com'
		}
	];
</script>

<img src="https://avatars.githubusercontent.com/u/6880254?v=4" alt="image of rajasekaran" />
<h1>Rajasekaran S</h1>
<p>I am a professor</p>
{#each skills as item}
	<p>{item}</p>
{/each}
{#each links as item}
	<h5>{item.name}</h5>
	<a href={item.url}>{item.url}</a>
{/each}

<style>
    h1{
        color: blue;
    }
</style>