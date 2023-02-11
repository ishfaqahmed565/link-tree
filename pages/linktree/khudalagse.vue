<script setup>
	let account = {
		mainBg: "fahrin_faiza-bg",
		profileImg: "fahrin_faiza",
		textColor: "text-[#710439]",
		linkStyle:
			"bg-purple-200/[.7] shadow-[0_2px_20px_0px_rgba(234,12,127,0.320)] hover:shadow-[0_2px_20px_2px_rgba(234,12,127,0.365)] hover:scale-[1.03]",
		socials: [
			{
				name: "Next Door Faiza",
				link: "https://www.instagram.com/nextdoorfaiza/?hl=en",
				svg: "dress",
			},
			{
				name: "Youtube",
				link: "https://www.youtube.com/@khudalagse",
				svg: "youtube",
			},
			{
				name: "Fahrin Faiza",
				link: "https://www.instagram.com/fahrinfaizaa/?hl=en",
				svg: "instagram",
			},
			{
				name: "Khuda Lagse",
				link: "https://www.instagram.com/khudalagse/?hl=en",
				svg: "instagram",
			},
			{
				name: "Facebook",
				link: "https://www.facebook.com/khudalagse2",
				svg: "facebook",
			},
		],
	};
</script>
<template>
	<Linktree :account="account">
		<template #title> @fahrinfaiza </template>
		<template #second-title>Follow my socials for an adventure! </template>
	</Linktree>
</template>
