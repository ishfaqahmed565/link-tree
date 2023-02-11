<script setup>
	let account = {
		mainBg: "salman_sadi-bg",
		profileImg: "salman_sadi",
		textColor: "text-[#710439]",
		linkStyle:
			"bg-cyan-100/[.5] shadow-[0_2px_20px_0px_rgba(234,12,127,0.320)] hover:shadow-[0_2px_20px_2px_rgba(234,12,127,0.365)] hover:scale-[1.03]",
		socials: [
			{
				name: "Course",
				link: "https://10minuteschool.com/skills/courses/109/communication-masterclass-by-tahsan-khan/?aff=V2UNK00006f33&utm_medium=affiliation&utm_source=28467&utm_campaign=2_CommunicationMasterclassbyTahsanKhan&utm_content=SkillDevelopment&type=affiliate",
				svg: "book",
			},
			{
				name: "Youtube",
				link: "https://www.youtube.com/@salmansadii",
				svg: "youtube",
			},
			{
				name: "Instagram",
				link: "https://www.instagram.com/salmansadii/",
				svg: "instagram",
			},

			{
				name: "Facebook",
				link: "https://www.facebook.com/salmansadii",
				svg: "facebook",
			},
			{
				name: "Tiktok",
				link: "https://www.tiktok.com/@salmansadii",
				svg: "tiktok",
			},
		],
	};
</script>
<template>
	<Linktree :account="account">
		<template #title> @salmansadii </template>
		<template #second-title>Caution: You might get addicted!! </template>
	</Linktree>
</template>
