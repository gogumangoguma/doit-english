<template>
  <v-app id="inspire">
    <v-app-bar app clipped-right flat height="72">
      <v-spacer></v-spacer>

      <v-responsive max-width="156">
        <v-text-field
          dense
          flat
          hide-details
          rounded
          solo-inverted
        ></v-text-field>
      </v-responsive>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" app permanent>
      <v-sheet color="grey lighten-5" height="72" width="100%"></v-sheet>

      <div class="list__container">
        <div v-for="item in items" :key="item.id">
          <router-link class="list__item" :to="item.link"
            >{{ item.title }}
          </router-link>
        </div>
      </div>
    </v-navigation-drawer>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    drawer: null,
    items: [
      { id: "0_home", title: "Home", link: "/" },
      {
        id: "1_howDoes",
        title: "How Does the Internet Work?",
        link: "/howInternetWork",
      },
      { id: "2_test", title: "Test", link: "/test" },
    ],
  }),
};
</script>

<style scoped lang="scss">
.list__container {
  display: flex;
  flex-direction: column;

  .list__item {
    display: flex;
    align-items: center;
    width: 100%;
    height: 48px;
    padding: 16px;

    text-decoration: none;
    color: #222222;
    font-size: 16px;
    font-weight: 600;
    &:hover {
      background-color: #65b2d045;
      opacity: 0.6;
    }
  }
}
</style>
