<template>
  <div class="question-answer py-5">
    <div class="container px-lg-5 px-3">
      <div class="feedback mb-5">
        <img src="../../assets/icons/img_suggest_feedback.svg" alt="qa" />
        <div
          class="w-100 d-flex flex-lg-row flex-column align-items-lg-center mb-lg-0 mb-3 justify-content-between"
        >
          <AtomTitle
            tag="h5"
            content="Have a problem or suggestion? Leave us a feedback"
            class="fw-bold mb-lg-0 mb-2 ms-lg-4 ms-0"
          />
          <AtomButton :link="{ name: 'Give Feedback', url: '#' }" />
        </div>
      </div>
      <QuestionTabs />
      <div class="mt-3 mb-5">
        <Terms />
      </div>
    </div>
  </div>
</template>

<style scope>
.feedback {
  background-color: #f4f4f4;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 15px 25px 15px 15px;
  border-radius: 20px;
}
</style>

<script>
import QuestionTabs from "./QuestionTabs.vue";
import AtomTitle from "../atoms/AtomTitle.vue";
import AtomButton from "../atoms/AtomButton.vue";
import Terms from "./Terms.vue";

export default {
  components: {
    QuestionTabs,
    AtomTitle,
    AtomButton,
    Terms,
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
