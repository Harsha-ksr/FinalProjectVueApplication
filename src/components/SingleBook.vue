<template>
    

    <div  :class="book.published ? 'green': 'red' ">
    <h1> Place Name : {{book.PlaceName}} </h1>
    <h2> Country : {{book.Country}} </h2>
    <h4> About : {{book.Description}} </h4>
    <h4> {{book.FamousFor}} </h4>
    <h4> Best Time to Visit : {{book.BestTimeToVisit}} </h4>
    <h4> Ranked : {{book.Rank}} </h4>
    <h4> No Of Visitors : {{book.NoOfVisitor}} </h4>
    </div>
</template>

<script>

export default{
    name: 'SingleBook',
    props:{
        book: Array
    }
}
</script>

<style scoped>

.green{
    background-color: green;
}

h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    border: 10px solid #FAFA33;
    

}

.red{
background-color: orangered !important;

}


</style>