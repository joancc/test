<template>
  <div class="item company">
    <button class="select-item">
      <div class="info">
        <p>
          <strong>{{enterpriseName}}</strong>
          <span class="on"></span>
          <span>{{keyType}}: {{rfc}}</span>
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

