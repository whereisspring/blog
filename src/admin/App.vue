<template>
  <div class="layout">
    <!-- banner -->
    <mu-row gutter>
      <mu-col width="100" tablet="100" desktop="100">
        <banner></banner>
      </mu-col>
    </mu-row>
    <!-- first -->
    <mu-row gutter>
      <mu-col width="100" tablet="80" desktop="60">
        <transition name="fade" mode="out-in">
          <router-view name="first"></router-view>
        </transition>
      </mu-col>
    </mu-row>
    <!-- second -->
    <mu-row gutter>
      <mu-col width="100" tablet="80" desktop="60">
        <transition name="fade" mode="out-in">
          <router-view name="second"></router-view>
        </transition>
      </mu-col>
    </mu-row>
    <!-- third -->
    <mu-row gutter>
      <mu-col width="100" tablet="100" desktop="100">
        <my-footer></my-footer>
        <!-- <transition name="fade" mode="out-in">
          <router-view name="third"></router-view>
        </transition> -->
      </mu-col>
    </mu-row>
  </div>
</template>

<style lang="css">
.layout div[class*="col-"] {
  margin-left: auto;
  margin-right: auto;
  color: #000;
  padding: 8px;
  margin-bottom: 8px;
}
</style>