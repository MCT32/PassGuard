<script lang="ts">
  import { invoke } from "@tauri-apps/api/core";
  import ListEntry from "$lib/components/ListEntry.svelte";
  import PhPlusSquare from '~icons/ph/plus-square';
  import PhMagnifyingGlass from '~icons/ph/magnifying-glass';
  import PhStar from '~icons/ph/star';
  import Field from "$lib/components/Field.svelte";
</script>

<div class="flex h-screen">
  <div class="flex flex-col min-w-[25rem] border-r-2 border-gray-400">
    <div class="bg-blue-500 py-3 px-5 flex flex-row shrink-0 items-center gap-2 h-20">
      <div class="flex flex-row grow bg-gray-200 rounded-md items-center pr-5">
        <input type="text" placeholder="Search" class="w-full p-2 bg-transparent">
        <PhMagnifyingGlass class="text-gray-500" />
      </div>
      <PhPlusSquare class="w-8 h-8 text-blue-200" />
    </div>
    <div class="overflow-y-auto grow">
      <ul>
        <ListEntry name="Github" username="MCT32" icon="https://github.githubassets.com/assets/GitHub-Mark-ea2971cee799.png" />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
        <ListEntry />
      </ul>
    </div>
  </div>
  <div class="flex flex-col grow">
    <div class="bg-blue-500 py-3 px-5 flex flex-row justify-between items-center gap-2 h-20">
      <button class="h-8 bg-blue-200 px-3 rounded-md text-gray-500">
        Edit
      </button>
      <PhStar class="w-8 h-8 text-blue-200" />
    </div>
    <div class="overflow-y-auto grow flex flex-col gap-2 py-10 px-20">
      <div class="flex flex-row items-center gap-2">
        <img src="https://github.githubassets.com/assets/GitHub-Mark-ea2971cee799.png" alt="icon" class="w-28 h-28">
        <h1 class="text-3xl">Github</h1>
      </div>

      <Field name="Username" content="MCT32" censor={false} />
      <Field name="Password" content="thisisapassword" censor={true} />
    </div>
  </div>
</div>
