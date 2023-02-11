<script setup>
	let account = {
		mainBg: "enayet_chowdhury-bg",
		profileImg: "enayet_chowdhury",
		textColor: "",
		linkStyle:
			"bg-cyan-200/[.5] shadow-[0_2px_20px_0px_rgba(234,12,127,0.320)] hover:shadow-[0_2px_20px_2px_rgba(234,12,127,0.365)] hover:scale-[1.03]",
		socials: [
			{
				name: "Merch",
				link: "https://madkoffee.com/product/enayet-chowdhury-official-merch/",
				svg: "merch",
			},
			{
				name: "Padma Setu - Book",
				link: "https://www.rokomari.com/book/198113/padma-setu",
				svg: "book",
			},
			{
				name: "Youtube",
				link: "https://www.youtube.com/@EnayetChowdhuryOfficial",
				svg: "youtube",
			},
			{
				name: "Instagram",
				link: "https://www.instagram.com/enayet_chowdhury_official/",
				svg: "instagram",
			},

			{
				name: "Facebook",
				link: "https://www.facebook.com/enayet.chowdhury1",
				svg: "facebook",
			},
		],
	};
</script>
<template>
	<Linktree :account="account">
		<template #title> @enayet_chowdhury_official </template>
		<template #second-title>তোরা নিজের সিমায় আগুন ধরা!</template>
	</Linktree>
</template>
