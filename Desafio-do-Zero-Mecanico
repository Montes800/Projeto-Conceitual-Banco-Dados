classDiagram
direção LR
classe Cliente {
-id: String
-nome: String
-contato: String
}

class Veiculo {
    -placa: String
    -modelo: String
    -marca: String
    -ano: Integer
}

class Mecanico {
    -codigo: String
    -nome: String
    -endereco: String
    -especialidade: String
}

class Equipe {
    -id: String
    -nome: String
}

class OrdemDeServico {
    -numero: String
    -dataEmissao: Date
    -dataConclusao: Date
    -status: String
    -valorTotal: Double
    +calcularValor()
    +cancelarOS()
}

class Servico {
    -id: String
    -descricao: String
    -valor: Double
}

class Peca {
    -id: String
    -nome: String
    -valor: Double
}

Cliente "1" -- "0..*" Veiculo: possui
Cliente "1" -- "0..*" OrdemDeServico: abre

Veiculo "1" -- "1" Cliente: pertence a
Veiculo "1" -- "0..*" OrdemDeServico: associado a

Mecanico "1..*" -- "1" Equipe: pertence a
Equipe "1" -- "0..*" OrdemDeServico: designada a

OrdemDeServico "1" -- "1..*" Servico: contém
OrdemDeServico "1" -- "1..*" Peca: utiliza

Servico "0..*" -- "0..*" OrdemDeServico: contido em
Peca "0..*" -- "0..*" 
