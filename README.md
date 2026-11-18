# exercicios-POO

respostas-poo-parte-1-typescript.md
100%
# Respostas — Exercícios POO (Parte 1) — TypeScript

## Exercício 1 — Classe e Objeto
```typescript
class Pessoa {
    nome: string;
    idade: number;

    constructor(nome: string, idade: number) {
        this.nome = nome;
        this.idade = idade;
    }
}

const pessoa = new Pessoa("Ana", 20);
console.log(pessoa.nome);
console.log(pessoa.idade);
```

## Exercício 2 — Construtor
```typescript
class Produto {
    nome: string;
    preco: number;
    estoque: number;

    constructor(nome: string, preco: number, estoque: number) {
        this.nome = nome;
        this.preco = preco;
        this.estoque = estoque;
    }
}

const produto1 = new Produto("Caneta", 2.5, 100);
const produto2 = new Produto("Caderno", 15.0, 40);

console.log(produto1.nome, produto1.preco, produto1.estoque);
console.log(produto2.nome, produto2.preco, produto2.estoque);
```

## Exercício 3 — Métodos
```typescript
class Aluno {
    nome: string;
    nota: number;

    constructor(nome: string, nota: number) {
        this.nome = nome;
        this.nota = nota;
    }

    aprovado(): boolean {
        return this.nota >= 6;
    }
}

const aluno = new Aluno("Carlos", 7.5);
console.log(aluno.aprovado());
```

## Exercício 4 — this / self
```typescript
class Retangulo {
    largura: number;
    altura: number;

    constructor(largura: number, altura: number) {
        this.largura = largura;
        this.altura = altura;
    }

    calcularPerimetro(): number {
        return 2 * (this.largura + this.altura);
    }
}

const retangulo = new Retangulo(5, 3);
console.log(retangulo.calcularPerimetro());
```

## Exercício 5 — Modificadores de acesso
```typescript
class ContaBancaria {
    private saldo: number = 0;

    depositar(valor: number): void {
        if (valor > 0) this.saldo += valor;
    }

    consultarSaldo(): number {
        return this.saldo;
    }
}

const conta = new ContaBancaria();
conta.depositar(100);
console.log(conta.consultarSaldo());
```
Exibindo respostas-poo-parte-1-typescript.md…
