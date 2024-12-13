<script lang="ts">
  import logo from '../assets/logo.png';

  let nombre: string = "";
  let email: string = "";
  let matricula: string = "";
  let telefono: string = "";
</script>
<div class="contenedor1">
 
  <div class="contenedor2">
    <div class="logo">
      <img src="{logo}" alt="Logo" />
    </div>
    <div class="form-cont">
      <h1>Crear Cuenta</h1>
      <input type="text" bind:value={nombre} placeholder="Nombre y Apellidos" />
      <input type="email" bind:value={email} placeholder="Email" />
      <input type="text" bind:value={matricula} placeholder="Matrícula" />
      <input type="tel" bind:value={telefono} placeholder="Teléfono" />
      <button>Crear Cuenta</button>
    </div>
  </div>
</div>
<style>
  .contenedor1{
    background-color: black;
    height: 630px;  
    width: 370px;
  }
  h1{
    color: black;
  }
  .contenedor2{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 600px;  
  }

  .form-cont {
    background: rgba(255, 255, 255, 0.9);
    border-radius: 8px;
    padding: 20px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    width: 230px;
    text-align: center;
  }

  .form-cont h1 {
    font-size: 24px; 
    margin-bottom: 16px; 
  }

  .form-cont input {
    width: 100%;
    padding: 10px;
    margin: 8px 0;  
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
  }

  .form-cont button {
    background-color: #333;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px; 
    width: 100%;
    margin-top: 16px;  
  }

  .form-cont button:hover {
    background-color: #555;
  }

  .logo {
    display: flex;
    justify-content: center;
    margin-bottom: 16px;  
  }

  .logo img {
    width: 80px;
  }
</style>
