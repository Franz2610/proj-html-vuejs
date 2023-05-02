<template>
    <div class="align-items-center justify-content-center text-center btn-wrapper">
        <h4>Start today for getting <span>Online Certificate</span> </h4>
        <h2 class="mb-4">You can be your own guiding star with our help</h2>
        <button class="btn btn-success">
            Get started now
        </button>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;

button{
    padding-left: 55px;
    padding-right: 55px;
}
.btn-success{
    background-color: $btn-green;
}
span{
    color: $btn-green;
}
.btn-wrapper{
    margin-top: 100px;
    height: 300px;
}
button:hover{
    background-color: $bg-primary;
    color: white;
    transition: 2s;
    padding: 25px;
}

</style>