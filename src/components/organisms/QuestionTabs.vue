<script setup>
import list from "../../data/ListQuestion";
</script>

<template>
  <AtomTitle tag="h5" content="Question and Answer" class="fw-bold mb-3" />
  <div class="tabs">
    <div class="nav-tabs">
      <div class="nav-item" @click="setActive('tab-1')" :class="{ active: isActive('tab-1') }">
        <p class="mb-0">General</p>
      </div>
      <div class="nav-item" @click="setActive('tab-2')" :class="{ active: isActive('tab-2') }">
        <p class="mb-0">Prepaid</p>
      </div>
      <div class="nav-item" @click="setActive('tab-3')" :class="{ active: isActive('tab-3') }">
        <p class="mb-0">Postpaid</p>
      </div>
    </div>
    <div class="tab-content">
      <div class="tab-pane" v-show="isActive('tab-1')">
        <ul>
          <li v-for="data in list" v-bind:key="data.id">
            <AtomSubtitle class="list mb-2 font-dark fw-lighter" :text="data.subtitle" />
          </li>
        </ul>
      </div>
      <div class="tab-pane" v-show="isActive('tab-2')">
        <ul>
          <li v-for="data in list" v-bind:key="data.id">
            <AtomSubtitle class="list mb-2 font-dark fw-lighter" :text="data.subtitle + '2'" />
          </li>
        </ul>
      </div>
      <div class="tab-pane" v-show="isActive('tab-3')">
        <ul>
          <li v-for="data in list" v-bind:key="data.id">
            <AtomSubtitle class="list mb-2 font-dark fw-lighter" :text="data.subtitle + '3'" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import AtomTitle from "../atoms/AtomTitle.vue";
import AtomSubtitle from "../atoms/AtomSubtitle.vue";

export default {
  components: {
    AtomTitle,
    AtomSubtitle,
  },
  data: () => ({
    activeTab: "tab-1",
  }),
  methods: {
    setActive(tab) {
      this.activeTab = tab;
    },
    isActive(tab) {
      return this.activeTab === tab;
    },
  },
};
</script>

<style scoped>
.nav-tabs {
  display: flex;
  border-bottom: none;
}
.nav-item {
  color: white;
  transition: all 150ms;
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-color: #ed2324;
  border-radius: 32px;
  margin-right: 8px;
  padding: 8px 14px;
  margin-bottom: 15px;
}
.nav-item:active {
  color: red;
  background-color: aqua;
}
.tab-content > .tab-pane {
  display: flex;
}
</style>
