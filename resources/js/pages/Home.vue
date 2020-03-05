<template>
  <div>
    <cook-header></cook-header>
    <products-container></products-container>
  </div>
</template>

<script>
import CookHeader from "../components/CookHeader";
import ProductsContainer from "../components/ProductsContainer";


export default {
  components: {
    CookHeader,
    ProductsContainer
  },
  data() {
    return {};
  }
};
</script>