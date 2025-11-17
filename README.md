# Casas Flutuantes de Cubatão - Website Institucional

## Visão Geral

Website institucional altamente moderno para o projeto das Casas Flutuantes de Cubatão, desenvolvido com tecnologias de ponta e inspirado em designs premiados do Awwwards.com.

## Tecnologias Utilizadas

- **Framework**: Next.js 13.5.1 (App Router)
- **Estilização**: Tailwind CSS
- **Animações**: GSAP (GreenSock Animation Platform) com ScrollTrigger
- **Tipografia**: Plus Jakarta Sans
- **UI Components**: shadcn/ui
- **Icons**: Lucide React

## Estrutura do Website

### Seções Principais

1. **HOME** (`#home`)
   - Hero section de tela cheia
   - Título impactante com gradiente
   - Imagem de fundo das casas flutuantes
   - Call-to-action com animações GSAP

2. **A IDEIA DO PROJETO** (`#ideia`)
   - Apresentação da origem e conceito
   - Cards de features com ícones
   - Layout assimétrico com imagem lateral
   - Animações de entrada ao rolar

3. **O APOIO DA PREFEITURA** (`#apoio`)
   - Citações das autoridades
   - Estatísticas do projeto
   - Design dark mode com gradientes
   - Cards de dados numéricos

4. **A MÍDIA MOSTRANDO O PROJETO** (`#midia`)
   - Grid de imagens com efeitos hover
   - Informações sobre a inauguração
   - Lista de parceiros homenageados
   - Animações de reveal

5. **PARCERIAS GLOBAIS** (`#global`)
   - Visita da comitiva chinesa
   - Conexão com COP 30
   - Grid dos 10 ODS atendidos
   - Animações de scale e bounce

## Características de Design

### Inspiração Awwwards

- **Animações Fluidas**: Todas as seções utilizam GSAP ScrollTrigger para animações suaves ao rolar a página
- **Tipografia Moderna**: Plus Jakarta Sans com múltiplos pesos para hierarquia visual clara
- **Espaçamento Generoso**: Muito whitespace para respirar o conteúdo
- **Gradientes Sofisticados**: Uso estratégico de gradientes azul-ciano
- **Efeitos de Hover**: Transformações e sombras em cards e imagens
- **Layout Assimétrico**: Quebra da grade tradicional para criar interesse visual

### Responsividade

O design é totalmente responsivo com breakpoints Tailwind:
- **Mobile**: Design empilhado vertical
- **Tablet** (md): Grid de 2 colunas
- **Desktop** (lg): Layout completo com múltiplas colunas

### Paleta de Cores

- **Primária**: Azul (#2563eb) a Ciano (#06b6d4)
- **Neutros**: Cinza 50-900 para textos e backgrounds
- **Acentos**: Gradientes vibrantes em CTAs

## Componentes Principais

### Navigation
- Navegação fixa com efeito glassmorphism
- Mudança de estilo ao rolar
- Menu mobile responsivo
- Links de ancoragem suaves

### Footer
- Grid de 4 colunas com informações
- Ícones e badges dos ODS
- Links institucionais

### Sections
Cada seção é um componente isolado com:
- Animações GSAP específicas
- useEffect para inicialização
- Refs para controle de elementos
- Cleanup de ScrollTriggers

## Animações GSAP

### Tipos de Animações Implementadas

1. **Fade In + Translate Y**: Entrada de títulos e textos
2. **Stagger**: Cards e listas aparecem em sequência
3. **Scale + Bounce**: Badges dos ODS com efeito elástico
4. **Slide In**: Imagens laterais deslizam para dentro

### Performance

- Animações otimizadas com `will-change`
- Cleanup apropriado de ScrollTriggers
- Durations e easings balanceados

## Imagens Utilizadas

As imagens do projeto estão em `/public/`:

1. `CasaFlutuanteIntro.jpg` - Hero e galeria
1. `CasaFlutuanteDestaque.jpg` - Exibição detalhada
2. `CasaFlutuanteIdeia.webp` - Seção A Ideia
3. `CasaFlutuanteInicio.jpg` - Galeria mídia
4. `ComitivaChinesa.jpeg` - Seção Global
5. `VideoJornal.jpg` - Galeria mídia

## Comandos de Desenvolvimento

```bash
# Instalar dependências
npm install

# Modo desenvolvimento
npm run dev

# Build de produção
npm run build

# Verificação de tipos
npm run typecheck
```

## Estrutura de Arquivos

```
app/
├── layout.tsx          # Layout raiz com fonte
├── page.tsx            # Página principal
└── globals.css         # Estilos globais

components/
├── Navigation.tsx      # Menu superior
├── Footer.tsx          # Rodapé
└── sections/
    ├── HeroSection.tsx
    ├── IdeiaSection.tsx
    ├── ApoioSection.tsx
    ├── MidiaSection.tsx
    └── GlobalSection.tsx
```

## Acessibilidade

- Links semânticos com aria-labels
- Estrutura HTML5 apropriada
- Contraste de cores adequado (WCAG AA)
- Navegação por teclado funcional
- Imagens com alt text descritivo

## SEO

- Metadata otimizada no layout
- Títulos hierárquicos (h1-h3)
- URLs semânticas com âncoras
- Descrição meta relevante
- Lang pt-BR definido

## Próximos Passos Recomendados

1. Adicionar vídeo institucional no hero
2. Implementar carrossel automático na seção mídia
3. Adicionar formulário de contato
4. Integrar analytics
5. Criar versão em inglês
6. Adicionar mais fotos do projeto

## Créditos

**Projeto**: Prefeitura Municipal de Cubatão
**Secretaria de Habitação**: Andrea Castro
**Arquiteta**: Karla Roncete
**Prefeito**: César Nascimento

---

Desenvolvido com Next.js, Tailwind CSS e GSAP
