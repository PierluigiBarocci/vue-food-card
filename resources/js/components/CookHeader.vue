<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
        <div class="container">
            <a class="navbar-brand" href="#">Cooking Pier</a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarColor02" aria-controls="navbarColor02" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarColor02">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item" v-for="(listItem, index) in listItems" :key="index">
                        <a class="nav-link" :href="listItem.href">{{ listItem.title }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>    
</template>

<script>
export default {
    data() {
        return {
            listItems: [
            {href: "home", title: "Home"},
            {href: "about-us", title: "About Us"},
            {href: "price", title: "Pricing"},
            {href: "work", title: "Work With Us"}
            ]
        };        
    }
}
</script>

<style>

</style>