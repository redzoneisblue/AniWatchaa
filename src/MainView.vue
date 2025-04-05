<script setup>
import Card from './components/Card.vue'
</script>

<template>

    <div class="main-container">
        <search>
            <input type="text" name="user_search" id="" placeholder="Enter to search">
            <button>Search</button>
        </search>
        <main>
            <!-- card div -->
            <Card />
            
        </main>
    </div>

</template>

<style lang="scss" scoped>
.main-container {
    padding-top: 2rem;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    search {
        input {
            outline: none;
            width: 15rem;
            padding: 0.5rem 1rem;
            margin-right: 0.5rem;
        }
        button {
            font-weight:bold;
            user-select: none;
            padding: 0.5rem 1rem;
            background-color: aqua;
            &:hover {
                cursor: pointer;
            }
            &:active {
                background-color: white;
            }
        }
    }
    main {
        background-color: grey;
        margin-top: 1rem;
        height: fit-content;
        width: 70%;
        padding: 1rem;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        row-gap: 1rem;
    }
}
</style>