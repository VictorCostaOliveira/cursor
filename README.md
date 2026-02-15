# Rails + Vue.js Development Agents

Uma suite de agentes especializados para desenvolvimento Rails + Vue.js seguindo TDD e boas práticas.

## 🎯 Agentes Disponíveis

### 1. rafael (Analista de Requisitos) ⭐
**Analista de Requisitos Sênior**

Analista de requisitos especializado em levantar requisitos funcionais e não funcionais através de perguntas estratégicas.

- **Stack-Agnostic**: Funciona para qualquer projeto, não apenas Rails/Vue
- **Perguntas Estratégicas**: Descobre requisitos através de questionamento estruturado
- **Requisitos Completos**: Funcionais, não funcionais, edge cases, dependências
- **Contexto de Negócio**: Entende usuários, processos, restrições, valor esperado
- **Documentação**: Gera documento completo com critérios de aceite Given-When-Then
- **Uso**: Use ANTES de planejar ou implementar features quando demanda estiver vaga ⚠️

### 2. rails-vue-feature-planner
**Planejador de Features (TDD-First)**

Transforma user stories e cards Jira em planos de implementação executáveis, **sempre começando pelos testes**.

- **Ruby on Rails**: REST APIs, Active Record, RSpec, Service Objects
- **Vue.js 3**: Composition API, Pinia, componentização, reatividade
- **TDD**: Red-Green-Refactor, Better Specs para backend e frontend
- **Arquitetura**: SOLID, Design Patterns, Clean Architecture
- **Qualidade**: Testes primeiro, segurança, performance, escalabilidade

### 3. junior (Desenvolvedor Júnior)
**Desenvolvedor de Implementação**

Pega o plano e testes definidos e implementa o código até todos os testes passarem.

- **Análise de Padrões**: Em projetos existentes, replica EXATAMENTE os padrões do código existente ⚠️
- **Foco**: Implementação pura, não planejamento
- **Regra Crítica**: NUNCA altera testes, apenas implementa código que os satisfaz
- **Workflow**: RED (testes falham) → GREEN (implementa) → REFACTOR
- **Boas Práticas**: Segue todos os conhecimentos da base (SOLID, DRY, segurança)
- **Consistência**: Código novo deve parecer escrito pela mesma pessoa do código antigo

### 4. verifier (Validador Independente) ⭐
**Validador Cético**

Confirma se trabalho declarado como completo realmente funciona através de validação independente.

- **Foco**: Validação independente de implementações
- **Processo**: Executa testes, verifica edge cases, valida fluxos de ponta a ponta
- **Uso**: Proativo APÓS Junior marcar implementação concluída
- **Importante**: Cético, não aceita declarações pelo valor aparente
- **Benefício**: Identifica implementações incompletas antes de considerar feature pronta

### 5. astolfo (Revisor Sênior)
**Revisor de Código Rails**

Analisa código Rails em busca de problemas de segurança, SOLID, escalabilidade e qualidade.

- **Verificação de Padrões**: Valida se código novo segue padrões existentes do projeto ⚠️
- **Expertise**: Ruby on Rails de larga escala
- **Foco**: Segurança, SOLID, performance, code smells, consistência
- **Uso**: Proativo após modificações em código Rails
- **Importante**: NÃO implementa mudanças sem confirmação explícita

## 🚀 Como Usar

### Workflow Completo: Feature do Zero à Implementação

#### Workflow Recomendado ⭐

1. **Análise de Requisitos** → Use `rafael` para levantar requisitos completos
2. **Planejamento TDD** → Use `ana` para criar plano e testes
3. **Implementação** → Use `junior` para desenvolver código
4. **Validação** → Use `verifier` para confirmar que realmente funciona ⭐ NOVO!
5. **Revisão** → Use `astolfo` para revisar qualidade

#### Por que começar com Rafael?

Começar com análise de requisitos garante:
- ✅ Nenhuma ambiguidade ou gap nos requisitos
- ✅ Todos os edge cases identificados
- ✅ Requisitos não funcionais mapeados (segurança, performance)
- ✅ Ana (planejadora) tem especificação completa para trabalhar
- ✅ Menos retrabalho e surpresas durante implementação

