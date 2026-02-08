# 💰 Ferramenta de Investimentos em FIIs

## 🚀 O que é?

Uma **ferramenta interativa estilo aplicativo** para simular e planejar seus investimentos em Fundos Imobiliários (FIIs). Simples, visual e prática!

## ✨ Funcionalidades

### 📱 ABA APP (Principal)

**1. SEU PERFIL**
- Configure seu salário mensal
- Defina o rendimento esperado dos FIIs
- Escolha seu perfil de risco (Conservador, Moderado ou Agressivo)
- Veja a sugestão automática de aporte (30% do salário)

**2. SIMULAÇÃO DE INVESTIMENTO**
- Defina quanto quer investir por mês
- Escolha por quantos anos
- Veja automaticamente:
  - 💰 Patrimônio acumulado total
  - 📊 Total investido
  - 💵 Rendimento total
  - 🎯 Renda mensal estimada

**3. ALOCAÇÃO POR TIPO DE FII**
A ferramenta sugere AUTOMATICAMENTE como dividir seu dinheiro entre:
- 📄 Papel (CRI/CRA)
- 🏢 Tijolo (Lajes/Shopping)
- 🔄 Híbridos
- 📈 FOFs (Fundos de Fundos)
- 🏗️ Desenvolvimento
- 🏨 Hotelaria

A alocação muda conforme seu perfil!

### 📊 ABA EVOLUÇÃO

Veja a evolução do seu patrimônio ano a ano por até 30 anos:
- Total investido acumulado
- Patrimônio projetado
- Renda mensal em cada ano


## 🎯 Como Usar (3 Passos)

### 1️⃣ Configure Seu Perfil
Na aba **APP**, preencha as células **AZUIS**:
- Salário mensal
- Rendimento esperado (média: 0,60% a 0,80% ao mês)
- Perfil de risco: Conservador, Moderado ou Agressivo

### 2️⃣ Defina Seu Investimento
- Quanto você vai investir por mês?
- Por quantos anos?

### 3️⃣ Veja os Resultados!
Automaticamente você verá:
- Quanto vai acumular
- Quanto vai receber de renda mensal
- Como dividir entre tipos de FII


## 💡 Entenda os Perfis

### 🛡️ CONSERVADOR (Menor Risco)
- 50% em FIIs de Tijolo (estáveis)
- 30% em FIIs de Papel (previsíveis)
- 20% em outros tipos
- ✅ Ideal para quem prioriza segurança

### ⚖️ MODERADO (Equilibrado)
- 35% em FIIs de Tijolo
- 32% em FIIs de Papel
- 33% em outros tipos (inclui desenvolvimento)
- ✅ Ideal para a maioria dos investidores

### 🚀 AGRESSIVO (Maior Retorno)
- 40% em Desenvolvimento (maior risco/retorno)
- 20% em Hotelaria
- 40% distribuído entre outros
- ✅ Ideal para quem aceita volatilidade


## 📊 Tipos de FII Explicados

**📄 Papel (CRI/CRA)**
- Investem em títulos de crédito imobiliário
- Renda mais previsível
- Menor volatilidade

**🏢 Tijolo (Lajes/Shopping)**
- Investem em imóveis físicos
- Aluguéis de escritórios, lojas, galpões
- Tradicional e estável

**🔄 Híbridos**
- Mix de papel e tijolo
- Diversificação em um só fundo

**📈 FOFs**
- Fundos que investem em outros FIIs
- Diversificação automática

**🏗️ Desenvolvimento**
- Constroem e vendem imóveis
- Maior potencial de retorno
- Mais arriscado

**🏨 Hotelaria**
- Investem em hotéis e resorts
- Afetados por sazonalidade
- Potencial de crescimento


## 🔧 Dicas de Uso

### ✅ FAÇA
- Use rendimentos realistas (0,60% a 0,80%/mês)
- Ajuste seu perfil conforme sua tolerância ao risco
- Simule diferentes cenários mudando o período
- Veja a aba "Evolução" para projeções de longo prazo

### ❌ EVITE
- Rendimentos irrealistas (acima de 1,5%/mês)
- Investir mais de 30-40% do salário no início
- Ignorar a diversificação (alocação por tipo)

## 📱 Abas da Ferramenta

### 📱 APP
A principal! Faça tudo aqui:
- Configure seu perfil
- Simule investimentos
- Veja alocação sugerida
- Receba dicas personalizadas

### 📊 Perfis
Dados técnicos de alocação (você não precisa mexer aqui)
- Tabela com % de cada tipo de FII por perfil
- Usada para calcular sua alocação automaticamente

### 📈 Evolução
Projeção detalhada ano a ano:
- Patrimônio em cada ano
- Renda mensal projetada
- Total investido acumulado

## ⚡ Ações Rápidas

**Quero simular diferentes períodos:**
→ Mude o valor em "Por quantos anos?" na aba APP

**Quero simular diferentes aportes:**
→ Mude o valor em "Quanto investir por mês?"

**Quero ver perfil mais conservador:**
→ Mude para "Conservador" e veja a alocação mudar

**Quero saber quanto vou ter em 20 anos:**
→ Digite 20 em "Por quantos anos?" e veja o resultado


## 🔐 Células Importantes

### NUNCA APAGUE
- C15 (Taxa de rendimento - é referência!)
- C17 (Patrimônio - fórmula FV)
- Tabela de Perfis (aba Perfis)

### PODE EDITAR À VONTADE
- C6 (Salário)
- C7 (Rendimento)
- C8 (Perfil)
- C13 (Aporte mensal)
- C14 (Período em anos)


## 📈 Fórmulas Principais

**Patrimônio Acumulado:**
```excel
=FV(taxa_mensal, anos*12, -aporte_mensal, 0)
```

**Renda Mensal:**
```excel
=Patrimônio * Taxa_Mensal
```

**Alocação por Tipo:**
```excel
=VLOOKUP(Perfil&"-tipo", Tabela_Perfis, 4, FALSE)
```


## 🎓 Aprenda Mais

### Sobre FIIs
- [Portal do Investidor - CVM](https://www.investidor.gov.br)
- [B3 - Fundos Imobiliários](https://www.b3.com.br/pt_br/produtos-e-servios/negociacao/renda-variavel/fundos-de-investimentos/fii/)

### Sobre a Ferramenta
- Baseada em fórmulas financeiras tradicionais (FV)
- Alocações baseadas em práticas de mercado
- Rendimentos baseados em médias históricas

## ⚠️ Avisos Importantes

- Esta é uma ferramenta educacional
- Não é recomendação de investimento
- Resultados são estimativas
- Passado não garante futuro
- Consulte um assessor financeiro
