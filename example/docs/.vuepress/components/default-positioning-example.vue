<script>
import { Cropper } from 'vue-advanced-cropper';
import ExampleWrapper from './Components/ExampleWrapper';

export default {
	components: {
		Cropper,
		ExampleWrapper,
	},
	data() {
		return {
			img:
				require('../assets/pictures/photo-1527199372136-dff50c10ea34.jpg'),
		};
	},
	methods: {
		defaultPosition() {
			return {
				left: 100,
				top: 100,
			};
		},
		defaultSize() {
			return {
				width: 400,
				height: 400,
			};
		},
	},
};
</script>
<template>
	<example-wrapper
		href="https://github.com/advanced-cropper/vue-advanced-cropper/blob/master/example/docs/.vuepress/components/default-positioning-example.vue"
	>
		<cropper :src="img" :default-position="defaultPosition" :default-size="defaultSize" />
	</example-wrapper>
</template>
