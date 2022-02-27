<template>
  <div class="about">
    <h1 class="page__title">{{ datas.title }}</h1>
    <div
      class="paragraph__container"
      v-for="(section, index) in datas.contents"
      :key="`${index}_${section.subTitle}`"
    >
      <div class="text__title">{{ section.subTitle }}</div>
      <div class="box__content">
        <span v-for="sentense in section.content" :key="sentense">
          {{ sentense }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
import data from "../assets/Data/en/HowDoesTheInternetWork.json";

export default {
  name: "AboutTest",

  data: () => ({
    datas: data,
  }),
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
  }
}
</style>
