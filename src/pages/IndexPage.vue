<template>
  <q-page class="page">
    <div class="sub-page limiter">
      <HeaderComponent class="header" v-model="tab"/>

      <q-tab-panels class="tabs" v-model="tab" animated>
        <q-tab-panel class="tab" :name="1">
          <div class="text-h6">Mails</div>
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </q-tab-panel>

        <q-tab-panel class="tab" :name="2">
          <div class="text-h6">Alarms</div>
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </q-tab-panel>

        <q-tab-panel class="tab" :name="3">
          <div class="text-h6">Movies</div>
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </q-tab-panel>
      </q-tab-panels>
    </div>
  </q-page>
</template>

<script>

import HeaderComponent from "components/header/HeaderComponent.vue";

export default {
  name: 'IndexPage',
  components: {HeaderComponent},
  data() {
    return {
      tab: 1
    }
  }
}
</script>

<style lang="scss">
.page {
  background-color: #545a88;
  display: flex;
  flex-direction: column-reverse;

  .sub-page {
    background-color: #0f1322;
    height: 90vh;
    border-radius: 25px 25px 0 0;
    padding: 40px 20px 0 20px;

    .header {
      margin: 5px 50px 25px 50px;
    }

    .tabs {
      border-radius: 20px;

      .tab {
        background: rgb(157, 223, 237);
        background: linear-gradient(45deg, rgba(157, 223, 237, 1) 0%, rgba(135, 203, 214, 1) 100%);
      }
    }

  }
}
</style>
