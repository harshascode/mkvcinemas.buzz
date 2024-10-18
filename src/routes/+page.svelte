<script>
	import Head from '$lib/components/layout/Head.svelte';
	import Blogs from '$lib/components/Blogs.svelte';
	import Middlebox from '$lib/components/Middlebox.svelte';

	export let data;
	let posts = data.posts;
</script>

<Head />

<Middlebox />
<div class="pt-12">
	<h1
		class="pb-6 text-3xl font-extrabold leading-9 tracking-tight text-gray-900 dark:text-gray-100 sm:text-4xl sm:leading-10 md:text-6xl md:leading-14"
	>
		Welcome to Mkvcinemas
	</h1>
	<p class="text-base prose-base text-gray-800 dark:text-gray-100">
		Looking for the latest HD-quality Mkv cinemas? MkvCinemas provides information on where to
		stream or download movies, TV shows, and web series through free or popular paid platforms. You
		can access content in multiple languages, including Tamil, Telugu, Hindi, English, Malayalam,
		Kannada, Marathi, and Odia, all conveniently available through the Mkvcinemas web app.
	</p>
</div>

<Blogs title="Latest Posts" h2 {posts} search={false} count={15} />

