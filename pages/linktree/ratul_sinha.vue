<script setup>
	let account = {
		mainBg: "ratul_sinha-bg",
		profileImg: "ratul_sinha",
		textColor: "",
		linkStyle:
			"bg-gradient-to-t from-black/[.80] to-[#4998CA]  shadow-[0_2px_10px_0px_rgba(73,152,202,0.320)] hover:shadow-[0_2px_15px_2px_rgba(73,152,202,0.365)] hover:scale-[1.03]",
		socials: [
			{
				name: "Youtube",
				link: "https://www.youtube.com/@itsratulsinha",
				svg: "youtube",
			},
			{
				name: "Instagram",
				link: "https://www.instagram.com/itsratulsinha/",
				svg: "instagram",
			},
			{
				name: "Facebook",
				link: "https://www.facebook.com/itsratulsinha",
				svg: "facebook",
			},
			{
				name: "Twitter",
				link: "https://twitter.com/itsratulsinha",
				svg: "twitter",
			},
			{
				name: "Gmail",
				link: "ratulsinha.work@gmail.com",
				svg: "mail",
			},
		],
	};
</script>
<template>
	<Linktree :account="account">
		<template #title> @itsratulsinha </template>
		<template #second-title
			>Don't follow my socials! You might fall in love UwU!
		</template>
	</Linktree>
</template>
<style scoped>
	.gh {
		color: rgb(73, 152, 202);
	}
</style>
