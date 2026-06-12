## 😴 Por que o Pillow foi criado?

A insônia e a má qualidade do sono são problemas cada vez mais comuns. Muitas pessoas dormem poucas horas, acordam cansadas, têm dificuldade para manter uma rotina regular ou não conseguem identificar quais hábitos estão prejudicando seu descanso.

Dados de instituições ligadas à saúde do sono, como Sleep Foundation, National Sleep Foundation e NIH, mostram que uma parcela significativa da população adulta sofre com sintomas de insônia, dificuldade para dormir, sono insuficiente ou baixa qualidade de descanso.

Pensando nisso, o **Pillow** foi criado como uma ferramenta para ajudar o usuário a entender melhor sua rotina de sono. O app permite registrar noites dormidas, horários, interrupções, humor ao acordar e observações pessoais, transformando esses dados em análises visuais e recomendações práticas.

O objetivo do Pillow não é substituir acompanhamento médico, diagnóstico profissional ou exames clínicos do sono, mas sim auxiliar o usuário a perceber padrões e melhorar seus hábitos com base nos próprios registros.

Com o Pillow, o usuário pode identificar situações como:

* Dormir menos do que o recomendado para sua idade;
* Ter muitas interrupções durante a noite;
* Manter horários irregulares de sono;
* Acordar frequentemente cansado ou indisposto;
* Ter queda de qualidade em noites com celular, ruído, ansiedade, luz ou outros fatores;
* Evoluir ou piorar ao longo dos dias.

Dessa forma, o app funciona como um apoio para melhorar a higiene do sono, incentivar uma rotina mais saudável e tornar os dados do sono mais fáceis de entender.

# 🌙 Pillow — Monitoramento e Análise do Sono

**Pillow** é um aplicativo desktop de monitoramento e análise do sono, desenvolvido com **React**, **TypeScript**, **Vite**, **Tailwind CSS** e **Electron**.
O objetivo do projeto é ajudar o usuário a registrar suas noites de sono, acompanhar sua evolução, entender padrões e receber recomendações personalizadas para melhorar a qualidade do descanso.

O app foi pensado para ter uma experiência visual moderna, calma e premium, inspirada em aplicativos de saúde e bem-estar como **Sleep Cycle**, **Fitbit**, **Samsung Health**, **Apple Health**, **Headspace** e **Calm**.

---

## 📌 Objetivo do Projeto

O Pillow tem como objetivo principal responder perguntas como:

* Como foi minha última noite de sono?
* Meu sono está melhorando ou piorando?
* Estou dormindo dentro da faixa recomendada para minha idade?
* Quais fatores estão prejudicando minha qualidade de sono?
* Que ações posso tomar para melhorar meu descanso?

Além disso, o projeto busca demonstrar o uso de tecnologias modernas para desenvolvimento de aplicações desktop com interface rica, armazenamento local e análise de dados.

---

## 🖥️ Tecnologias Utilizadas

* **React**
* **TypeScript**
* **Vite**
* **Tailwind CSS**
* **Electron**
* **Lucide React**
* **LocalStorage / Banco local**
* **HTML5**
* **CSS3**
* **JavaScript/TypeScript**

---

## 🎨 Identidade Visual

O Pillow foi desenvolvido com uma identidade visual voltada para:

* Sono
* Calma
* Conforto
* Tecnologia
* Bem-estar
* Visual premium

Características visuais:

* Dark mode elegante
* Cores principais em azul e roxo
* Glassmorphism leve
* Sombras suaves
* Fundo com estrelas
* Animações discretas
* Interface limpa e moderna
* Cards com boa hierarquia visual

### Cores semânticas

As cores semânticas são usadas apenas como apoio visual:

* 🟢 Verde: bom, ideal, meta atingida
* 🟡 Amarelo/Laranja: atenção, regular, pode melhorar
* 🔴 Vermelho: ruim, crítico, interrupções
* 🔵 Azul/Roxo: informações neutras, identidade visual e análise

