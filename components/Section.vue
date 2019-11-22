<template>
    <div class="content">
        <div class="Section">
            <h2 class="Section__title">{{ title }}</h2>
            <div class="Section__content">
                <slot></slot>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['title']
    }
</script>

<style>

    .Section {
        position: relative;
        justify-content: space-between;
        display: flex;
    }

    .Section__title {
        width: 30%;
        padding-top: 3.125rem;
    }

    .Section__content {
        width: 65%;
        margin-top: 3.665rem;

    }

    @media (max-width: 667px) {

        .Section {
            display: contents;
        }

        .Section__title {
            width: 100%;
        }

        .Section__content {
            width: 100%;
            margin-top: 2rem;
        }
    }

</style>
