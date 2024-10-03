<script lang="ts">
    import PhEye from '~icons/ph/eye';
    import PhEyeSlash from '~icons/ph/eye-slash';

    export let name: string;
    export let content: string;
    export let censor: boolean;

    let show: boolean = false;
</script>

<div class="bg-gray-200 p-3 rounded-md">
    <h4 class="text-sm text-gray-600">{name}</h4>
    <div class="flex flex-row">
        <input type={censor ? "password" : "text"} disabled value={content} class="text-lg grow">
        {#if censor}
            <PhEyeSlash />
        {/if}
    </div>
</div>
