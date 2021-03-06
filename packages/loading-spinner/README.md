# LoadingSpinner

A component that renders an animated spinner circle next to a "Loading..." or a custom text.

## Installation

```
npm install @reciprocity/loading-spinner
```
or
```
yarn add @reciprocity/loading-spinner
```

## Usage

This component is meant to be used as an ES module, so you can import it using the ES6 `import` syntax.

After importing you can just register it with Vue. Eg:

app.vue

```vue
<template>
	<loading-spinner text="Downloading..." />
</template>
<script>
	import LoadingSpinner from '@reciprocity/spinner';

	export default Vue.extend({
		name: 'My App',
		components: {
			LoadingSpinner
		}
	};
</script>
```
