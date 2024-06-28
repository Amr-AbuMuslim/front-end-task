<template>
  <div class="home">
    <MainSection></MainSection>
    <NFTCard
      title="Moddy Character NFT"
      details="The image is a high-quality digital painting with a resolution of 3000x2000 pixels and is optimized for the web."
      price="$101,593"
    ></NFTCard>
    <NFTCard2
      title="KattyEfa NFT"
      details="The image is a high-quality digital painting with a resolution of 5000x1250 pixels ."
      price="$1.5 million"
    ></NFTCard2>
    <CollectionGal></CollectionGal>
    <FooterPage></FooterPage>
  </div>
</template>

<script>
// @ is an alias to /src
import MainSection from "../components/MainSection.vue";
import NFTCard from "../components/NFTCard.vue";
import NFTCard2 from "../components/NFTCard2.vue";
import CollectionGal from "../components/CollectionGal.vue";
import FooterPage from "../components/FooterPage.vue";

export default {
  name: "HomeView",
  components: {
    MainSection,
    NFTCard,
    NFTCard2,
    CollectionGal,
    FooterPage,
  },
};
</script>
