//---------------------------------------------------------------//
function validaNombre() {
    var cajaNombre = document.getElementById('nombre');
    var correctoNombre = /^[A-Za-z\s]+$/;
    var errorNombre = document.getElementById('nombreError');

    if (cajaNombre.value == 0) {
        errorNombre.innerHTML = "Rellene este campo";
        cajaNombre.classList.add("incorrecto");
        cajaNombre.classList.add("iconoincorrecto");
        return false;
    }
    else if (correctoNombre.test(cajaNombre.value)) {
        cajaNombre.classList.remove("incorrecto");
        cajaNombre.classList.remove("iconoincorrecto");
        errorNombre.innerHTML = "";
        cajaNombre.classList.add("correcto");
        cajaNombre.classList.add("iconocorrecto");
        return true;
    }
    else {
        errorNombre.innerHTML = "Nombre inválido";
        cajaNombre.classList.add("incorrecto");
        cajaNombre.classList.add("iconoincorrecto");
        return false;
    }
}

//---------------------------------------------------------------//

function validaEmail() {
    var cajaEmail = document.getElementById('email');
    var correctoEmail = /^\w+([.-_+]?\w+)*@\w+([.-]?\w+)*(\.\w{2,10})+$/;
    var errorEmail = document.getElementById('emailError');

    if (cajaEmail.value == 0) {
        errorEmail.innerHTML = "Rellene este campo";
        cajaEmail.classList.add("incorrecto");
        cajaEmail.classList.add("iconoincorrecto");
        return false;
    }
    else if (correctoEmail.test(cajaEmail.value)) {
        cajaEmail.classList.remove("incorrecto");
        cajaEmail.classList.remove("iconoincorrecto");
        errorEmail.innerHTML = "";
        cajaEmail.classList.add("correcto");
        cajaEmail.classList.add("iconocorrecto");
        return true;
    }
    else {
        errorEmail.innerHTML = "Email inválido";
        cajaEmail.classList.add("incorrecto");
        cajaEmail.classList.add("iconoincorrecto");
        return false;
    }
}

//---------------------------------------------------------------//

function validaContrasena() {
    var cajaContrasena = document.getElementById('contrasena');
    var correctoContrasena = /^[\s\S]{1,8}$/;
    var errorContrasena = document.getElementById('contrasenaerror');

    if (cajaContrasena.value == 0) {
        errorContrasena.innerHTML = "Rellene este campo";
        cajaContrasena.classList.add("incorrecto");
        cajaContrasena.classList.add("iconoincorrecto");
        return false;
    }
    else if (correctoContrasena.test(cajaContrasena.value)) {
        cajaContrasena.classList.remove("incorrecto");
        cajaContrasena.classList.remove("iconoincorrecto");
        errorContrasena.innerHTML = "";
        cajaContrasena.classList.add("correcto");
        cajaContrasena.classList.add("iconocorrecto");
        return true;
    }
    else {
        errorContrasena.innerHTML = "No debe tener más de 8 caracteres";
        cajaContrasena.classList.add("incorrecto");
        return false;
    }
}

//---------------------------------------------------------------//

function validaConfirmar() {
    var cajaContrasena = document.getElementById('contrasena');
    var cajaConfirmar = document.getElementById('confirmar');
    var errorConfirmar = document.getElementById('confirmarerror');

    if (cajaConfirmar.value == 0) {
        errorConfirmar.innerHTML = "Rellene este campo";
        cajaConfirmar.classList.add("incorrecto");
        cajaConfirmar.classList.add("iconoincorrecto");
        return false;
    }
    else if (cajaContrasena.value == cajaConfirmar.value) {
        cajaConfirmar.classList.remove("incorrecto");
        cajaConfirmar.classList.remove("iconoincorrecto");
        errorConfirmar.innerHTML = "";
        cajaConfirmar.classList.add("correcto");
        cajaConfirmar.classList.add("iconocorrecto");
        return true;
    }
    else {
        errorConfirmar.innerHTML = "Las contraseñas no coinciden";
        cajaConfirmar.classList.add("incorrecto");
        cajaConfirmar.classList.add("iconoincorrecto");
        return false;
    }
}

//---------------------------------------------------------------//

function validaForm() {

    if (validaConfirmar() && validaContrasena() && validaEmail() && validaNombre()) {
        alert("La inscripción ha sido correcta");
        return true;
    }
    else {
        return false;
    }
}
