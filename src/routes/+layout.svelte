<script>
  import "../app.postcss";
  import { AppShell, AppRail, AppRailAnchor } from "@skeletonlabs/skeleton";
  import ShellHeader from "./shellHeader.svelte";
</script>

<!-- App Shell -->
<AppShell regionPage=" h-full ">
  <svelte:fragment slot="header">
    <ShellHeader />
  </svelte:fragment>
  <svelte:fragment slot="sidebarLeft">
    <div class="grid grid-cols-[auto_1fr] h-full">
      <AppRail class="hidden lg:grid" background=" bg-surface-50-900-token">
        <AppRailAnchor
        >
          <div class="flex items-center justify-center">
          </div>
          <p class="text-center">Dashboard</p>
        </AppRailAnchor>
        <AppRailAnchor
          ><div class="flex items-center justify-center">
          </div>
          <p class="text-center">Call</p>
        </AppRailAnchor>
        <AppRailAnchor
          label="Connect"
        >
          <div class="flex items-center justify-center">
          </div>

          <p class="text-center">Connect</p>
        </AppRailAnchor>
        <AppRailAnchor
          label="Library"
        >
          <div class="flex items-center justify-center">
          </div>

          <p class="text-center">Library</p>
        </AppRailAnchor>
        <AppRailAnchor
          label="Environment"
        >
          <div class="flex items-center justify-center">
          </div>

          <p class="text-center">Environment</p>
        </AppRailAnchor>

        <svelte:fragment slot="trail">
          <AppRailAnchor
            label="Account"
          >
            <div class="flex items-center justify-center">
            </div>

            <p class="text-center">Account</p>
          </AppRailAnchor>
        </svelte:fragment>

        <!-- <AppRailTile label="Leads" value={2}>🔍</AppRailTile> -->
        <!-- <AppRailTile label="Phonebook" value={3}>📞</AppRailTile> -->
        <!-- <AppRailTile label="Industries" value={4}>🏭</AppRailTile> -->
      </AppRail>
      <section>
      </section>
    </div>
  </svelte:fragment>
  <!-- <svelte:fragment slot="sidebarRight">Sidebar Right</svelte:fragment> -->
  <!-- <svelte:fragment slot="pageHeader"><AppBar>pageheaderbar</AppBar></svelte:fragment> -->
  <!-- Router Slot -->
  <slot />

  <!-- ---- / ---- -->
  <!-- <svelte:fragment slot="footer"><Footer></Footer></svelte:fragment> -->
</AppShell>
