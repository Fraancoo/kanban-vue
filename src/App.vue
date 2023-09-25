<template>
  <div class="main_container">
    <div class="div_title">
      <h1 class="title">Kanban</h1>
    </div>
    <div class="div_content">
      <section id="sect_todo">
        <div>
          <h2 class="subtitle">To Do</h2>
          <div class="add_postit"></div>
        </div>
      </section>
      <div class="h_line"></div>
      <section id="sect_doing">
        <div>
          <h2 class="subtitle">Doing</h2>
        </div>
      </section>
      <div class="h_line"></div>
      <section id="sect_done">
        <div>
          <h2 class="subtitle">Done</h2>
        </div>
      </section>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style scoped>
.main_container {
  height: 100vh;
  width: 100vw;
  background-color: var(--blue-gray-1);
}

.div_title {
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 1px 0 3px var(--box-shadow);
}

.title {
  font-size: 3rem;
  user-select: none;
}

.div_content {
  height: calc(100% - 100px);
  padding: 10px;
  display: flex;
  justify-content: space-between;
}

.div_content > section {
  width: 100%;
  text-align: center;
}
.h_line {
  height: 100%;
  widows: 30px;
  border: 3px solid var(--yellow);
  border-radius: 3px;
}
</style>
