<script>
    import Modal from "./Modal.svelte";

    let showModal = false;
    const handleToggleModal = () => {
        showModal = !showModal;
    }
</script>

<button on:click={handleToggleModal} class="bg-blue-500 rounded-full p-3 m-10 drop-shadow-md">Open Modal</button>
<Modal open={showModal} on:cancle={handleToggleModal}/>
