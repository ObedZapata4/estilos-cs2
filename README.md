# estilos-cs2

@import url('https://fonts.googleapis.com/css2? family= Open+Sans &familia = Roboto & display=swap');

*{
    margin: 0;
    
    text-decoration: none;
    list-style: none;
    
    
    
}

body{
    
    background-color: #f5f5f5;
    

}    

a, li{
    font-family: 'Roboto', sans-serif;
    color: #fff;
}

.nav_conteiner{
    background-color: #6495ED;
    display: flex;
    height: 100%;
    width: 90%;
    margin: 0 auto;
    justify-content: space-between;
    align-items: center;
    padding: .5rem 7rem;
    --clippy: polygon(0 0, 0 0, 0 100%, 0% 100%);
    
}

.nav_menu ul{
    display: flex;
    align-items: center;
    
}

.nav_menu li{
    margin-right: 1.5rem;
}

.nav_menu li:last-child{
    background-color: #1E90FF;
    border: 2px solid #ffff;
    padding: .25rem .75rem;
    border-radius: .2rem;
    
}
.nav_menu
li:last-child:hover{
    background: transparent;
    border: 2px solid #fff;
}

.nav_menu li:first-child
::after{
    content: "";
    display: block;
    background: #fff;
    width: 90%;
    margin-top: 3px;
    height: 3px;
    clip-path: var(--clippy);
    transition: clip-path .20s;
}

.nav_menu li:first-child
:hover{
    --clippy: polygon(0 0, 100% 0, 100% 100%, 0 100%);
}



/*Barra Scroll*/

.barra::-webkit-scrollbar{
    width: 7px;
}

.barra::-webkit-scrollbar-thumb{
    background: #111;
    border-radius: 5px;
}

/*Fecha*/

.Fechas {
    position: fixed;
    padding: 15px 30px;
}

/*Barra de busqueda*/

.buscar {
    position: fixed;
    padding: 130px 35px;
}

.buscar input{
   width: 0px;
   height: 20px;
   padding: 0 20px;
   font-size: 15px;
   color: black;
   outline: none;
   border: 1px solid silver;
   border-radius: 30px; 
   transition: all 0.6s ease;
}

.btn {
    position: absolute;
    top: 120px;
    right: 30px;
    background: #3CB371;
    width: 55px;
    height: 55x;
    line-height: 55px;
    text-align: center;
    color: white;
    font-size: 20px;
    border-radius: 50%;
    cursor: pointer;

}

.buscar:hover input{
    width: 150px;
}

.buscar input:focus{
    width: 200px;
}

/*Checkbox*/

.wrap {
    width: 90%;
    max-width: 1000px;
    margin: 5px 15px 5px 220px;
   
}



.formulario {
    padding: 20px;
    border-bottom: 1px solid #1E90FF;
    
}

.formulario input[type="checkbox"]{
    display: none;
   

}


.formulario .checkbox label{
    color: #111;
    padding: 5px 15px 5px 51px;
    display: inline-block;
    position: relative;
    font-size: 1em;
    border-radius: 3px;
    cursor: pointer;
    -webkit-transition: all 0.3s ease;
    -o-transition: all 0.3s ease;
    transition: all 0.3s ease;
    
    
}

.formulario .checkbox label:hover {
    background: rgba(100, 149, 237, 0.1);
}

.formulario .checkbox label::before{
    content: "";
    width: 10px;
    height: 10px;
    display: inline-block;
    background: none;
    border: 3px solid #0774D9;
    border-radius: 50%;
    position: absolute;
    left: 25px;
    top: 4px;
}

.formulario .checkbox label:before {
    border-radius: 3px;
}

.formulario input[type="checkbox"]:checked + label {
    padding: 5px 15px;
    background: #0774D9;
    border-radius: 2px;
    color: #fff;
}

.formulario input[type="checkbox"]:checked + label:before {
    display: none;
}

/*Filtro de barra de busqueda*/

.filtro{
    display: none;
}
