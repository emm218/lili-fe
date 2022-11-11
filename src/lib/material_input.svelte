<script>
	export let name
	export let label
</script>

<div class="my-[16px]">
<label for={name} class="text-sm">{label}</label>
<div class="relative">
	<div class="absolute 
		left-0 
		top-0 
		z-10 p
		pl-[12px] 
		pr-[16px] 
		flex 
		items-center 
		h-full 
		w-[52px] 
		leading-none 
		justify-center"
	>
		<slot name="prefix">
		</slot>
	</div>
	<input type="text" {name} class="pl-[52px] bg-surface0 rounded-[4px] border-overlay1 focus:border-mauve">
</div>
</div>
<style>
	input:valid::placeholder {
		visibility: visible !important;
	}
</style>
