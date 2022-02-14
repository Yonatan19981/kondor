<template>
  <div>
    <h1>New to Kondor?</h1>
    <div>
      <img src alt />
      <div>No, I already have a private key</div>
      <button @click="importPrivateKey">Import private key</button>
    </div>
    <div class="disabled">
      <img src alt />
      <div>No, I already have a 12 word seed phrase</div>
      <button @click="importWallet" class="button-disabled">Import wallet</button>
    </div>
    <div class="disabled">
      <img src alt />
      <div>Yes, let's setup a new wallet and seed phrase</div>
      <button class="button-disabled">Create wallet</button>
    </div>
  </div>
</template>

<script>
import router from "@/index/router";
import AlertHelper from "@/shared/mixins/AlertHelper";

export default {
  mixins: [AlertHelper],
  methods: {
    async importPrivateKey() {
      this.alertClose();
      router.push("/importPrivateKey");
    },

    async importWallet() { },
  },
};
</script>
