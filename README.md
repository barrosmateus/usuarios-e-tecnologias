# usuarios-e-tecnologias
desafio 

const usuarios = [
    {nome: 'carlos', tecnologias: ["HTML", "CSS"] },
    {nome: 'daniela', tecnologias: ["java", "php"] },
    {nome: 'priscila', tecnologias:["javascript", "CSS"]},
    {nome: 'divina', tecnologias: ["python"] },
    {nome: 'maria', tecnologias: ["java", "javascript", "csS"] },
    {nome: 'ester', tecnologias:["javascript", "CSS"]}
]
//para cada individuo do array usuarios ...
for ( let individuosdoarray of usuarios) {
    //mostre na tela...
    //join == mostra os individuos do array como string e separa com a pontuaçao que for colocada entre as aspas dentro do parentesis
    console.log (`usuario(a) ${individuosdoarray.nome} usa as tecnologias ${individuosdoarray.tecnologias.join(',')}`)
}

console.log('==================================================================')
function checaSeUsuarioUsaCSS(){
    for (let individuosdoarray of usuarios) {
        // se nos individuos do Array tiverem "CSS(nesse caso)" retorne verdadeiro
        if (individuosdoarray == "CSS") return true
    }
    //se nao tiverem ... retorne falso
    return false
}
// para a contagem i, onde i é igual a zero, some mais um ao numero da posiçao até i ficar igual a quantidade de usuarios
    for (let i = 0; i < usuarios.length; i++) {
        //cheque se o usuario da posiçao i usa Css
        const usuarioTrabalhaComCSS = checaSeUsuarioUsaCSS(usuarios[i])
        // se o usuario usar
        if (checaSeUsuarioUsaCSS){
            //mostre o usuario e o nome 
            console.log(`o usuario ${usuarios[i].nome} trabalha com CSS`)
            //o i irá assumir e avaliar todos os nomes cadastrados
        }
    }


