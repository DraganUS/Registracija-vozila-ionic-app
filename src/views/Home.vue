<template>
  <div class="ion-page">
    <ion-header>
      <ion-toolbar color="dark">
       <h1>Registracija Vozila </h1>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      
   <ion-item>
      <ion-label>Izaberite opštinu:<span>*</span></ion-label>
      <ion-select value="Putničko"  okText="Okay" cancelText="Dismiss" required>
         <ion-select-option value="1" > Barajevo</ion-select-option>
         <ion-select-option value="2" >Čukarica</ion-select-option>
         <ion-select-option value="3" >Grocka</ion-select-option>
         <ion-select-option value="14" >Lazarevac</ion-select-option>
         <ion-select-option value="16" >Mladenovac</ion-select-option>
         <ion-select-option value="4" >Novi Beograd</ion-select-option>
         <ion-select-option value="5" >Obrenovac</ion-select-option>
         <ion-select-option value="6" >Palilula</ion-select-option>
         <ion-select-option value="17" >Rakovica</ion-select-option>
         <ion-select-option value="7" >Savski Venac</ion-select-option>
         <ion-select-option value="8" >Sopot</ion-select-option>
         <ion-select-option value="9" >Stari Grad</ion-select-option>
         <ion-select-option value="18" >Surčin</ion-select-option>
         <ion-select-option value="10" >Voždovac</ion-select-option>
         <ion-select-option value="11" >Vračar</ion-select-option>
         </ion-select>
     </ion-item>

     <ion-item >
      <ion-label>Vrsta vozila:<span>*</span></ion-label>
      <ion-select @ionChange='tipVozila=event.target.value' :value="tipVozila" okText="Okay" cancelText="Dismiss">
        <ion-select-option @ionChange='tipVozila=event.target.value' @click="promenaTipVozila()"  value="putnicko">Putničko</ion-select-option>
        <ion-select-option @ionChange='tipVozila=event.target.value' value="teretno">Teretno</ion-select-option>
        <ion-select-option @ionChange='tipVozila=event.target.value' value="motocikli">Motocikli</ion-select-option>
      </ion-select>
    </ion-item>   
    
      <ion-item v-if="tipVozila=='teretno'">
        <ion-label position="floating">Tezina <span>*</span></ion-label>
        <ion-input type="number" description="numeric"></ion-input>
      </ion-item>
    <!-- Ako se izabere teretno vozilo doda se nova kolona nosivost -->

    <ion-item>
    <ion-label>Godište: <span>*</span></ion-label>
    <ion-datetime display-format="YYYY" picker-format="YYYY" ></ion-datetime>
    </ion-item>
    
     <ion-item>
        <ion-label  position="floating">Snaga motora u KW: <span>*</span></ion-label>
        <ion-input  type="number" description="numeric"></ion-input>
      </ion-item>

        <ion-item>
        <ion-label position="floating">Zapremina motora: <span>*</span></ion-label>
        <ion-input type="number" description="numeric"></ion-input>
      </ion-item>

    <ion-item>
      <ion-label> Premijski stepen:<span>*</span></ion-label>
      <ion-select value="" okText="Okay" cancelText="Dismiss">
        <ion-select-option value="newCar">Tek nabvljeno vozilo</ion-select-option>
        <ion-select-option value="1">1</ion-select-option>
        <ion-select-option value="2">2</ion-select-option>
        <ion-select-option value="3">3</ion-select-option>
        <ion-select-option value="4">4</ion-select-option>
        <ion-select-option value="5">5</ion-select-option>
        <ion-select-option value="6">6</ion-select-option>
        <ion-select-option value="7">7</ion-select-option>
        <ion-select-option value="8">8</ion-select-option>
        <ion-select-option value="9">9</ion-select-option>
        <ion-select-option value="10">10</ion-select-option>
        <ion-select-option value="11">11</ion-select-option>
        <ion-select-option value="12">12</ion-select-option>
      </ion-select>
    </ion-item> 

      <ion-item>
      <ion-label> Koliko ste šteta imali:<span>*</span></ion-label>
      <ion-select value="" okText="Okay" cancelText="Dismiss">
        <ion-select-option value="0">0</ion-select-option>
        <ion-select-option value="1">1</ion-select-option>
        <ion-select-option value="2">2</ion-select-option>
        <ion-select-option value="3">3</ion-select-option>
        <ion-select-option value="4">4</ion-select-option>
        <ion-select-option value="5">5</ion-select-option>
        <ion-select-option value="6">6</ion-select-option>
        <ion-select-option value="7">7</ion-select-option>
        <ion-select-option value="8">8</ion-select-option>
        <ion-select-option value="9">9</ion-select-option>
        <ion-select-option value="10">10</ion-select-option>
        <ion-select-option value="11">11</ion-select-option>
        <ion-select-option value="12">12</ion-select-option>
      </ion-select>
    </ion-item> 

   <ion-list>  
   <div id="saobracajna">
    <ion-item> 
      <ion-label>Vozilo se vodi na firmu</ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
    <ion-item> 
      <ion-label>Vozilo kupljeno na lizing</ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
      <ion-item> 
      <ion-label> Vozilo je TAXI</ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
      <ion-item> 
      <ion-label>TAXI vozilo ima atestiran plinski uredaj</ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
    <ion-item> 
      <ion-label>Vlasnik vozila invalid preko 80%</ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
    <ion-item> 
      <ion-label>Vozilo u vlasništvu rent-a-car firme </ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
    </div>
 </ion-list>


 <ion-list>
   <div id="saobracajna">
    <ion-item> 
      <ion-label>Potrebna mi je nova saobraćajna </ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
      <ion-item> 
      <ion-label>Potrebne su mi tablice  </ion-label>
      <ion-checkbox color="dark"></ion-checkbox>
    </ion-item>
    </div>
 </ion-list>

     <ion-col class="ion-margin-top">  
        <ion-button expand="block" color="dark" fill="outline" >Izračunaj</ion-button>
     </ion-col>
    </ion-content>
  </div>
</template>

<style scoped>
span{
  color: red;
}
ion-toolbar{
  --ion-background-color: rgba(45, 45, 45, 0.98); 
  color: #fffffe;
  text-align: center;
}
.alert-ios .alert-wrapper, .alert-md .alert-wrapper,.alert-wrapper{
  width: 100% !important;
  max-width: unset !important;
}
#saobracajna{
  margin-top: 10px;
  border: 1px solid black;
}
.ion-margin-top{
  margin-top: 16px;
}
</style>


<script>

export default {
  name: "home",
   data() {
     return{
        opstina: 1,
        tipVozila: '',
        promenaTipVozila: ''
     }
    },
     methods: {
       promenaTipVozila: function(){
        this.promenaTipVozila='sasd';
     }
  },
};
</script>