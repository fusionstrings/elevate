<script>
    import Overlay from '../components/overlay.svelte';
    export let alertsList = [];
    let isOpen= false;

    function openNotificationsPopup() {
        isOpen = true;
    }

</script>

<style>
	.alerts-icon{
		background: url('/images/icon-bell.png') no-repeat center bottom;
		background-size: contain;
		display: inline-block;
		width: 30px;
        height: 30px;
        justify-self: end;
    }
    
    ul {
        margin-bottom: 0;
    }

    .alerts-icon h3 {
        color: white;
        border-bottom: 2px solid white;
    }

    .alert-item{
        color: white;
        padding: 10px 0;
        border-bottom: 1ps solid white;
    }
</style>

<span class="alerts-icon" on:click={openNotificationsPopup}>
    <Overlay {isOpen}>
        <h3 slot="title">NOTIFICATIONS</h3>

        <ul slot="body">
            {#each alertsList as alert}
                <li class="alert-item">{alert}</li>
            {/each}
        </ul>
    </Overlay>
</span>
