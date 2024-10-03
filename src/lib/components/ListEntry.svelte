<script lang="ts">
    export let name: string = "Name";
    export let username: string = "Username";
    export let icon: string = "https://beta.mct32.xyz/favicon.png";
</script>

<div class="flex flex-row h-20 p-3 border-b border-gray-400 hover:bg-gray-200 active:bg-gray-300 select-none">
    <img src={icon} alt="icon" class="h-full">

    <div class="pl-3 h-fit w-full font-semibold">
        <h3>{name}</h3>
        <h4 class="text-gray-500">{username}</h4>
    </div>
</div>
