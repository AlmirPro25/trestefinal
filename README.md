# Sistema de Geração de Código com Anti-Simulação

## Visão Geral

Este projeto implementa um sistema avançado de geração de código utilizando a API Gemini, com foco especial em eliminar simulações e garantir código 100% funcional e pronto para produção. O sistema inclui detecção e correção automática de simulações, integração real de APIs, implementação de segurança e configuração automática.

## Principais Funcionalidades

### Sistema Anti-Simulação V2

- **Eliminação total de simulações** - Detecção e correção automática de código simulado
- **Integração real de APIs** - Implementação forçada de APIs reais (Stripe, Cloudinary, etc.)
- **Segurança completa** - Implementação obrigatória de medidas de segurança
- **Configuração automática** - Minimização da configuração manual pelo usuário
- **Qualidade de código** - Garantia de código de alta qualidade e pronto para produção

### Geração de Código Aprimorada

- **Personas especializadas** - Geração de código com expertise específica
- **Auto-avaliação** - Avaliação automática da qualidade do código gerado
- **Melhorias automáticas** - Correção automática de problemas detectados
- **Instruções robustas** - Diretrizes detalhadas para geração de código de alta qualidade

## Componentes Principais

### 1. GeminiServiceEnhanced

Serviço aprimorado para interação com a API Gemini, com recursos anti-simulação integrados.

### 2. SimulationDetector

Sistema de detecção de simulações que identifica placeholders, funções vazias, simulações de segurança e APIs.

### 3. CodeQualityChecker

Verificador de qualidade de código que avalia diversos aspectos como integração de APIs, segurança e tratamento de erros.

### 4. GeminiEnhancer

Sistema que melhora automaticamente o código gerado, substituindo simulações por implementações reais.

### 5. AntiSimulationIntegration

Ponto central de integração que conecta todos os componentes e fornece uma API simples para usar o sistema.

## Como Usar

### Configuração Inicial

**Pré-requisitos:** Node.js

1. Instale as dependências:
   ```
   npm install
   ```

2. Configure suas chaves de API no arquivo `.env` (use `.env.example` como referência)
   - Defina `GEMINI_API_KEY` com sua chave da API Gemini

3. Execute o script de configuração:
   ```
   node setup.js
   ```

4. Inicie o servidor de desenvolvimento:
   ```
   npm run dev
   ```

### Uso Básico

```javascript
// Importar o sistema anti-simulação
const AntiSimulationIntegration = require('./src/integration/AntiSimulationIntegration').default;

// Configurar para um tipo específico de projeto
AntiSimulationIntegration.updateOptions({
  projectType: 'ecommerce',
  strictnessLevel: 9,
  autoRegenerate: true
});

// Gerar conteúdo aprimorado
const prompt = 'Crie uma função para processar pagamentos com Stripe';
const resultado = await AntiSimulationIntegration.generateEnhancedContent(prompt);

console.log('Conteúdo gerado:', resultado.content);
```

## Documentação

Documentação detalhada está disponível nos seguintes arquivos:

- `docs/ANTI_SIMULATION_SYSTEM_V2.md` - Documentação completa do Sistema Anti-Simulação V2
- `GEMINI_ENHANCED_INSTRUCTIONS.md` - Instruções aprimoradas para o Gemini
- `examples/antiSimulationExample.js` - Exemplos práticos de uso do sistema
