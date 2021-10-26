<script>
	import { page } from '$app/stores';
</script>

<header>

	<nav class="navbar">

	
	<ul class="nav nav-tabs w-100">
		<li class="nav-item">
		  <a class="nav-link"  class:active={$page.path === '/'} aria-current="page" href="/">KH/TB</a>
		</li>
		<li class="nav-item">
		  <a class="nav-link"  class:active={$page.path === '/danhmuc'} href="/danhmuc">Danh mục</a>
		</li>
	</ul>
	</nav>

</header>