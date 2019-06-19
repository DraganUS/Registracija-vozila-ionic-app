<template>
  <div class="ion-page">
    <ion-header>
      <ion-toolbar color="dark">
       <h1>Registracija Vozila </h1>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      
        <ion-item>
          <ion-label position="floating">Unesite Vaše</ion-label>
          <ion-input type="text" placeholder="Ime"></ion-input>
        </ion-item>
        <ion-item>
          <ion-label position="floating">Unesite Vaše Prezime</ion-label>
           <ion-input type="text" placeholder="Prezime"></ion-input>
        </ion-item>

   <ion-item>
      <ion-label>Izaberite opštinu:<span>*</span></ion-label>
      <ion-select value="Putničko" okText="Okay" cancelText="Dismiss" required>
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

     <ion-item>
      <ion-label>Vrsta vozila:<span>*</span></ion-label>
      <ion-select value="Putničko" okText="Okay" cancelText="Dismiss">
        <ion-select-option value="brown">Putničko</ion-select-option>
        <ion-select-option value="blonde">Teretno</ion-select-option>
        <ion-select-option value="black">Motocikli</ion-select-option>
        <ion-select-option value="red">Priklkucno</ion-select-option>
      </ion-select>
    </ion-item>   

    <ion-item>
    <ion-label>Godište: <span>*</span></ion-label>
    <ion-datetime display-format="YYYY" picker-format="YYYY" ></ion-datetime>
    </ion-item>
    
     <ion-item>
        <ion-label position="floating">Snaga motora u KW: <span>*</span></ion-label>
        <ion-input type="number" description="numeric"></ion-input>
      </ion-item>

        <ion-item>
        <ion-label position="floating">Zapremina motora: <span>*</span></ion-label>
        <ion-input type="number" description="numeric"></ion-input>
      </ion-item>

    <ion-item >
      <ion-label>Ostali podaci:</ion-label>
      <ion-select  multiple="true" cancelText="Cancel" okText="Ok">
        <ion-select-option  value="1">Vodi na firmu</ion-select-option>
        <ion-select-option value="2">Kupljeno na lizing</ion-select-option>
        <ion-select-option value="3">Vozilo je TAXI</ion-select-option>
        <ion-select-option value="4">TAXI ima atest plinski uredaj</ion-select-option>
        <ion-select-option value="5">Vlasnik invalid preko 80%</ion-select-option>
        <ion-select-option value="5">Vlasništvo rent-a-car</ion-select-option>
      </ion-select>
    </ion-item>

    

    <ion-item>
      <ion-label>Saobracajne i tablice:</ion-label>
      <ion-select multiple="true" cancelText="Cancel" okText="Ok">
        <ion-select-option value="1"> + nova saobraćajna</ion-select-option>
        <ion-select-option value="2"> + tablice </ion-select-option>
      </ion-select >
    </ion-item>
 



<div mbsc-form>
    <div class="mbsc-grid mbsc-form-grid">
        <div class="mbsc-row">
            <div class="mbsc-col-sm-12 mbsc-col-md-6">
                <label>
                    Mobile
                    <select name="City" id="demo-multiple-lines" data-input-style="box" data-label-style="stacked">
                        <option value="1">Percentage of assets covered by systematic risk assessments (>99)</option>
                        <option value="2">Number of personal vacancies in the security roles required for ISMS (Nil)</option>
                        <option value="3">Time taken to grant, change and remove access privileges (Max. 2 hours)</option>
                        <option value="4">Percentage of agents covered by an effective security awareness program (100%)</option>
                        <option value="5">Number of security access violations (<2)</option>
                        <option value="6">Number of emergency changes (<5)</option>
                        <option value="7">Number of security incidents involving malicious code (Max. 2)</option>
                        <option value="8">Number of systems where security requirements are not met (Max. 2)</option>
                        <option value="9">Average turnaround time of incidents (Max. 2 hours)</option>
                        <option value="10">Number of pending actions to meet response and recovery requirements (Max. 5)</option>
                        <option value="11">Number of scheduled internal audits not done (Max. 1)</option>
                        <option value="12">Number of scheduled penetration tests not done (Max. 1)</option>
                        <option value="13">Number of overdue actions arising out of audit reports (Max. 5)</option>
                        <option value="14">Number of changes not carried out as per change control procedure (Max. 1)</option>
                    </select>
                </label>
            </div>
            <div class="mbsc-col-sm-12 mbsc-col-md-6">
                <label>
                    Desktop
                    <select name="City" id="demo-multiple-lines-desktop" data-input-style="box" data-label-style="stacked">
                        <option value="1">Percentage of assets covered by systematic risk assessments (>99)</option>
                        <option value="2">Number of personal vacancies in the security roles required for ISMS (Nil)</option>
                        <option value="3">Time taken to grant, change and remove access privileges (Max. 2 hours)</option>
                        <option value="4">Percentage of agents covered by an effective security awareness program (100%)</option>
                        <option value="5">Number of security access violations (<2)</option>
                        <option value="6">Number of emergency changes (<5)</option>
                        <option value="7">Number of security incidents involving malicious code (Max. 2)</option>
                        <option value="8">Number of systems where security requirements are not met (Max. 2)</option>
                        <option value="9">Average turnaround time of incidents (Max. 2 hours)</option>
                        <option value="10">Number of pending actions to meet response and recovery requirements (Max. 5)</option>
                        <option value="11">Number of scheduled internal audits not done (Max. 1)</option>
                        <option value="12">Number of scheduled penetration tests not done (Max. 1)</option>
                        <option value="13">Number of overdue actions arising out of audit reports (Max. 5)</option>
                        <option value="14">Number of changes not carried out as per change control procedure (Max. 1)</option>
                    </select>
                </label>
            </div>
        </div>
    </div>
</div>


     <ion-col class="ion-margin-top">
      <div>
        <ion-button expand="block" color="dark" fill="outline" >Izračunaj</ion-button>
      </div>
     </ion-col>
       <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
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

.alert-ios .alert-radio-label {white-space: pre-line !important;}
.alert-md .alert-radio-label  {white-space: pre-line !important;}
.alert-wp .alert-radio-label  {white-space: pre-line !important;}
.select-text {white-space: pre-line !important;}
/* .ios {
  --ion-background-color: #222;
  color: #fffffe;
}
.ios ion-toolbar{
  color: #222;
}
.ios ion-button{
  color: #fffffe;
} */
.ion-margin-top{
  margin-top: 16px;
}
/* #fafafa */
</style>


<script>

export default {
  name: "home",
   data: {
    opstina: 1
  },
};
</script>