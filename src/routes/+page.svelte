
<script>
    let count = 0;
</script>

<div class="container">
   <div class="image"></div>
    <h1 class="title">Tasbih</h1>
    <h1 class="count">{count}</h1> 
    <div class="btn">
        <button class='reset' on:click={()=>{count = 0}} >Reset</button>
        <button class="btn" on:click={()=>{count ++}}>Button</button></div>
    

</div>

<style>
    .title{
        color: rgb(234, 132, 149) ;
    }
:global(body){
    background-color: rgb(248, 231, 234);
}
.container{
    font-family: Arial, Helvetica, sans-serif;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items:center;
    min-height: 80vh;
   

   
}
.image{
    background-image: url('/test.png');
    background-size: cover;
    background-position: center;
    width: 7rem;
    height: 7rem;
    border-radius: 50%;
}
button{
    border-radius: 5%;
    padding: 1.2rem 2rem;
    
   background-color:rgb(234, 132, 149) 
}
.reset{
    
   background-color: pink;;
    border-radius: 50%;
    padding: 20px 10px;
}
.count{
    color: rgb(202, 68, 113);
        font-size: 4rem;
    }
.btn{
    display: flex;
    align-items: center;
    flex-direction: column;
    gap: 40px;
}
button:active{
    background-color: rgb(202, 68, 113);
}
</style>
