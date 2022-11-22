<template>
	<button @click="onClick()"
	:style="{background:color}"
	v-bind:class="btn"
	>
		{{text}}
	</button>
</template>

<script>
export default {
	name: 'Button',
	props: {
		text: {
			type: String,
			default: 'Add Task',
			required: true
		},
		color: {
			type: String,
			default: 'green'
		}
	},
	methods: {
		onClick() {
			this.$emit('click')
		}
	}
};

</script>
