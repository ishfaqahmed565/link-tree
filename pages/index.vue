<script setup>
	let socials = [
		{
			name: "Merch",
			link: "https://www.instagram.com/justicebychotobhai/",
			svg: "merch",
		},
		{
			name: "Youtube",
			link: "https://www.youtube.com/@RafsanTheChotobhai",
			svg: "youtube",
		},
		{
			name: "Instagram",
			link: "https://www.instagram.com/thechotobhai/",
			svg: "instagram",
		},
		{
			name: "Facebook",
			link: "https://www.facebook.com/Rafsanthechotobhai",
			svg: "facebook",
		},

		{
			name: "Linked In",
			link: "https://bd.linkedin.com/in/iftekhar-rafsan-633587171",
			svg: "linked_in",
		},
	];
</script>
<template>
	<div class="bg-black main">
		<div class="absolute w-full h-full">
			<img
				src="/images/rafsan_bg.jpg"
				alt=""
				class="object-cover w-full h-full"
			/>
		</div>
		<div
			class="py-4 max-w-5xl px-5 flex flex-col justify-center items-center gap-5 mx-auto relative z-[50]"
		>
			<img src="/images/rafsan_img.jpg" alt="" class="w-[6rem] rounded-full" />
			<h1 class="text-white text-xl font-bold">@thechotobhai</h1>
			<p class="text-white text-lg font-semibold">Follow my socials below:</p>
			<NuxtLink
				class="w-full flex flex-col gap-4"
				target="”_blank”"
				v-for="(social, index) in socials"
				:key="social.link"
				:to="social.link"
			>
				<div
					class="bg-gradient-to-r from-[#FFB802] to-[#DA158A] w-full pr-7 flex item-center rounded-full text-base text-bold text-gray-400 p-3 font-semibold shadow-1 transition-all duration-900"
					:class="{ 'animate-bounce': index == 0 }"
				>
					<Svgs :name="social.svg" />
					<p
						class="pt-1 w-full text-center uppercase text-center font-semibold text-white text-lg"
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
	.shadow-1 {
		box-shadow: #ea0c7f70 0px 2px 20px 1px;
		transform: scale(1);
	}
	.shadow-1:hover {
		box-shadow: #ea0c7f5d 0px 2px 20px 6px;
		transform: scale(1.03);
	}
</style>
