<template>
    <div class="grid place-content-center">
        <slot name="image" ></slot>
        <div class="flex gap-2">
            <div class="flex gap-1">
                <slot name="user" ></slot>
            </div>
            <div class="flex gap-1">
                <slot name="agenda" ></slot>
            </div>
        </div>
    </div>
    <div>
        <!-- Content slot -->
        <slot name="content" ></slot>
    </div>
</template>

