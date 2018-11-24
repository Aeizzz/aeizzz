<template>
<div id="app" class="docs scotchified">
    <nav class="main mb-6">
        <div class="container-lg d-flex flex-justify-between pl-3">
            <router-link :to="'/list'" class="brand">
            <img :src="brand">
                <span class="h1">{{subtitle}}</span>
            </router-link>
        </div>
    </nav>
    <section id="top">
        <router-view>
        </router-view>
    </section>
    <footer class="main container-lg">
        <p>This is A light style blog based on Vue with Github api,
            <a href="https://github.com/Aeizzz/aeizzz/issues">edit</a></p>
    </footer>
</div>
</template>
<script>
import "primer-base/index.scss";
import "primer-layout/index.scss";
import "primer-utilities/index.scss";
import "../style/main.scss";
import "../style/nav.scss";
import "../style/footer.scss";
import * as brand from "../assets/svg/brand.svg";
export default {
  name: "app",
  data: function() {
    return {
      subtitle: "Aei",
      brand: brand
    };
  }
};
</script>
