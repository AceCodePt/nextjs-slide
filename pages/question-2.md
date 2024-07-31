# Search Question

<div class="flex justify-center items-end gap-12 h-1/5">
<input placeholder="What would you like to search?" />
<button>Search</button>
</div>
<div class="color-gray">
/search
</div>

<style>
    input {
        outline: 1px solid white;
        width: 400px;
        border-radius: 10px;
        padding: 10px;
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
