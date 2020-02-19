<script>
    export let isOpen = false

    function closePopup(){
        isOpen = false;
    }
</script>

<style>
    .overlay{
        position: fixed; 
        display: none; 
        width: 100%; 
        height: 100%; 
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgba(0,0,0,0.5); 
        z-index: 100; 
    }

    .overlay-body {
        position: absolute;
        background-color: #2e2e2e;
        min-height: 20vh;
        width: 50vw;
        padding: 30px;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        -ms-transform: translate(-50%,-50%);
    }
    .overlay-body h3 {
        color: white;
    }

    .close{
        position: absolute;
        top: 10px;
        right: 10px;
        font-size: 25px;
        color: white;
        /* border: 2px solid white; */
        border-radius: 50%;
        padding: 0px 5px;
    }

    .show{
        display: block
    }

    @media only screen and (max-width: 768px) {

        .overlay-body {
            width: 100vw;
            min-height: 50vh;
            top: 100px;
            left: 0;
            transform: inherit;
        }
    }
	
</style>

<div class="overlay" class:show={isOpen}>
    <div class="overlay-body">
        <span class="close" on:click={closePopup}>x</span>
        <slot name="title"><h3>Header</h3></slot>
        <slot name="body"><p>Body</p></slot>
    </div>
</div>
