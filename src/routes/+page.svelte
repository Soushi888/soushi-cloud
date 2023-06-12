<script lang="ts">
  import { invoke } from "@tauri-apps/api/tauri";

  let name = "";
  let greetMsg = "";

  async function greeting() {
    greetMsg = await invoke("greet", { name });
  }
</script>

<div class="container h-full mx-auto flex justify-center items-center">
  <div class="space-y-5">
    <h1 class="h1">Soushi Cloud</h1>
    <input
      class="input p-3"
      id="greet-input"
      placeholder="Enter a name..."
      bind:value={name}
    />
    <button class="btn variant-filled-primary" on:click={greeting}>Greet</button
    >
    <p>{greetMsg}</p>
  </div>
</div>
