<script>
  import LdModeSwitch from "./LDModeSwitch.svelte";

  import { goto } from "$app/navigation";

  import { Facebook, Instagram } from "lucide-svelte";
  import Button from "$lib/components/ui/button/button.svelte";
</script>

<header
  class="fixed top-0 flex justify-between p-3 w-full bg-background border-b"
>
  <button onclick={() => goto("/#")}>
    <h1 class="text-xl">
      <i class="fa-solid fa-cart-shopping"></i> Prime Gadget
    </h1>
  </button>

  <div>
    <a href="https://www.instagram.com/shop.primeg">
      <Button variant="outline" size="icon">
        <Instagram />
        <span class="sr-only">Instagram</span>
      </Button>
    </a>
    <a href="https://www.facebook.com/shop.primeg">
      <Button variant="outline" size="icon">
        <Facebook />
        <span class="sr-only">Facebook</span>
      </Button>
    </a>
    <LdModeSwitch />
  </div>
</header>
