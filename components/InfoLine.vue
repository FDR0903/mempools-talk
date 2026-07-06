<template>
	<footer class="absolute bottom-0 left-0 right-0 flex text-center text-white">
		<div class="flex-1 p-1" style="background:#1e293b">
			{{ $slidev.configs.author || "Unknown author" }}
		</div>
		<div class="flex-1 p-1" style="background:#334155">
			{{ $slidev.configs.title || "Unknown title" }}
		</div>
		<div class="flex-1 p-1" style="background:#475569">
			<div class="float-right">
				<template v-if="inAppendix">Appendix</template>
				<template v-else>{{ $slidev.nav.currentPage }} / {{ mainTotal }}</template>
			</div>
			{{ $slidev.configs.date || new Date().toLocaleDateString() }}
		</div>
	</footer>
</template>

<script setup lang="ts">
import { computed } from "vue";
import type { SlideInfoBase } from "@slidev/types";

const APPENDIX_SECTION = "Appendix";

const runningSections = computed(() => {
	const result: string[] = [];
	let title = "";
	for (let i = 0; i < $slidev.nav.slides.length; i++) {
		const s = ($slidev.nav.slides[i]?.meta?.slide as SlideInfoBase)?.frontmatter?.section;
		if (s) title = s;
		result.push(title);
	}
	return result;
});

const mainTotal = computed(() =>
	runningSections.value.filter(s => s !== APPENDIX_SECTION).length,
);

const inAppendix = computed(
	() => runningSections.value[$slidev.nav.currentPage - 1] === APPENDIX_SECTION,
);
</script>