### Exemplos de Uso por Agente

#### rafael: Análise de Requisitos ⭐

```
Preciso implementar um sistema de comentários nos posts.
Use o rafael para levantar todos os requisitos funcionais e não funcionais.
```

**Output**: Documentação completa com requisitos funcionais, não funcionais, casos de uso, edge cases, critérios de aceite e dependências.

#### ana: Criar Plano TDD

```
Já tenho os requisitos completos do sistema de comentários levantados pelo rafael.
Use a ana para criar um plano TDD completo com testes.
```

**Output**: Plano com testes RSpec + Vitest especificados primeiro, depois design de implementação.

#### junior: Implementar Feature

```
Tenho o plano de comentários pronto e os testes escritos pela ana.
Use o junior para implementar o código até todos os testes passarem.
```

**Output**: Implementação completa (backend + frontend) com todos os testes passando.

#### verifier: Validar Implementação ⭐

```
Use o verifier para confirmar que o sistema de comentários realmente funciona.
```

**Output**: Validação independente confirmando o que funciona vs o que está incompleto.

#### astolfo: Revisar Código

```
Use o astolfo para analisar o código de comentários implementado e validado.
```

**Output**: Análise de segurança, SOLID, performance, consistência e sugestões de melhoria.

### Exemplos Combinados

#### Feature Completa (Análise + Planejamento + Implementação + Validação + Revisão)
```
User Story: Sistema de likes nos posts

1. rafael: Levanta requisitos funcionais e não funcionais
2. ana: Cria plano TDD com testes especificados
3. junior: Implementa código até todos os testes passarem
4. verifier: Valida que realmente funciona de ponta a ponta ⭐ NOVO!
5. astolfo: Revisa código para garantir qualidade
```

#### API + Frontend do Zero
```
Preciso criar endpoints REST para gerenciar produtos e a interface Vue.

rafael: Levanta todos os requisitos (auth, validações, edge cases, performance)
ana: Desenha a solução completa com testes primeiro
junior: Implementa backend Rails + frontend Vue seguindo padrões do projeto
verifier: Confirma que tudo funciona de ponta a ponta (testes + fluxo real) ⭐
astolfo: Valida segurança, SOLID, performance e consistência
```

## 🤔 Quando Usar Cada Agente

### Use o Rafael (Analista de Requisitos) quando:

✅ Você recebe uma **demanda nova** de feature
✅ Requisitos estão **vagos ou incompletos**
✅ Precisa mapear **edge cases e validações**
✅ Precisa definir **requisitos não funcionais** (segurança, performance)
✅ Quer garantir **nenhuma ambiguidade** antes de implementar

**Exemplo**: "Implementar sistema de notificações" (muito vago!)

### Use a Ana (Planejadora) quando:

✅ Requisitos já estão **claros e completos**
✅ Precisa criar **plano TDD** com testes especificados
✅ Quer **design de implementação** detalhado
✅ Requisitos funcionais e não funcionais já estão mapeados

**Exemplo**: "Já tenho requisitos completos, preciso do plano técnico"

### Use o Junior (Desenvolvedor) quando:

✅ Já tem **plano e testes prontos**
✅ Só precisa de **implementação pura**
✅ Testes já estão escritos e validados
✅ Sabe exatamente o que implementar

**Exemplo**: "Tenho os testes, só implementar"

### Use o Verifier (Validador) quando:

✅ Junior **marcou tasks como concluídas**
✅ Quer **confirmar que realmente funciona**
✅ Precisa **validar de ponta a ponta**
✅ Quer **identificar implementações incompletas**

**Exemplo**: "Verificar se sistema de comentários está realmente completo"

### Use o Astolfo (Revisor) quando:

✅ Código já foi **implementado e validado**
✅ Precisa validar **segurança, SOLID, performance**
✅ Quer verificar **consistência com padrões do projeto**
✅ Precisa de **sugestões de melhoria**

**Exemplo**: "Revisar PR de comentários"

## 📋 O Que Cada Agente Entrega

### rafael (Analista de Requisitos) ⭐

**Output**: Documentação completa de requisitos incluindo:

