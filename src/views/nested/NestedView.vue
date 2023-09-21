// 중첩라우트 push 히스토리 쌓음 , replace 히스토리 쌓지 않음
<template>
	<div>
		<ul class="nav nav-pills">
			<li class="nav-item">
				<RouterLink
					class="nav-link"
					active-class="active"
					:to="{ name: 'NestedOne', replace: true }"
				>
					Nested One
				</RouterLink>
			</li>
			<li class="nav-item">
				<RouterLink
					class="nav-link"
					active-class="active"
					:to="{ name: 'NestedTwo', replace: true }"
				>
					Nested Two
				</RouterLink>
			</li>
		</ul>
		<hr class="my-4" />
		<RouterView></RouterView>
	</div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
