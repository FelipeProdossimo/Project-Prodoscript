# Prodoscript

---

## Miro com a documentação do projeto 

[Exemples](https://miro.com/app/board/o9J_lBMxbWc=/) 

---

## Documentação.

* Baixar Git, Github CLI, basta instalar...
* Faça login em sua Conta Github utilizando a [Documentação](https://github.com/cli/cli#installation) do GitCLI.

### Tecnologias.

* A decidir;

### Pré-requisitos minimos.

* 8GB RAM;
* I5 ou compatível;

## SQL - Banco de dados 


### Criação do banco de dados

```

CREATE DATABASE db_exemples

```

### Criação da tabela de clientes

```

CREATE TABLE `tb_clientes` ( 

  `id` int(11) NOT NULL, 

  `nome` varchar(100) NOT NULL, 

  `email` varchar(70) NOT NULL, 

  `telefone` varchar(20) NOT NULL, 

  `senha` varchar(30) NOT NULL 

) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4; 

```

### Criação de Indíces para tables despejadas

#### Table de Clientes

```

ALTER TABLE `tb_clientes` 
  ADD PRIMARY KEY (`id`); 

```

#### Table de Itens

```

ALTER TABLE `tb_itens` 
  ADD PRIMARY KEY (`id`), 
  ADD KEY `fk_itens_vendedores` (`id_vendedor`); 

```
