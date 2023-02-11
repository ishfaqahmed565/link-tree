<script setup>
	let account = {
		mainBg: "jubaer_talukdar-bg",
		profileImg: "jubaer_talukdar",
		textColor: "text-[#112A46]",
		linkStyle:
			"bg-gradient-to-t from-[#D2D5DF]/[.80] to-[#FFF8D9]/[.80] shadow-[0_2px_20px_0px_rgba(234,12,127,0.320)] hover:shadow-[0_2px_20px_2px_rgba(234,12,127,0.365)] hover:scale-[1.03]",
		socials: [
			{
				name: "Youtube",
				link: "https://www.youtube.com/@JubaerTalukder",
				svg: "youtube",
			},
			{
				name: "Instagram",
				link: "https://www.instagram.com/films.by.jubaer/",
				svg: "instagram",
			},
			{
				name: "Tiktok",
				link: "https://www.tiktok.com/@jubaer_talukder",
				svg: "tiktok",
			},
			{
				name: "Facebook",
				link: "https://www.facebook.com/jubaer.talukder.5",
				svg: "facebook",
			},
			{
				name: "Linked In",
				link: "https://www.linkedin.com/in/jubaer-talukder-48b3a1195/",
				svg: "linked_in",
			},
		],
	};
</script>
<template>
	<Linktree :account="account">
		<template #title> @films.by.jubaer </template>
		<template #second-title>The guy with a camera!</template>
	</Linktree>
</template>