1. **Contexto do Projeto** - Arquitetura, padrões, integrações, restrições
2. **Requisitos Funcionais** - Fluxos, validações, casos de erro, edge cases
3. **Requisitos Não Funcionais** - Segurança, performance, escalabilidade, observabilidade
4. **Casos de Uso** - Fluxos principais, alternativos e de exceção
5. **Critérios de Aceite** - Given-When-Then para cada cenário
6. **Dependências e Riscos** - Impactos, integrações, pontos de atenção
7. **Estimativa de Complexidade** - Tamanho da feature e justificativa

### rails-vue-feature-planner (Planejador)

**Output**: Plano TDD completo incluindo:

1. **Critérios de Aceite** - Cenários Given-When-Then, edge cases
2. **Especificação de Testes (RED)** - RSpec + Vitest escritos ANTES da implementação
3. **Design de Implementação (GREEN)** - Backend Rails + Frontend Vue
4. **Plano de Execução** - Fases TDD com ordem de implementação
5. **Considerações Técnicas** - Segurança, performance, rollback

### rails-vue-developer (Desenvolvedor)

**Output**: Código implementado incluindo:

1. **Backend Rails** - Migrations, Models, Controllers, Routes
2. **Frontend Vue** - Stores Pinia, Composables, Components
3. **Todos os Testes Passando** - `rspec` ✅ + `npm run test` ✅
4. **Código Limpo** - SOLID, DRY, métodos < 15 linhas
5. **Sem Alterações nos Testes** - Testes originais intactos


### verifier (Validador) ⭐ NOVO!

**Output**: Validação independente incluindo:

1. **Resultados dos Testes** - Backend (RSpec) e Frontend (Vitest) com status
2. **O Que Funciona** - Features realmente implementadas e operacionais
3. **O Que Está Incompleto** - Problemas específicos encontrados com reprodução
4. **Edge Cases Não Tratados** - Cenários que precisam atenção
5. **Resumo de Completude** - Taxa real de conclusão e próximas ações

### astolfo (Revisor)

**Output**: Análise detalhada incluindo:

1. **Problemas de Segurança** - Auth, validations, SQL injection, XSS
2. **Violações SOLID** - SRP, OCP, LSP, ISP, DIP
3. **Problemas de Performance** - N+1 queries, eager loading
4. **Code Smells** - Duplicação, complexidade, acoplamento
5. **Sugestões de Melhoria** - Refactorings específicos

## 🗂️ Estrutura do Projeto

```
.cursor/agents/
├── rafael.md                       # 🎯 Analista de requisitos (levanta RF e RNF) ⭐
├── ana.md                          # 📐 Arquiteta & Planejadora TDD (testes primeiro)
├── junior.md                       # 🛠️  Desenvolvedor júnior (implementação rápida)
├── verifier.md                     # ✅ Validador cético (confirma que funciona) ⭐ NOVO!
├── astolfo.md                      # 🔍 Revisor sênior (segurança, SOLID, performance)
├── knowledge/                      # 📚 Base de conhecimento compartilhada
│   ├── architecture.md             # SOLID e design patterns
│   ├── backend.md                  # Padrões de arquitetura backend
│   ├── frontend.md                 # Vue.js + Pinia best practices
│   ├── rails-code-quality.md       # Qualidade de código Rails
│   ├── rails-scalability.md        # Escalabilidade Rails
│   ├── rails-security.md           # Segurança Rails
│   ├── rails-solid.md              # SOLID aplicado ao Rails
│   ├── rails-vue-examples.md       # Exemplos práticos Rails + Vue
│   └── templates.md                # Templates de planejamento
└── README.md                       # 📖 Esta documentação
```

## 📚 Base de Conhecimento

O agente consulta automaticamente a base de conhecimento durante o planejamento:

### Rails Backend
- `knowledge/rails-solid.md` - SOLID principles aplicados ao Rails
- `knowledge/rails-security.md` - Segurança Rails (auth, validations)
- `knowledge/rails-scalability.md` - N+1 queries, eager loading, caching
- `knowledge/rails-code-quality.md` - Best practices Rails