O app evita usar cores fortes em fundos inteiros de cards, priorizando um visual mais suave e relaxante.

---

## 🔐 Login e Cadastro

O sistema possui tela de login e cadastro de usuários.

### Cadastro

O usuário pode cadastrar:

* Nome
* Data de nascimento
* Email
* Senha
* Confirmação de senha
* Foto de perfil opcional

A data de nascimento é usada para calcular automaticamente a idade do usuário e definir a faixa de sono recomendada.

### Login

O usuário pode acessar sua conta usando email e senha.

Também existe uma conta demo/sistema:

```txt
Usuário: admin
Senha: admin123
```

O login admin é permitido mesmo sem formato de email, enquanto usuários comuns precisam usar um email válido.

---

## 👤 Perfil do Usuário

O app utiliza o nome do usuário para personalizar a experiência.

Exemplo:

```txt
Boa noite, Pedro 👋
```

Caso o usuário altere o nome em **Configurações > Conta**, o novo nome é atualizado em todo o aplicativo, incluindo a sidebar.

Também é possível utilizar uma foto de perfil. Caso nenhuma imagem seja cadastrada, o app exibe um avatar padrão com a inicial do nome.

---

## 🏠 Tela Início — Visão Geral do Sono

A aba **Início** responde à pergunta:

> Como foi minha última noite?

Ela apresenta um resumo da noite mais recente registrada pelo usuário.

Principais informações exibidas:

* Diagnóstico da última noite
* Tempo total de sono
* Qualidade do sono
* Horário de dormir
* Horário de acordar
* Humor ao acordar
* Interrupções registradas
* Recomendação prática

### Análise Inteligente

A seção de Análise Inteligente interpreta os dados reais do último registro e apresenta informações em blocos:

* Resumo da noite
* Ponto positivo
* Fator de atenção
* Impacto provável
* Próxima ação recomendada

Exemplo:

```txt
Você dormiu 8h42min, dentro da faixa recomendada para sua idade.
Ruído ambiente foi registrado e pode ter afetado a continuidade do sono.
```

---

## 📊 Histórico de Sono

A aba **Histórico de Sono** responde à pergunta:

> Como meu sono vem evoluindo ao longo do tempo?

Ela mostra a evolução do sono com base nos registros salvos.

Funcionalidades principais:

* Média do período
* Qualidade média
* Melhor noite
* Pior noite
* Meta atingida
* Comparação detalhada do período
* Leitura inteligente do período
* Gráfico de registros
* Evolução dos últimos 30 dias

### Filtros de período

O usuário pode analisar os dados por:

```txt
7 dias | 30 dias | Este mês | Todos
```

Ao trocar o período, os cards, gráficos e leituras são atualizados conforme os dados reais daquele intervalo.

### Gráfico de Registros

O gráfico de registros mostra:

* Horas de sono
* Qualidade do sono

As barras são exibidas lado a lado, nunca uma dentro da outra.

### Evolução dos Últimos 30 Dias

Esse gráfico mostra a variação diária do sono nos últimos 30 dias, permitindo visualizar se o sono está:

* Melhorando
* Piorando
* Oscilando
* Estável

---

## 🧠 Análise de Sono

A aba **Análise de Sono** oferece uma interpretação mais profunda dos dados registrados.

Ela utiliza informações como:

* Duração do sono
* Qualidade
* Interrupções
* Humor
* Regularidade
* Observações
* Horários de dormir e acordar

A análise busca identificar padrões, possíveis causas de queda na qualidade do sono e fatores externos que podem influenciar o descanso.

---

## 🎯 Plano de Sono

A aba **Plano de Sono** gera recomendações e metas personalizadas com base nos dados reais do usuário.

Ela pode apresentar:

* Progresso geral
* Foco principal automático
* Próxima ação do dia
* Metas personalizadas
* Hábitos recomendados
* Evolução semanal

Exemplo:

