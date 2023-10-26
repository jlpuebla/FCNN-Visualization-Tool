<script>
    let active = {clicked: false };
    export let name = "default";

    function onClick(){
        active.clicked = !active.clicked;
    }

</script>

<button on:click = {onClick}>
    {name}
</button>

{#if active.clicked}
    <br><br>
    <label for="hlayers">Hidden Layers</label>
    <input type="radio" id="hlayers" name="createnn"><br><br>
    <label for="olayer">Output Layer</label>
    <input type="radio" id="olayer" name="createnn"><br><br>
    <label for="dataset">Dataset</label>
    <input type="radio" id="dataset" name="createnn"><br><br>
{/if}