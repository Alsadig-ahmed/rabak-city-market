<script>
    import {RealStates} from '../store'
</script>
<section>
    {#each $RealStates as land}
    <div class="flex card">
        <h2 class="img"> صورة {land.Image} </h2>
        <div class="">
             <p> المالك :  { land.landOwner} </p>
             <h2>  وصف لقطعة الارض : {land.discription} </h2>
             <h2> الموقع : {land.location} </h2>
        </div>
        </div>
    {/each}
</section>

<style>
    .flex{
        display: flex;
    }
    .card{
        border: 1px solid rgba(0, 0, 0, 0.13);
        text-align: center;
        margin: .5rem  auto;
        border-radius: 2rem;
        box-shadow: 0 0 12px 0px rgba(0, 0, 0, 0.616);
    }
    .img{
        width: 50%;
        height: 12rem;
        border-radius: 2rem;
        background-color: rgb(211, 236, 209);
        margin-inline: 2rem;
    }
</style>