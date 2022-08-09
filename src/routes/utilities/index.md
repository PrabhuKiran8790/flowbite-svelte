---
layout: typographyLayout
---

<script>
	import { Htwo, ExampleDiv, GitHubSource, CompoDescription, TableProp, TableDefaultRow} from '../utils'
	import { Breadcrumb, BreadcrumbItem, CloseButton } from '$lib';
	import { Home } from 'svelte-heros';
  export let visible = true;
</script>

<Breadcrumb>
	<BreadcrumbItem href="/" icon={Home} variation="solid">Home</BreadcrumbItem>
	<BreadcrumbItem>Utilities</BreadcrumbItem>
</Breadcrumb>

<h1 class="text-3xl w-full dark:text-white pt-8 pb-4">Utilities</h1>

<Htwo label="CloseButton" />

Use `CloseButton` component to close a component.

<ExampleDiv>
{#if visible}
<div id="banner" tabindex="-1" class="flex z-50 gap-8 justify-between items-start py-3 px-4 w-full bg-gray-50 border border-b border-gray-200 sm:items-center dark:border-gray-700 lg:py-4 dark:bg-gray-800">
    <p class="text-sm font-light text-gray-500 dark:text-gray-400">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorem, ipsa culpa ea laudantium earum quis? Neque unde aliquam enim, distinctio repellendus delectus? Illo numquam ex fugit dolor esse, cumque nesciunt?</p>
    <CloseButton
				on:click={() => (visible = false)}
				class="text-gray-400 hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm p-1.5 dark:hover:bg-gray-600 dark:hover:text-white"
			/>
  </div>
{/if}
</ExampleDiv>

```html
{#if visible}
<div id="banner" tabindex="-1" class="flex z-50 gap-8 justify-between items-start py-3 px-4 w-full bg-gray-50 border border-b border-gray-200 sm:items-center dark:border-gray-700 lg:py-4 dark:bg-gray-800">
    <p class="text-sm font-light text-gray-500 dark:text-gray-400">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorem, ipsa culpa ea laudantium earum quis? Neque unde aliquam enim, distinctio repellendus delectus? Illo numquam ex fugit dolor esse, cumque nesciunt?</p>
    <CloseButton
				on:click={() => (visible = false)}
				class="text-gray-400 hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm p-1.5 dark:hover:bg-gray-600 dark:hover:text-white"
			/>
  </div>
{/if}
```