<template>
  <div class="home">
    <barcode-scaner @onLoad="onLoad($event)" @onDecode="onDecode($event)" @onError="onError($event)"/>

    <span>SCANER BARCODE</span> <br/><br/>
    <span>{{ scaneado }}</span>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class HomeView extends Vue {
  scaneado: string = "";
  onLoad(val: any){
    alert("LOAD: " + val);
  }
  onDecode(val: any){
    alert("LOAD: " + val);
  }
  onError(val: any){
    alert("LOAD: " + val);
  }
}
</script>
