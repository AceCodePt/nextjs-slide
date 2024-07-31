# Buttons Question

<div class="button-container flex justify-center items-center gap-14 h-4/5">
<button>1</button>
<button>2</button>
<button>3</button>
<button>4</button>
<button>5</button>
</div>

<style>
    button {
        cursor: pointer;
        outline: white solid 1px;
        border-radius: 10px;
        padding: 10px;
        transition: scale 0.3s ease;
    }

    .button-container:has(button:hover) button:not(:hover) {
        scale: 0.5;
    }
</style>
