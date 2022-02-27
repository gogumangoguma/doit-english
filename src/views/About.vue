<template>
  <div class="about">
    <h1 class="page__title">{{ dataEn.title }}</h1>
    <div
      class="paragraph__container"
      v-for="(section, index) in dataEn.contents"
      :key="`${index}_${section.subTitle}`"
    >
      <div class="text__title">{{ section.subTitle }}</div>
      <div class="box__content">
        <template v-for="(sentense, idx) in section.content">
          <div :key="`en_sentense_${idx}`" class="sentense__en">
            <span
              v-for="(word, i) in splitSentense(sentense)"
              :key="`word_${i}`"
            >
              {{ word }}
            </span>
          </div>
          <div :key="`ko_sentense_${idx}`" class="sentense__ko">
            <span
              v-for="(word, i) in splitSentenseKorea(index, idx)"
              :key="`word_ko_${i}`"
            >
              {{ word }}
            </span>
          </div>
        </template>
      </div>
    </div>
  </div>
</template>

<script>
import dataEn from "../assets/Data/en/HowDoesTheInternetWork.json";
import dataKo from "../assets/Data/ko/HowDoesTheInternetWork.json";

export default {
  name: "AboutTest",

  data: () => ({
    dataEn,
    dataKo,
  }),
  methods: {
    splitSentense(sentense) {
      return sentense.split(" ");
    },
    splitSentenseKorea(index, idx) {
      const sentense = this.dataKo.contents?.[index]?.content?.[idx];
      if (sentense !== undefined) {
        return sentense.split(" ");
      }
      return [];
    },
  },
};
</script>

<style lang="scss" scoped>
.page__title {
  padding: 12px;
}
.paragraph__container {
  .text__title {
    padding: 12px;
    font-size: 24px;
    color: grey;
  }
  .box__content {
    padding: 4px 12px;
    display: flex;
    flex-direction: column;
    font-size: 16px;
    .sentense__en {
      font-size: 16px;
      font-weight: 500;
    }
    .sentense__ko {
      font-weight: 400;
      color: darkgrey;
    }
  }
}
</style>
