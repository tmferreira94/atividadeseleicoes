let votes = [];

let addvotes = (vote) => {
    if (vote>= 1 && vote<= 4){
        votes.push(vote);
        console.log(`voto para o canditado ${vote}adcionado.`);
        
        }else{
            console.log('numero invalido .vote em um candidato de 1 a 4.');


        }
    };
let listaVotes = () => {
    console.log("votos registrados:");
    votes .forEach((vote,index) =>{
        console.log(`voto ${index + 1} :candidato${vote}`);
    });
};
let updatevote = (index,newVote) => {
    if (index >= 0 && index <votes.length){
        if (newVotes >= 1 && newVote <= 4){
            votes [index]= newVote;
            console.log(`voto atualizado para o candidato $ {newVote}.`);
        }else{
            console.log.apply('numero invalido.vote em umm candidato de 1 a 4.');

        }
    }else{
console.log.apply('indice invalido');
    }
        };
        let deleteVote = (index) =>{
            if (index >= 0 && index < votes.length){
                votes.concat.splice(index,1);
                console.log('voto removido');
            }else{
                console.log('indice invalido');
            }
            };
 
