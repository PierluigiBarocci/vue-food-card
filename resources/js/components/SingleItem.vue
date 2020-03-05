<template>
    <div class="card mt-4 mr-2">
        <img class="card-img-top" :src="item.img" :alt="item.name">
        <div class="card-body">
            <h5 class="card-title">{{ item.name }}</h5>
            <h6 class="card-subtitle mb-2 text-muted">{{ item.category }}</h6>
            <p class="card-text">{{ item.description }}</p>
            <a href="#" class="btn btn-success">Acquista</a>
        </div>
    </div>
</template>

<script>
export default {
  props: ["item"]
};
</script>

<style scoped>
.card {
    width: 350px;
}
.card img {
    height: 200px;
}
</style>