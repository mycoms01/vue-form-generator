<template lang="jade">
	.wrapper
		input(type="color", v-model="value", :autocomplete="schema.autocomplete", :disabled="disabled", :name="schema.inputName")
		span.helper {{ value }}
</template>

<script>
	import abstractField from "./abstractField";
	export default {
		mixins: [ abstractField ]
	};
</script>


<style lang="sass">
	.vue-form-generator .field-color {

		input {
			width: 60px;
		}

		.helper {
			margin-left: 0.3em;
		}
	} 
</style>
