<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  <!-- <h1 class="fade">Hello anh em. Welcome to Vue CLI</h1> -->
  <!-- <base-modal
    v-if="isShowModal"
    title="This is the title called from App.vue"
    content="This is the content called from App.vue"
    theme="sales"
    @cancel="onToggleModal"
  /> -->
  <!-- <teleport to="body">
    <base-modal
      v-if="isShowModal"
      title="This is the title called from App.vue"
      content="This is the content called from App.vue"
      theme="sales"
      @cancel="onToggleModal"
    >
      <template v-slot:header>
        <h2>This is a header</h2>
      </template>
      <label for="">Email</label>
      <input type="email" />
      <template v-slot:footer>
        <button @click="onToggleModal">Cancel</button>
      </template>
    </base-modal>
  </teleport>
  <button @click="onToggleModal">Toggle modal</button> -->
  <quiz-form />
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import MyModal from "./components/MyModal.vue";
import QuizForm from "./components/QuizForm.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    // BaseModal: MyModal,
    QuizForm,
  },
  data() {
    return {
      isShowModal: false,
    };
  },
  methods: {
    onToggleModal() {
      console.log("RUN RUN RUN");
      this.isShowModal = !this.isShowModal;
    },
  },
};
</script>