### Vue.js Frontend
- `knowledge/frontend.md` - Vue.js 3, Pinia, componentização, reatividade
- Composition API, composables, scoped styles
- Testes com Vitest seguindo Better Specs

### Arquitetura e Padrões
- `knowledge/architecture.md` - SOLID, Design Patterns, DDD
- `knowledge/backend.md` - API design, camadas, serviços
- `knowledge/templates.md` - Templates de planejamento

### Better Specs
- Referência: https://www.betterspecs.org/
- Use `expect` syntax (nunca `should`)
- Organize com `describe` e `context`
- Uma expectativa por teste (quando possível)
- Use `let` e `let!` para setup
- Factories (FactoryBot), não fixtures

## 🎓 Princípios Seguidos

Todos os agentes seguem:

1. **Requisitos Primeiro** ⭐: Rafael levanta requisitos completos ANTES de qualquer planejamento ou código
2. **Padrões Existentes Primeiro** ⚠️: Em projetos existentes, SEMPRE analisar e seguir os padrões já implementados
3. **Test-First**: Ana define testes ANTES da implementação (TDD)
4. **Red-Green-Refactor**: RED (testes falham) → GREEN (implementa) → REFACTOR (limpa)
5. **Validação Independente** ⭐ NOVO!: Verifier confirma que "completo" realmente funciona
6. **Better Specs**: https://www.betterspecs.org/ em RSpec E Vitest
7. **SOLID Principles**: Código limpo, coeso, manutenível
8. **Security by Default**: Auth, validations, proteções desde o início
9. **Performance Optimization**: N+1 prevention, eager loading, indexação
10. **Never Touch Tests**: Junior NUNCA altera testes, apenas implementa código
11. **Consistency > Perfection**: Manter consistência com código existente é mais importante que "fazer do jeito perfeito"

## ⚙️ Workflow TDD Completo

### Fase 1: Planejamento (rails-vue-feature-planner)

```
INPUT: User story / Card Jira
↓
1. Análise de requisitos
2. Critérios de aceite (Given-When-Then)
3. Especificação de testes (RED PHASE)
   - RSpec (backend)
   - Vitest (frontend)
4. Design de implementação (GREEN PHASE)
5. Plano de execução em fases
↓
OUTPUT: Plano TDD completo + Testes escritos
```

### Fase 2: Implementação (rails-vue-developer)

```
INPUT: Plano + Testes escritos
↓
1. Executar testes → Todos falham (RED) ✅
2. Backend Rails
   - Migration → Model → Controller → Routes
   - Rodar testes após cada camada
3. Frontend Vue
   - Store → Composables → Components
   - Rodar testes após cada camada
4. Executar TODOS os testes → Todos passam (GREEN) ✅
5. Refactor (se necessário)
↓
OUTPUT: Feature completa funcionando
```

### Fase 3: Validação (verifier) ⭐ NOVO!

```
INPUT: Código implementado
↓
1. Executar testes (rspec + npm test)
2. Verificar implementação real
3. Testar edge cases
4. Validar fluxo de ponta a ponta
5. Identificar problemas
↓
OUTPUT: Relatório de validação (o que funciona vs incompleto)
```

### Fase 4: Revisão (astolfo)

```
INPUT: Código implementado
↓
1. Análise de segurança
2. Análise SOLID
3. Análise de performance
4. Code smells
5. Sugestões de melhoria
↓
OUTPUT: Relatório de qualidade + Refactorings
```

## 🔄 Ciclo Completo: Exemplo Prático

### User Story: Sistema de Comentários em Posts

**Workflow Completo** (5 fases) ⭐

**1. ANÁLISE DE REQUISITOS** → `rafael`
```
Input: "Preciso implementar sistema de comentários nos posts"

Rafael faz perguntas:
  - Quem pode comentar? Apenas logados?
  - Pode editar/deletar comentários?
  - Há limite de caracteres?
  - Precisa moderar comentários?
  - Notifica autor do post?
  - Como lidar com spam?
  - Soft delete ou hard delete?
  - Etc...

Output:
  ✓ Requisitos funcionais completos
  ✓ Requisitos não funcionais (segurança, performance)
  ✓ Casos de uso mapeados
  ✓ Edge cases identificados
  ✓ Critérios de aceite definidos
  ✓ Dependências e riscos conhecidos
```

