<template>
  <div>
    <div class="pageTitle">
      <span class="title">LaraFood</span>
      <span class="dots">
        <span></span>
        <span></span>
        <span></span>
      </span>
    </div>

    <div class="content">
      <div class="container">
        <modules />
        <div class="right">
          <div class="content">
            <player />

            <support-lesson />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Modules from "./components/Modules.vue";
import Player from "./components/Player.vue";
import SupportLesson from "./components/Supports.vue";

export default {
  name: "ModulesAndLessons",

  components: {
    Modules,
    Player,
    SupportLesson,
  },
};
</script>