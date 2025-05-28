# Ferramenta de Controle de Investimentos em Excel - FIIs

## Sobre o Projeto

Esta ferramenta foi desenvolvida para simular investimentos em Fundos Imobiliários (FIIs), permitindo aos usuários calcular projeções e distribuir investimentos de acordo com diferentes perfis de risco.

## Principais Funcionalidades

### 1. Cálculo de Projeções

- Utiliza a fórmula de juros compostos: VF = VP * (1 + i)^t
- Considera aportes mensais fixos
- Projeta resultados para 3, 5, 10, 20 e 30 anos
- Calcula rendimentos mensais esperados

### 2. Distribuição por Perfil de Investidor

Implementa três perfis de risco com alocações específicas:

### Conservador

- PAPEL: 30%
- TIJOLO: 50%
- HÍBRIDOS: 10%
- FOFs: 10%
- DESENVOLVIMENTO: 0%
- HOTELARIAS: 0%

### Moderado

- PAPEL: 32%
- TIJOLO: 35%
- HÍBRIDOS: 8%
- FOFs: 5%
- DESENVOLVIMENTO: 10%
- HOTELARIAS: 10%

### Agressivo

- PAPEL: 50%
- TIJOLO: 10%
- HÍBRIDOS: 5%
- FOFs: 5%
- DESENVOLVIMENTO: 20%
- HOTELARIAS: 10%

## Fórmulas Utilizadas

1. Cálculo de Valor Futuro:

```
PMT * (((1 + taxa)^(anos * 12) - 1) / taxa)
```

1. Cálculo de Rendimento Mensal:

```
Valor_Futuro * Taxa_Rendimento_Mensal
```

1. Distribuição por Tipo de FII:

```
Valor_Mensal * Percentual_Alocação
```

## Como Usar

- Selecione seu perfil de investidor
- Insira o valor mensal a ser investido
- A planilha calculará automaticamente:
    - Projeções de valor futuro
    - Rendimentos mensais esperados
    - Distribuição por tipo de FII
