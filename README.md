# Projeto Smart Farm

O projeto será dividido em três entregas, realizadas em três semanas consecutivas, de forma a permitir uma evolução gradual e integrada do trabalho.

| Etapa   | Descrição                            | Data de Entrega |
|---------|--------------------------------|----------------|
| Etapa 01 | Necessidades, objetivos e restrições | 27/03/2025 |
| Etapa 02 | Projeto Lógico | 10/04/2025 |
| Etapa 03 | Projeto Físico | 17/04/2025 |

**Sumário**:
- [Projeto Smart Farm](#projeto-smart-farm)
- [Cenário: Fazenda Inteligente "Nova Piratininga"](#cenário-fazenda-inteligente-nova-piratininga)
  - [Infraestrutura e Tecnologias Utilizadas](#infraestrutura-e-tecnologias-utilizadas)
  - [Desafios do Projeto](#desafios-do-projeto)
  - [Sistema de Monitoramento](#sistema-de-monitoramento)
- [Etapas do Projeto](#etapas-do-projeto)
  - [Etapa 01: Necessidades, Objetivos e Restrições](#etapa-01-necessidades-objetivos-e-restrições)
  - [Etapa 02: Projeto Lógico](#etapa-02-projeto-lógico)
  - [Etapa 03: Projeto Físico](#etapa-03-projeto-físico)
- [Pontos de Avaliação](#pontos-de-avaliação)

---

## Cenário: Fazenda Inteligente "Nova Piratininga"

A fazenda "Nova Piratininga" está implementando um projeto de **rede sem fio de missão crítica** para permitir o controle eficiente de máquinas agrícolas, monitoramento de rebanho e operação de drones. **Qualquer falha na conectividade pode causar riscos graves**, como:

- **Máquinas agrícolas desgovernadas**, podendo colidir, danificar plantações ou colocar operadores em risco.
- **Drones fora de controle**, comprometendo atividades como monitoramento aéreo, pulverização de defensivos e levantamento de dados topográficos.
- **Interrupções no rastreamento do rebanho**, dificultando a segurança e logística dos animais, além de inviabilizar o uso de cercas virtuais.
- **Falhas no sistema de irrigação automatizado**, podendo levar à perda de safras devido a irrigação inadequada.

> **⚠️ ATENÇÃO:** O projeto da rede sem fio já esta elaborado, não ha necessidade de especificar. O trabalho é focado na infraestrutura de rede.


### **Infraestrutura e Tecnologias Utilizadas**

A fazenda já adquiriu equipamentos para prover conectividade por meio de duas tecnologias principais:

1. **Rede TVWS (White Space Broadband)** – Opera nas bandas VHF e UHF, fornecendo cobertura de longo alcance e baixa latência para comunicação entre sensores, máquinas e sistemas de automação.
2. **Rede LTE privada** – Voltada para a conectividade móvel dos funcionários, permitindo comunicação via dispositivos celulares e tablets em campo.

As torres de comunicação já foram instaladas conforme o posicionamento no arquivo [KML](https://earth.google.com/earth/d/1o5tbjMjzbidYEa2fGGH9Z7ZJPmPEXq-7?usp=sharing) fornecido.

### **Desafios do Projeto**

Os alunos devem projetar a rede considerando os seguintes requisitos:

- **Alta disponibilidade e redundância:** A rede deve ser resiliente a falhas, garantindo que a conectividade não seja interrompida. Isso pode incluir redundância em links, balanceamento de carga e mecanismos de failover.
- **Capacidade para tráfego atual:** Cada torre de TVWS deve suportar **400 Mbps de tráfego**.
- **Escalabilidade:** A rede deve ser planejada para permitir um crescimento de até **20x a demanda atual** em 10 anos, sem investimentos desnecessários no presente.
- **Segmentação de Rede:**
  - A fazenda recebeu a faixa de endereçamento **200.129.0.0/16**.
  - Cada torre de TVWS deve suportar **1000 dispositivos**.
  - Cada torre LTE deve suportar **250 dispositivos**.
  - Os roteadores utilizarão uma rede exclusiva para sua comunicação interna.
  - O **sistema de monitoramento** deve operar em uma rede privada com endereços não públicos, isolada da infraestrutura principal.

---

## Etapas do Projeto

### **Etapa 01: Necessidades, Objetivos e Restrições**  
Nesta primeira etapa os alunos deverão:
* Levantar e identificar as necessidades e os objetivos do cliente, considerando tanto os aspectos técnicos quanto os de negócio.
* Elaborar um documento com:
    * **Sumário Executivo:** Resumo dos principais objetivos e requisitos.
    * **Análise do Cliente:** Descrição do perfil, necessidades funcionais e não funcionais.
    * **Objetivos de Negócio e Técnicos:** Destacar metas, restrições e exigências do projeto.
* **Data de entrega: Quinta-feira, 27/03.**

### **Etapa 02: Projeto Lógico**

Na segunda etapa os alunos devem desenvolver o design lógico da rede, com base na análise realizada na primeira parte:
* Criar diagramas lógicos que representem a topologia da rede.
* Definir esquemas de endereçamento IP, protocolos de roteamento e políticas de segurança.
* Descrever os fluxos de tráfego e as interconexões lógicas entre os diversos pontos da rede.
* Comparar a teoria estudada com as demandas identificadas na etapa anterior.
* Considerar aspectos de escalabilidade, redundância, segurança e desempenho.
* **Data de entrega: Quinta-feira 11/04.**

### **Etapa 03: Projeto Físico**

Na terceira e última etapa, o projeto transita para o planejamento físico da rede:
* Elaborar a topologia física da rede, incluindo a disposição de equipamentos, cabeamento e pontos de distribuição.
* Detalhar as especificações dos dispositivos (roteadores, switches, servidores etc.) e suas localizações.
* Desenvolver diagramas físicos que ilustrem a implementação da rede no ambiente real.
* **A especificação dos equipamentos de rede vale 0,5 pontos nesta etapa.**
* **Data de entrega: Quinta-feira 17/04.**


## Pontos de Avaliação

Os projetos serão avaliados com base nos seguintes critérios:

1. **Aderência aos objetivos expostos neste documento**
2. **Clareza na identificação das necessidades do cliente e justificativa das escolhas feitas**
3. **Qualidade e coerência do projeto lógico**
4. **Adequação do endereçamento IP, protocolos e segurança da rede**
4. **Escolha e justificativa do roteamento**
5. **Capacidade de escalabilidade e planejamento para crescimento futuro**
6. **Organização e clareza na apresentação dos diagramas**
7. **Adequação do projeto físico à realidade da fazenda**
8. **Especificação correta dos equipamentos de rede (0,5 pontos)**
