<script setup>
	let props = defineProps({
		account: { type: Object, required: true },
	});
</script>
<template>
	<div class="main">
		<div class="absolute w-full h-full">
			<img
				:src="`/images/background/${props.account.mainBg}.jpg`"
				alt=""
				class="object-cover w-full h-full"
			/>
		</div>
		<div
			class="py-4 max-w-3xl px-5 flex flex-col justify-center items-center gap-5 mx-auto relative z-[50]"
		>
			<div class="grid gap-4 place-items-center mb-2">
				<img
					:src="`/images/profileImg/${props.account.profileImg}.jpg`"
					alt=""
					class="w-[6rem] rounded-full"
				/>
				<h1 :class="`text-white text-xl font-bold ${props.account.textColor}`">
					<slot name="title"></slot>
				</h1>
				<p
					:class="`text-white text-lg font-semibold ${props.account.textColor}`"
				>
					<slot name="second-title"></slot>
				</p>
			</div>
			<NuxtLink
				class="w-full flex flex-col gap-4"
				target="”_blank”"
				v-for="(social, index) in props.account.socials"
				:key="social.link"
				:to="social.link"
			>
				<div
					:class="` ${
						index == 0 ? 'animate-bounce' : ''
					} w-full pr-7 flex item-center rounded-full text-base text-bold text-gray-400 hover:scale-[1.03] p-3 font-semibold shadow-1 transition-all duration-900 ${
						props.account.linkStyle
					}`"
				>
					<Svgs :name="social.svg" />
					<p
						:class="`pt-1 w-full text-center text-center font-semibold text-white text-lg ${props.account.textColor} `"
					>
						{{ social.name }}
					</p>
				</div>
			</NuxtLink>
		</div>
	</div>
</template>
<style scoped>
	/** .main {
		background-image: url("/images/rafsan_bg.jpg");
	}**/
</style>
