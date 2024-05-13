<template>
    <div class="pill">
        <span class="name"> {{ name }} </span>
        <span class="amount"> {{ amount }} </span>
    </div>
</template>

<script>
export default {
    props: ['name', 'amount']
}
</script>

<style scoped>
.pill {
    display: flex;
    align-items: center;
    margin: 8px;
    height: 55px;
    border-radius: 30px;
    background-color: #dc143c;
    color: #fff;
    font-size: 1.3rem;
    font-weight: bold;
}

.pill .name {
    margin-left: 16px;
}

.pill .amount {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 8px;
    padding: 6px;
    height: 35px;
    min-width: 35px;
    border-radius: 18px;
    background-color: #fff;
    color: #dc143c;
    font-size: 14px;
}
</style>