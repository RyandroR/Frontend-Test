<template>
    <div>
      <vueper-slides>
        <vueper-slide
          v-for="(slide, i) in slides"
          :key="i"
          :title="slide.title"
          :content="slide.content"
          :image="slide.image">
        </vueper-slide>
      </vueper-slides>
      
          <vueper-slides
      :visible-slides="3"
      slide-multiple
      :gap="3"
      :slide-ratio="1 / 4"
      :dragging-distance="200"
      :breakpoints="{ 800: { visibleSlides: 2, slideMultiple: 2 } }"
    >
      <vueper-slide
        v-for="i in 10"
        :key="i"
        :title="`title ${i}`"
        :image="`https://picsum.photos/id/${i}/400/300`"
      />
    </vueper-slides>
    </div>
  </template>
  
  <script>
  import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
  export default {
    components : {
VueperSlides, VueperSlide
    },
    data: () => ({
  slides: Array(10)
  .fill()
  .map((_, i) => ({
          title: `title ${i}`,
          content: `content ${i}`,
          image: `https://picsum.photos/id/${i + 1}/400/300`
        }))
  
})
  }
  </script>
  