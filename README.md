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

    Algunos en la próxima clase han presentado este problema con el CRLF, no es nada serio, es  básicamente una interpretación de un carácter.
    Simplemente ejecuten este comando si presentan el error:
    
    git config core.autocrlf true
}

Restaurar el ultimo commit {

    git checkout -- .
}

Revisar los commits {
    git log
}

Realizar git add . a archivos comunes {

    git add *.html (extención del archivo cuando esta en la raiz)
    git add js/*.js (extención del archivo cuando esta dentro de una carpeta)
}

Nota: Git no le dara seguimiento a una carpeta vacia de fotma predeterminada, para evitar esto, dentro de la carpeta podemos generar un archivo llamado .gitkeep

Creando alias en los comandos de git{

    git config --global alias.(aqui abreviamos y depues colocamos el comando correcto)

    git config --global alias.s "status --short"
}

Nota: git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"

Revisar las modificaciones realidas en los archivos {

    git diff (Compara los cambios que aun no estan en el staged)

    git diff --staged (comparar los datos de staged)
}

git commit -am "" // podemos usas este comando corto para realizar el commit, siempre que le estemos dando seguimiento al archivo.

git commit --amend -m "" //Comando para corregir el ultimo commit.

 git reset --soft HEAD^  //Comando para borrar el ultimo commit
 

