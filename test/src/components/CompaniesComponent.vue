<template>
  <div class="column companies is-half">
    <EnterpriseBanner></EnterpriseBanner>
    <ItemCompany></ItemCompany>
    <ItemCompanyDisabled></ItemCompanyDisabled>
    <ItemCompany></ItemCompany>
  </div>
</template>

<script>
import EnterpriseBanner from "./EnterpriseBanner.vue";
import ItemCompany from "./ItemCompany.vue";
import ItemCompanyDisabled from "./ItemCompanyDisabled";

export default {
  components: {
    EnterpriseBanner: EnterpriseBanner,
    ItemCompany: ItemCompany,
    ItemCompanyDisabled: ItemCompanyDisabled
  }
};
</script>

