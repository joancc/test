<template>
  <div class="item company">
    <button class="select-item">
      <div class="info">
        <p>
          <strong v-if="keyType == 'RFC'">{{enterpriseName}}</strong>
          <strong v-else-if="keyType == 'Clave'">{{warehouseTitle}}</strong>
          <span class="on"></span>
          <span v-if="keyType == 'RFC'">{{keyType}}: {{rfc}}</span>
          <span v-else-if="keyType == 'Clave'">{{keyType}}: {{warehouseKey}}</span>
        </p>
      </div>
    </button>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      enterpriseName:
        "Empresa no patito S.A de C.V Empresa no patito S.A de C.V Empresa no patito S.A de C.V Empresa no patito S.A de C.V Empresa no patito S.A de C.V",
      keyType: "RFC",
      rfc: "POASHF12434",
      warehouseKey: "90078434",
      warehouseTitle: "Almacén Sonora Grill"
    };
  }
};
</script>