```txt
Celular apareceu em vários registros recentes e suas noites com celular tiveram qualidade média menor.
Tente ativar o modo Não Perturbe antes de dormir.
```

O objetivo é que o plano não seja genérico, mas adaptado ao comportamento do usuário.

---

## 🔔 Notificações

O Pillow possui sistema de notificações internas na sidebar.

As notificações podem incluir:

* Lembrete para dormir
* Aviso de horário ideal
* Lembrete de monitoramento
* Meta atingida
* Lembrete de registro

As notificações consideram:

* Horário atual
* Horário configurado pelo usuário
* Última notificação enviada
* App aberto depois do horário
* Reinício ou recarregamento do app

Exemplos:

```txt
Faltam 30 minutos para seu horário de dormir.
Está na hora de dormir.
Você já passou do seu horário ideal de dormir.
Está na hora de iniciar o monitoramento do sono.
```

---

## ⚙️ Configurações

A aba **Configurações** permite controlar informações da conta e preferências do app.

Principais seções:

* Conta
* Informações pessoais
* Foto de perfil
* Horários de sono
* Notificações
* Aparência
* Privacidade e segurança
* Gerenciamento de dados

### Gerenciamento de dados

O usuário pode apagar registros de sono de forma controlada:

* Selecionar um único registro
* Selecionar vários registros
* Selecionar todos
* Confirmar antes de excluir

A exclusão afeta apenas os registros do usuário logado, sem apagar conta, email, senha, configurações ou foto de perfil.

---

## 📥 Importação de Dados

O Pillow possui suporte planejado/implementado para importação de dados em:

* CSV
* JSON
* Apple Health XML

Caso um arquivo importado tenha um registro para uma data que já existe, o registro antigo é substituído pelo novo.

---

## 💤 Faixas Recomendadas de Sono

O app usa a data de nascimento do usuário para calcular a faixa recomendada de sono.

Faixas utilizadas:

```txt
Criança: 9 a 12 horas
Adolescente: 8 a 10 horas
Adulto: 7 a 9 horas
Idoso: 7 a 8 horas
```

Caso não exista data de nascimento cadastrada, o app utiliza o padrão adulto:

```txt
7 a 9 horas por noite
```

---

## 🌙 Estimativa de Sono REM

O Pillow não utiliza sensores clínicos para medir fases reais do sono.

Por isso, qualquer informação relacionada a REM é apresentada como:

```txt
Estimativa de sono REM
```

O app evita apresentar REM como valor exato.

---

## 🧮 Qualidade do Sono

A qualidade do sono é calculada com base em fatores como:

* Duração da noite
* Interrupções
* Humor ao acordar
* Regularidade
* Horário de dormir
* Observações negativas
* Distância da faixa recomendada de sono

Fatores negativos, como muitas interrupções ou baixa duração, impactam a pontuação final.

---

## 📁 Estrutura Geral do Projeto

A estrutura pode variar conforme a organização final, mas o projeto segue uma base semelhante a:

```txt
Pillow/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   ├── utils/
│   ├── data/
│   ├── App.tsx
│   └── main.tsx
├── electron/
│   └── main.js
├── package.json
├── vite.config.ts
├── tailwind.config.js
└── README.md
```

---

## 🚀 Como Executar o Projeto

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

### 2. Acessar a pasta do projeto

```bash
cd seu-repositorio
```

### 3. Instalar dependências

```bash
npm install
```

### 4. Rodar em modo desenvolvimento

```bash
npm run dev
```

---

## 🖥️ Executar com Electron

Dependendo dos scripts configurados no `package.json`, use:

```bash
npm run electron
```

ou:

```bash
npm run electron:dev
```

---

## 🏗️ Gerar Build

### Build web

```bash
npm run build
```

### Build desktop com Electron

Dependendo da configuração do projeto:

```bash
npm run dist
```

ou:

```bash
npm run electron:build
```

O instalador ou executável final será gerado na
