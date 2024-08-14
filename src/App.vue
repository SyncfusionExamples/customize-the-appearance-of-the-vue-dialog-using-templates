<script setup>
import {DialogComponent as EjsDialog} from '@syncfusion/ej2-vue-popups';

</script>

<template>

<ejs-dialog height="200px" width="370px" :header="'headerTemplate'" :content="'contentTemplate'"
:footerTemplate="'footerTemplate'"
showCloseIcon="true">
<template v-slot:headerTemplate>
  <div class="header">
    <img class="image" src="\logo.png" />   
    <span id="template"> Syncfusion </span>
  </div>
</template>
<template v-slot:contentTemplate>
    <div class="content">  
       <span class="dialogText">Want to be alerted when our videos are published? Enter your mail address to be the first notified!</span>
      </div>
 </template>
<template v-slot:footerTemplate>
  <div class="footer">
  <input id='textbox' class='e-input' placeholder='Enter your mail id'/>
  <button class='e-info e-btn'>SUBSCRIBE</button>
</div>
</template>
</ejs-dialog>
</template>

<style scoped>
@import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-popups/styles/material.css";
@import "../node_modules/@syncfusion/ej2-buttons/styles/material.css";
 #template {
   font-weight: bold;
   font-size:20px;
   margin:6px; 
}
.image{
        width: 40px;
        height: 35px;
    } 
    .header{
  display:inline-flex;
}

.content {
  font-family: serif;
  font-size: 16px;
}
#textbox {
    float: left;
    width: 65%;
    padding:2px;
}
.footer{
  padding: 10px;
}
</style>

