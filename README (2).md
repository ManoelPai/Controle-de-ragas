# Controle de Ordem de Serviço

Sistema de gerenciamento de Ordens de Serviço para controle de pragas, otimizado para uso mobile por técnicos em campo.

---

## Funcionalidades Principais

- **Autenticação Simples:** Login por CPF/Registro e senha/PIN.
- **Lista Dinâmica de OS:** Visualize, inicie, continue e finalize ordens do dia.
- **Cadastro Ágil de Clientes:** Pessoa Física ou Jurídica, com formulário adaptativo.
- **Detalhamento Completo da OS:** Dados do cliente, status, histórico e navegação entre etapas.
- **Ficha Técnica Interativa:** Selecione pragas, ambientes, produtos, EPIs, equipamentos, faça observações e registre recomendações.
- **Assinaturas Digitais:** Captação de assinaturas do técnico e cliente diretamente na tela.
- **Finalização Profissional:** Geração de laudo em PDF, impressão Bluetooth e envio facilitado por e-mail.

---

## Estrutura dos Componentes

- **LoginScreen:** Tela de login com alternância de visualização da senha e feedback de erro.
- **OSListScreen:** Exibe as OS do dia, com status colorido, busca de cliente relacionada e botão para iniciar/continuar OS.
- **NewClientScreen:** Formulário dinâmico (Pessoa Física/Jurídica), com validação e campos inteligentes de endereço.
- **OSDetailScreen:** Mostra detalhes completos da OS e do cliente, com ações para iniciar, preencher ficha técnica ou finalizar.
- **TechnicalSheetScreen:** Registro detalhado da execução, com controles de múltipla seleção e adição dinâmica de produtos.
- **SignatureScreen:** Captura de assinatura via canvas para técnico e cliente, com opção de limpar e confirmar.
- **FinalizationScreen:** Gera laudo visual, permite exportar PDF, imprimir (simulado) ou encaminhar por e-mail.

---

## Tecnologias & Observações

- **React + Hooks:** Componentização moderna e gestão de estado local.
- **Tailwind CSS:** Estilização responsiva, visual limpo e intuitivo.
- **Mock Data:** Utilizado para clientes e OS apenas para demonstração.
- **PDF e Canvas:** html2canvas e jsPDF são carregados via CDN, facilitando exportação de laudos.

---

## Como Usar

1. **Login:** Entre com CPF/Registro e senha (exemplo: `123`/`123`).
2. **Visualize as OS:** Veja as ordens do dia, inicie ou continue conforme necessário.
3. **Cadastre Clientes:** Novo atendimento? Cadastre o cliente rapidamente.
4. **Preencha a Ficha Técnica:** Selecione todas as informações da execução.
5. **Assinaturas:** Capture as assinaturas digitalmente.
6. **Finalize:** Gere o laudo em PDF, imprima ou envie por e-mail.

---

## Personalização

- **Integração Backend:** Basta substituir os mocks por chamadas de API reais.
- **Autenticação:** Implemente OAuth ou integração com sistemas existentes para maior segurança.
- **Impressão Bluetooth:** Integrar com plugins nativos em apps híbridos para impressão real.
- **Envio de PDF:** Conecte com serviços de e-mail ou armazenamento em nuvem.

---

## Exemplo de Uso

```jsx
<LoginScreen onLogin={...} />
<OSListScreen osList={mockOS} ... />
<NewClientScreen onSave={...} />
<OSDetailScreen os={...} client={...} ... />
<TechnicalSheetScreen os={...} onSaveTechnicalSheet={...} />
<SignatureScreen os={...} onSaveSignatures={...} />
<FinalizationScreen os={...} client={...} />
```

---

## Observações Finais

- Este projeto é um exemplo e pode ser expandido para uso real em campo.
- Facilidade de adaptação para outros tipos de serviços e equipes externas.
- Priorize sempre usabilidade para técnicos — poucos cliques para cada ação.

---

## Licença

MIT
