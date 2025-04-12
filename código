function calcularRanking(medalhas) {

    const ranking = Object.entries(medalhas).sort((a, b) => b[1] - a[1]);

    console.log("\n #Ranking de medalhas#: ");

    ranking.forEach(([pais, total]) => {

        console.log(`\n #${pais}: ${total} medalhas`);
    });
}

function main() {

    const medalhas = {};

    while (true) {

        const pais = prompt("\n Digite o nome do país (ou 'sair' para finalizar): ");

        if (pais.toLowerCase() === 'sair') {
            break;

        }

        const ouro = parseInt(prompt(`\n Digite o número de medalhas de ouro para ${pais}: `), 10);
        const prata = parseInt(prompt(`\n Digite o número de medalhas de prata para ${pais}: `), 10);
        const bronze = parseInt(prompt(`\n Digite o número de medalhas de bronze para ${pais}: `), 10);
        
        const total = ouro + prata + bronze;

        medalhas[pais] = total;
    }

    calcularRanking(medalhas);
    
}

main();
