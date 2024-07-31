# Search Question

<div class="flex justify-center items-end gap-12 h-1/5">
<input placeholder="What would you like to search?" />
<button>Search</button>
</div>
<div class="color-gray">
/search?q=SomeSearch
</div>
<div class="flex flex-col gap-2">
Here are the results:
<div class="result-item">Some item</div>
<div class="result-item">Some item</div>
<div class="result-item">Some item</div>
<div class="result-item">Some item</div>
</div>

<style>
    input {
        outline: 1px solid white;
        width: 400px;
        border-radius: 10px;
        padding: 10px;
    }

    .result-item {
        outline: 1px solid white;
        width: 400px;
        border-radius: 10px;
        padding-inline: 10px;
        padding-block: 5px;
    }

    button {
        outline: 1px solid white;
        border-radius: 10px;
        padding: 10px;
    }

    .button-container:has(button:hover) button:not(:hover) {
        scale: 0.5;
    }
</style>
