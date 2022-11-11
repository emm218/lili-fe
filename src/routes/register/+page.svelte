<script>
	import { User, Envelope, LockKey } from "phosphor-svelte"
	import MaterialInput from "../../lib/material_input.svelte"
</script>

<div class="bg-base md:bg-transparent md:fixed md:top-0 md:bottom-0 w-full flex items-center justify-center">
<div class="md:m-auto bg-base md:rounded-[28px] p-[24px] md:drop-shadow-lg">
	<header>
		<h2 class="text-2xl mb-[16px]">Register</h2>
	</header>
	<form>
		<MaterialInput name="username" label="Username">
			<span slot="prefix">
				<User size={24} />
			</span>
		</MaterialInput>
		<MaterialInput name="email" label="Email">
			<span slot="prefix">
				<Envelope size={24} />
			</span>
		</MaterialInput>
		<MaterialInput name="password" label="Password">
			<span slot="prefix">
				<LockKey size={24} />
			</span>
		</MaterialInput>
		<MaterialInput name="password_confirmation" label="Confirm password">
			<span slot="prefix">
				<LockKey size={24} />
			</span>
		</MaterialInput>
		<input type="submit" value="Continue" class="rounded-full bg-mauve hover:bg-[#BA98E3] transition-colors text-crust px-[16px] h-[40px] mt-[24px] float-right">
	</form>
</div>
</div>
