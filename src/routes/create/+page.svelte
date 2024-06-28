<script>
    import { RangeSlider } from '@skeletonlabs/skeleton';
    import graph from '$lib/graph-example.png';

    let value = 0;
    let max = 10000;
</script>

<h1 class="h1">Node Activations</h1>
<br>
<img alt="Node Activation Graph" src={graph} style="height:20%;width:50%"/>
<br>

<div style="width:50%">
    <RangeSlider name="range-slider" bind:value={value} max={10000} step={1}>
        <div class="flex justify-between items-center">
            <div class="font-bold">Label</div>
            <div class="text-xs">{value} / {max}</div>
        </div>
    </RangeSlider>
    <div class="flex justify-between items-center">
        <div class="font-bold">Less</div>
        <div class="font-bold">More</div>
    </div>
</div>
<br>

<div class="table-container text-token">
    <table class="table table-hover">
        <thead>
            <tr>
                <th>Layer 1</th>
                <th>Layer 2</th>
                <th>Layer 3</th>
                <th>....</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Text Line</td>
                <td>Text Line</td>
                <td>Text Line</td>
                <td>
                    <button type="button" class="btn variant-filled">Publish</button>
                    <button type="button" class="btn variant-filled">Edit</button>
                    <button type="button" class="btn variant-filled">Delete</button>
                </td>
            </tr>
        </tbody>
    </table>
</div>