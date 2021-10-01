<template>
  <ul class="pt-2">
    <li v-for="(item, idx) in items" :key="`item-${idx}`" class="pb-2 flex">
      <ul v-if="isArrayOfStrings(item)" class="pl-12">
        <li v-for="subitem in item" :key="subitem" class="mb-0">
          - {{ subitem }}
        </li>
      </ul>
      <div v-else-if="isObjectWithTitleAndItems(item)">
        <div class="text-base text-gray-500">
          <span class="font-bold text-lg">
            {{ item.title }}
          </span>
          <ul class="mt-2">
            <li v-for="subitem in item.items" :key="subitem" class="pb-2 flex">
              <SvgCheckmark />
              <span class="ml-3">
                {{ subitem }}
              </span>
            </li>
          </ul>
        </div>
      </div>
      <div v-else class="text-base text-gray-500 flex">
        <SvgCheckmark />
        <span class="ml-3">
          {{ item }}
        </span>
      </div>
    </li>
  </ul>
</template>

<script>
import SvgCheckmark from '@/components/svgIcons/SvgCheckmark.vue'

export default {
  name: 'ItemsList',
  components: {
    SvgCheckmark,
  },
  props: {
    items: {
      type: Array,
      default: () => [],
    },
  },
  methods: {
    // Check if item is an array of strings
    isArrayOfStrings(item) {
      return Array.isArray(item) && item.every((i) => typeof i === 'string')
    },
    // Check if item is an object with title and items
    isObjectWithTitleAndItems(item) {
      return typeof item === 'object' && item.title && item.items
    },
  },
}
</script>
