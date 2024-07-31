# Interactivity Question

<div class="flex justify-center items-end h-1/5">
<div class="flex items-center gap-12 w-[250px]">
<input type="checkbox" />
<span class="not-checked">I'm not checked</span>
<span class="checked">I'm checked!</span>
</div>
</div>

<style>
    input {
        /* outline: 1px solid white; */
        border-radius: 10px;
        padding: 10px;
    }

    span {
        display:none;
        /* line-height: 11px; */
    }

    input:not(:checked) ~ .not-checked {
        display:block;
    }

    input:checked ~ .checked {
        display:block;
    }
</style>
