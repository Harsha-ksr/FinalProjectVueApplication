<template>
<div>
 <h1> {{bookName}} </h1>
    <h2>{{authorName}} </h2 >
    <h3> {{yourname}} </h3>
</div>
</template>

<script>

export default{ // Exporting Default Object
    name: 'MyHeader',
    props:{ 

        authorName:String,
        bookName:String,
        yourname:String

    }
}

</script>

<style scoped>

div{
    text-align: center;
    background-color: #FAFA33;
    font-style: sans-serif;
    padding: 1em;
    border: 10px solid #ffb89e;
}

</style>