<template>
    <div class="zawartosc">
        <div v-if="img == 1">
            <img src="../assets/image1.png" :alt="alt" class="pictures">
        </div>
        <div v-if="img == 2">
            <img src="../assets/image2.png" :alt="alt" class="pictures">
        </div>
        <div v-if="img == 3">
            <img src="../assets/image3.png" :alt="alt" class="pictures">
        </div>
        <div v-if="img == 4">
            <img src="../assets/image4.png" :alt="alt" class="pictures">
        </div>
        <div v-if="img == 5">
            <img src="../assets/image5.png" :alt="alt" class="pictures">
        </div>
        <div v-if="img == 6">
            <img src="../assets/image6.png" :alt="alt" class="pictures">
        </div>
        <div>
            <h3>{{ title }}</h3>
            <p>{{ content }}</p>
            <a href="http://">Learn More ⭢</a>
        </div>    
    </div>
</template>

<script lang="ts">
import { Options, Vue} from 'vue-class-component';

@Options({
  props: {
    img: Number,
    alt: String,
    title: String,
    content: String

  }
})
export default class PageCard extends Vue {
    img!: number
    alt!: string
    title!: string
    content!: string
}
</script>