**2. PLANEJAMENTO TDD** → `ana`
```
Input: Requisitos completos do rafael

Output:
  ✓ Testes RSpec escritos (Comment model + API)
  ✓ Testes Vitest escritos (CommentStore + Components)
  ✓ Design: Migration, Model, Controller, Routes, Store, Components
  ✓ Plano de execução em fases
```

**3. IMPLEMENTAR** → `junior`
```
Input: Plano da ana + Testes escritos

Workflow:
  0. Analisa padrões do projeto existente
  1. Roda testes → RED (todos falham)
  2. Cria migration CreateComments (seguindo padrões)
  3. Implementa Comment model
  4. Roda model specs → GREEN ✅
  5. Implementa CommentsController
  6. Roda request specs → GREEN ✅
  7. Implementa useCommentsStore
  8. Roda store specs → GREEN ✅
  9. Implementa CommentForm, CommentList
  10. Roda component specs → GREEN ✅
  11. Roda TODOS testes → GREEN ✅

Output: Feature implementada com testes passando
```

**4. VALIDAR** → `verifier` ⭐ NOVO!
```
Input: Código implementado pelo junior

Workflow:
  1. Executa todos os testes (rspec + npm test)
  2. Verifica implementação real (não só testes)
  3. Testa edge cases (validações, erros, concorrência)
  4. Valida fluxo de ponta a ponta
  5. Identifica implementações incompletas

Output:
  ✓ O que realmente funciona
  ✓ O que está incompleto (se houver)
  ✓ Edge cases não tratados
  ✓ Taxa real de completude
```

**5. REVISAR** → `astolfo`
```
Input: Código implementado pelo junior

Output:
  ✓ Segurança OK (auth, validations)
  ✓ SOLID OK (SRP, DRY)
  ✓ Consistência OK (seguiu padrões do projeto)
  ✓ Performance: Sugestão de adicionar eager loading
  ✓ Sugestão: Extrair CommentCreator service (opcional)
```

**RESULTADO FINAL**: Feature completa, testada, **validada**, revisada e documentada! 🎉

## 📖 Exemplo de Saída por Agente

### 📐 rails-vue-feature-planner Output

**🧪 Testes Backend (escritos pelo planner)**
```ruby
# spec/models/comment_spec.rb
RSpec.describe Comment, type: :model do
  it { is_expected.to belong_to(:post) }
  it { is_expected.to belong_to(:author).class_name('User') }
  it { is_expected.to validate_presence_of(:content) }
  it { is_expected.to validate_length_of(:content).is_at_most(500) }
end

# spec/requests/api/v1/comments_spec.rb
RSpec.describe 'Comments API', type: :request do
  describe 'POST /api/v1/posts/:post_id/comments' do
    it 'creates comment' do
      expect { post url, params: valid_params, headers: auth_headers }
        .to change(Comment, :count).by(1)
      expect(response).to have_http_status(:created)
    end
  end
end
```

**🧪 Testes Frontend (escritos pelo planner)**
```javascript
// stores/comments.spec.js
describe('useCommentsStore', () => {
  it('creates comment', async () => {
    const store = useCommentsStore()
    await store.createComment(postId, content)
    expect(store.comments).toHaveLength(1)
  })
})

// components/CommentForm.spec.js
describe('CommentForm', () => {
  it('emits submit with content', async () => {
    const wrapper = mount(CommentForm)
    await wrapper.find('textarea').setValue('Nice post!')
    await wrapper.find('form').trigger('submit')
    expect(wrapper.emitted('submit')[0][0]).toBe('Nice post!')
  })
})
```

**🏗️ Plano de Implementação (guia para developer)**
```
Backend:
  1. Migration: create_table :comments (post_id, author_id, content)
  2. Model: validations, associations, methods
  3. Controller: create, update, destroy actions
  4. Routes: resources :comments, only: [:create, :update, :destroy]

Frontend:
  1. Store: useCommentsStore (state, getters, actions)
  2. Composables: useCommentForm (validations)
  3. Components: CommentForm.vue, CommentList.vue, CommentItem.vue
```

