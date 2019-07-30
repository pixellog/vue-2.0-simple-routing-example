<template>
    <main-layout>

        <h4 id="item-1" style="">Item 1</h4>
        <p>{{ text }}</p>
        <h5 id="item-1-1" style="">Item 1-1</h5>
        <p>{{ text }}</p>
        <h5 id="item-1-2" style="">Item 1-2</h5>
        <p>{{ text }}</p>
        <h5 id="item-1-2-1" style="">Item 1-2-1</h5>
        <p>{{ text }}</p>
        <p>{{ text }}</p>
        <h5 id="item-1-2-2" style="">Item 1-2-2</h5>
        <p>{{ text }}</p>
        <p>{{ text }}</p>
        <p>{{ text }}</p>
        <h4 id="item-2" style="">Item 2</h4>
        <p>{{ text }}</p>
        <h4 id="item-3" style="">Item 3</h4>
        <p>{{ text }}</p>
        <h5 id="item-3-1" style="">Item 3-1</h5>
        <p>{{ text }}</p>
        <h5 id="item-3-2" style="">Item 3-2</h5>
        <p>{{ text }}</p>

    </main-layout>
</template>

<script>
    import MainLayout from '../../layouts/Main.vue'

    export default {
        components: {
            MainLayout
        },
        data() {
            return {
                text: `
          Quis magna Lorem anim amet ipsum do mollit sit cillum voluptate ex nulla
          tempor. Laborum consequat non elit enim exercitation cillum aliqua
          consequat id aliqua. Esse ex consectetur mollit voluptate est in duis
          laboris ad sit ipsum anim Lorem. Incididunt veniam velit elit elit veniam
          Lorem aliqua quis ullamco deserunt sit enim elit aliqua esse irure. Laborum
          nisi sit est tempor laborum mollit labore officia laborum excepteur
          commodo non commodo dolor excepteur commodo. Ipsum fugiat ex est consectetur
          ipsum commodo tempor sunt in proident.
        `
            }
        }
    }
</script>
