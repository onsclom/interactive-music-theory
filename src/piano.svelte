<script lang="ts">
  const noteSize = 40;
  const blackNoteSize = 23;
  const octaves = 2;
</script>

<div class="h-28 relative overflow-x-scroll flex">
  {#each Array(octaves) as _, i}
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${noteSize + i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${noteSize * 2 + i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${noteSize * 3 + i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${noteSize * 4 + i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${noteSize * 5 + i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer border-2 absolute h-full"
      style:left={`${noteSize * 6 + i * noteSize * 7}px`}
      style:width={`${noteSize}px`}
    ></div>
    <div />

    <!-- black keys -->
    <div
      class="hover:bg-red-500 cursor-pointer h-16 absolute bg-black"
      style:left={`${noteSize / 2 + (noteSize - blackNoteSize) / 2 + i * noteSize * 7}px`}
      style:width={`${blackNoteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer h-16 absolute bg-black"
      style:left={`${noteSize / 2 + (noteSize - blackNoteSize) / 2 + noteSize + i * noteSize * 7}px`}
      style:width={`${blackNoteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer h-16 absolute bg-black"
      style:left={`${noteSize / 2 + (noteSize - blackNoteSize) / 2 + noteSize * 3 + i * noteSize * 7}px`}
      style:width={`${blackNoteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer h-16 absolute bg-black"
      style:left={`${noteSize / 2 + (noteSize - blackNoteSize) / 2 + noteSize * 4 + i * noteSize * 7}px`}
      style:width={`${blackNoteSize}px`}
    ></div>
    <div
      class="hover:bg-red-500 cursor-pointer h-16 absolute bg-black"
      style:left={`${noteSize / 2 + (noteSize - blackNoteSize) / 2 + noteSize * 5 + i * noteSize * 7}px`}
      style:width={`${blackNoteSize}px`}
    ></div>
  {/each}
</div>
