<template>
    <div class="container ">
       <h2> Sign In Form</h2>
       <form>
         <input  type="text" class="input-field" placeholder="name" required>
           <input  type="email" class="input-field" placeholder="Email" required>
           <input  type="password" class="input-field" placeholder="Password" required>
           <button @click="handleAlertClick" type="submit" class="btn">Sign In</button>
           <br/>
           <br/>
           <br/>
       </form>
   </div>
</template>

<script>
import Swal from 'sweetalert2';

export default {
    name: 'SweetAlert2',
    methods:{
        handleAlertClick(){ 
         Swal.fire({
  title: "Good job!",
  text: "You clicked the button!",
  icon: "success",
});
        }
},
}

</script>
<style >

.container {
   margin-left: 595px;
   margin-top: 150px;
   background: rgba(255, 255, 255, 0.9);
   padding: 25px;
   border-radius: 12px;
   box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
   width: 320px;
   text-align: center;
   font-family: 'Poppins', sans-serif;
}

.container h2 {
   margin-bottom: 20px;
   color: #ffa600;
   font-weight: bold;
}

.input-field {
   width: 100%;
   padding: 12px;
   margin: 10px 0;
   border: 1px solid #ccc;
   border-radius: 6px;
}

.btn {
   width: 100%;
   padding: 12px;
   background: #ffa600;
   color: #fff;
   border: none;
   border-radius: 6px;
   cursor: pointer;
   font-size: 16px;
   transition: 0.3s;
}

.btn:hover {
   background: #edce33;
}

.link {
   display: block;
   margin-top: 12px;
   text-decoration: none;
   color: #ffa600;
   font-weight: bold;
}
</style>