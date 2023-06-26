# Notas

Configuracion de email y usuario git {

    git config --global user.name ""
    git config --global user.email ""

    Comprobar email y usuario (

        git configg --global -e
        
        Al presionar la tecla a, nos permide editar email y usuario,
        para salir y guardar:

        Esc , :wq! Enter
    )
}

Inicializar repositorio {

    git init
}

Informacion sobre los commits, ramas y estados {

    git status
}

Guardar modificaciones {

    git add .                           //prepara todos los archivos para guardar
    git reset nameArchivo               //no guarda el archivo indicado
    git commit -m "nombre del commit"   //guarda el estado de los archivos
}

Nota de actualización {

    Algunos en la próxima clase han presentado este problema con el CRLF, no es nada serio, es básicamente una interpretación de un carácter.
    Simplemente ejecuten este comando si presentan el error:
    
    git config core.autocrlf true
}

Restaurar el ultimo commit {

    git checkout -- .
}

Revisar los commits {
    git log
}