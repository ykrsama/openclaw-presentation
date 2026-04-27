<script setup lang="ts">
import { useNav } from '@slidev/client'
import { computed, ref, watch, nextTick } from 'vue'

const { currentSlideNo, slides, total } = useNav()

const currentPage = computed(() => currentSlideNo.value)
const totalPages = computed(() => total?.value ?? slides.value.length)
const isTitlePage = computed(() => currentPage.value === 1)
const shouldHidePageNumber = ref(false)

const checkPageNumber = () => {
  nextTick(() => {
    const slideElements = document.querySelectorAll('.slidev-page, [id^="page-"]')
    const currentIndex = currentSlideNo.value - 1
    const currentSlideElement = slideElements[currentIndex]

    if (currentSlideElement) {
      shouldHidePageNumber.value = currentSlideElement.classList.contains('no-page-number')
    } else {
      const altElement = document.querySelector(`#page-${currentSlideNo.value}`) ||
                         document.querySelector(`[data-slide="${currentSlideNo.value}"]`)
      if (altElement) {
        shouldHidePageNumber.value = altElement.classList.contains('no-page-number')
      } else {
        shouldHidePageNumber.value = false
      }
    }

    const currentSlide = slides.value[currentIndex]
    if (currentSlide) {
      const meta = currentSlide.meta || {}
      for (const key in meta) {
        const value = meta[key]
        if (typeof value === 'string' && value.includes('no-page-number')) {
          shouldHidePageNumber.value = true
        }
      }
    }
  })
}

watch(currentSlideNo, () => {
  checkPageNumber()
}, { immediate: true })

checkPageNumber()
</script>

<template>
  <div
    v-if="!isTitlePage && !shouldHidePageNumber"
    class="page-number"
    aria-label="Page number"
  >
    <span class="page-number-current">{{ currentPage }}</span>
    <span class="page-number-separator">/</span>
    <span class="page-number-total">{{ totalPages }}</span>
  </div>
</template>

<style scoped>
.page-number {
  position: fixed;
  top: 1.5rem;
  right: 2rem;
  z-index: 100;
  display: flex;
  align-items: baseline;
  gap: 0.25rem;
  font-family: 'DM Sans', sans-serif;
  font-size: 0.875rem;
  letter-spacing: 0.01em;
  color: var(--fg-2);
  user-select: none;
  pointer-events: none;
  opacity: 0.85;
  transition: opacity 300ms ease;
}

.page-number:hover {
  opacity: 1;
}

.page-number-current {
  font-weight: 600;
  color: var(--fg-1);
}

.page-number-separator {
  color: var(--fg-2);
  opacity: 0.6;
}

.page-number-total {
  color: var(--fg-2);
}
</style>