### 🛠️ rails-vue-developer Output

**Implementação Real (código que faz testes passarem)**

```ruby
# app/models/comment.rb (implementado pelo developer)
class Comment < ApplicationRecord
  belongs_to :post
  belongs_to :author, class_name: 'User'
  
  validates :content, presence: true, length: { maximum: 500 }
end

# app/controllers/api/v1/comments_controller.rb
class Api::V1::CommentsController < ApplicationController
  before_action :authenticate_user!
  
  def create
    @comment = current_user.comments.build(comment_params)
    
    if @comment.save
      render json: @comment, status: :created
    else
      render json: { errors: @comment.errors }, status: :unprocessable_entity
    end
  end
  
  private
  
  def comment_params
    params.require(:comment).permit(:post_id, :content)
  end
end
```

```javascript
// stores/comments.js (implementado pelo developer)
import { defineStore } from 'pinia'
import { commentsApi } from '@/api/comments'

export const useCommentsStore = defineStore('comments', {
  state: () => ({
    comments: []
  }),
  
  actions: {
    async createComment(postId, content) {
      const comment = await commentsApi.create(postId, content)
      this.comments.push(comment)
      return comment
    }
  }
})
```

**Resultado Final:**
```bash
$ bundle exec rspec
# 42 examples, 0 failures ✅

$ npm run test
# Test Suites: 8 passed
# Tests: 24 passed ✅
```

### 🔍 rails-senior-reviewer Output

**Análise de Qualidade**
```
✅ SOLID Principles
  - SRP: Controller skinny, lógica no model
  - OCP: Extensível via callbacks

⚠️  Performance
  - Adicionar eager loading: Comment.includes(:author, :post)
  - Adicionar índices: add_index :comments, [:post_id, :created_at]

✅ Security
  - Authentication OK (before_action :authenticate_user!)
  - Authorization OK (current_user.comments.build)
  - Strong params OK

💡 Sugestões
  - Extrair CommentNotificationService para envio de emails
  - Adicionar scope: scope :recent, -> { order(created_at: :desc) }
```

## 🔧 Personalização

Você pode personalizar os agentes editando:

- Arquivos `.md` dos agentes: Comportamento e instruções
- `knowledge/*.md`: Adicionar ou modificar base de conhecimento
- Adicionar novos arquivos de conhecimento conforme necessário

## 💡 Dicas de Uso

1. **SEMPRE comece com Rafael**: Ele vai levantar requisitos completos e fazer as perguntas certas ⭐
2. **SEMPRE mencione se é projeto existente**: Os agentes vão analisar e seguir os padrões estabelecidos ⚠️
3. **Não pule a análise de requisitos**: Requisitos mal levantados = retrabalho garantido
4. **Valide os requisitos com Rafael**: Confirme que ele cobriu tudo antes de passar para Ana
5. **Siga a ordem completa**: Rafael → Ana → Junior → **Verifier** → Astolfo ⭐
6. **Use Verifier após implementação**: Confirme que funciona antes de considerar completo ⭐ NOVO!
7. **Use Better Specs**: Sempre siga os padrões do https://www.betterspecs.org/
8. **Itere quando necessário**: Se requisitos mudarem, volte ao Rafael
9. **Confie na equipe**: Rafael analisa, Ana planeja, Junior implementa, Verifier valida, Astolfo revisa
10. **Consistência é chave**: Em projetos existentes, seguir padrões > inventar novos padrões
11. **Documente decisões**: Rafael vai documentar tudo, use isso como referência

## 🤝 Contribuindo

Para melhorar este agente:

1. Adicione novos patterns nos checklists
2. Expanda os exemplos de anti-patterns
3. Adicione novas seções no template
4. Documente learnings de features reais

## 📝 Licença

Este agente é específico do projeto e pode ser customizado conforme necessário.

---

**Rails + Vue.js + TDD + IA = Feature Planning de Qualidade** 🚀
onforme necessário.

---

**Rails + Vue.js + TDD + IA = Feature Planning de Qualidade** 🚀
