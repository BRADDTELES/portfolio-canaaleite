# Portfólio 🐄 CanaaLeite: Gestão Inteligente para Pecuária Leiteira

![Logo do App](docs/images/ic_launcher_legacy_square.png)

O **CanaaLeite** é um aplicativo Android nativo, desenvolvido em Kotlin, que revoluciona a gestão de pequenos e médios criadores de gado leiteiro. Ele atua como um assistente completo para o produtor rural, integrando controles de rebanho, produção, finanças e o ciclo reprodutivo em uma única plataforma poderosa e fácil de usar.

## ✨ O Que Torna o CanaaLeite Inovador?

O grande diferencial do CanaaLeite é funcionar como um **consultor veterinário virtual** para o
produtor que não tem acesso constante a um profissional. O app guia o usuário através do complexo
ciclo reprodutivo das vacas, com o objetivo de alcançar a meta ideal de um bezerro por vaca por ano.

- **Diagnóstico de Prenhez sem Veterinário:** O sistema utiliza um método inovador baseado na
  observação do ciclo estral (cio). Ele alerta o produtor para verificar a ausência de cio em 21 e
  42 dias após a cobertura, permitindo uma confirmação de prenhez com alta probabilidade, sem a
  necessidade de exames caros ou da presença de um veterinário.
- **Sistema de Alertas Proativo:** O app gera um mural de alertas inteligentes para todas as tarefas críticas do ciclo reprodutivo, como
  previsão de cio, data de secagem e previsão de parto.
- **Gestão 360° da Fazenda:** Além do controle reprodutivo, o CanaaLeite integra:
    - **Controle Financeiro:** Gerencie despesas e receitas com dashboards visuais.
    - **Gestão de Estoque:** Controle a produção de leite e a fabricação de derivados como queijos e
      iogurtes.
    - **Controle de Vendas:** Registre vendas de leite e outros produtos, com gestão de clientes.
- **Funcionalidade Offline-First:** O aplicativo é 100% funcional sem conexão com a internet. Todos
  os dados são salvos localmente e sincronizados automaticamente com a nuvem (Firebase) assim que a
  conexão é restabelecida, garantindo que nenhuma informação seja perdida.

## 🛠️ Tecnologias e Arquitetura

O CanaaLeite foi construído utilizando as mais modernas práticas e tecnologias do desenvolvimento
Android:

- **Linguagem:** **[Kotlin](https://kotlinlang.org/)** - A linguagem oficial para o desenvolvimento
  Android, garantindo código conciso, seguro e moderno.
- **Arquitetura:**
    - **[Clean Architecture](https://developer.android.com/topic/architecture?hl=pt-br):** Separação
      clara das responsabilidades em camadas (Data, Domain, Presentation), facilitando a manutenção,
      testabilidade e escalabilidade do projeto.
    - **MVVM (Model-View-ViewModel):** Padrão de arquitetura que promove a separação entre a lógica
      de apresentação e a UI.
- **Jetpack Components:**
    - **[Room](https://developer.android.com/training/data-storage/room):** Para persistência de
      dados local, garantindo a funcionalidade offline.
    - **[ViewModel](https://developer.android.com/topic/libraries/architecture/viewmodel):** Para
      gerenciar o estado da UI de forma consciente ao ciclo de vida.
    - **[Flow](https://developer.android.com/kotlin/flow)
      e [Coroutines](https://developer.android.com/kotlin/coroutines?hl=pt-br#kts):** Para
      programação assíncrona e reativa, garantindo uma UI fluida e responsiva.
    - **[Hilt](https://dagger.dev/hilt/):** Para injeção de dependência, simplificando a gestão de
      objetos e a modularização.
    - **[Navigation Component](https://developer.android.com/guide/navigation):** Para gerenciar a
      navegação entre as telas de forma simplificada e visual.
    - **[WorkManager](https://developer.android.com/topic/libraries/architecture/workmanager):**
      Para agendar tarefas em segundo plano, como a verificação diária de alertas para gerar
      notificações.
- **UI (Interface do Usuário):**
    - **[ViewBinding](https://developer.android.com/topic/libraries/view-binding?hl=pt-br#kts):**
      Para acesso seguro e eficiente às views do layout.
    - **Material Design:** Para uma interface moderna, intuitiva e visualmente agradável.
    - **[MPAndroidChart](https://github.com/PhilJay/MPAndroidChart):** Para a criação de dashboards
      e gráficos dinâmicos.
- **Backend e Sincronização:**
    - **[Firebase](https://firebase.google.com/):**
        - **[Firestore](https://firebase.google.com/docs/firestore?hl=pt-br):** Como banco de dados
          NoSQL na nuvem para sincronização e backup dos dados.
        - **[Authentication](https://firebase.google.com/docs/auth/android/start?hl=pt-br):** Para
          gerenciar a autenticação de usuários (Email/Senha e Google Sign-In).
        - **[Cloud Messaging](https://firebase.google.com/docs/cloud-messaging?hl=pt-br):** Para o
          envio de notificações push.

## 🖼️ Telas do Aplicativo

<table>
  <tr>
    <td align="center">
      <img src="docs/images/tela_home.png" alt="Tela Principal" width="250"/>
      <br>
      <sub><b>Tela Principal (Home)</b></sub>
    </td>
    <td align="center">
      <img src="docs/images/tela_dashboard.png" alt="Dashboard Financeiro" width="250"/>
      <br>
      <sub><b>Dashboard Financeiro</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="docs/images/tela_mural_de_alertas.png" alt="Mural de Alertas" width="250"/>
      <br>
      <sub><b>Mural de Alertas Inteligentes</b></sub>
    </td>
    <td align="center">
      <img src="docs/images/gaveta_de_notificacoes_com_alertas.png" alt="Notificações de Alertas" width="250"/>
      <br>
      <sub><b>Notificações de Alertas</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="docs/images/tela_rebanho_animal.png" alt="Lista de Animais" width="250"/>
      <br>
      <sub><b>Lista de Animais do Rebanho</b></sub>
    </td>
    <td align="center">
      <img src="docs/images/tela_detalhes_do_animal.png" alt="Detalhes do Animal" width="250"/>
      <br>
      <sub><b>Detalhes do Animal</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="docs/images/tela_com_calendario-customizado_ao_fundo_gerenciamento_de_paricao.png" alt="Gerenciamento de Parição" width="250"/>
      <br>
      <sub><b>Gerenciamento de Parição</b></sub>
    </td>
    <td align="center">
      <img src="docs/images/tela_coletas_de_leite.png" alt="Controle de Coletas de Leite" width="250"/>
      <br>
      <sub><b>Controle de Coletas de Leite</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="docs/images/tela_produtos.png" alt="Gestão de Produtos e Estoque" width="250"/>
      <br>
      <sub><b>Gestão de Produtos</b></sub>
    </td>
    <td align="center">
      <img src="docs/images/tela_movimentacoes_financeira_despesas_e_receita.png" alt="Movimentações Financeiras" width="250"/>
      <br>
      <sub><b>Movimentações Financeiras</b></sub>
    </td>
  </tr>
</table>

## 🚀 Próximos Passos e Inovações Futuras

O CanaaLeite está em constante evolução. As próximas grandes funcionalidades planejadas incluem:

- **Controle Genético e de Linhagem:**
    - Rastreamento de parentesco (`mãe` e `pai`) para auxiliar na seleção genética do rebanho,
      otimizar cruzamentos e evitar a consanguinidade.
- **Gerenciamento por Lotes:**
    - Funcionalidade para agrupar animais em lotes (ex: "vacas em lactação", "bezerras desmamadas"),
      facilitando a gestão e a aplicação de manejos específicos para cada grupo.
- **Integrações Externas e Geolocalização:**
    - Integração com **APIs de Clima e Tempo** para fornecer previsões que possam impactar o manejo
      diário.
    - Uso de **GPS e Mapas** para registrar a localização de laticínios, cooperativas e as fazendas
      dos clientes, otimizando a logística de coleta e entrega.
- **Modernização da Interface:**
    - Migração gradual da interface de ViewBinding (XML) para **[Jetpack Compose](https://developer.android.com/jetpack/compose)**, o toolkit declarativo
      moderno do Android, para acelerar o desenvolvimento da UI e criar interfaces ainda mais ricas
      e dinâmicas.
- **Estrutura de Dados Colaborativa:**
    - Refatoração do modelo de dados no Firestore para uma estrutura baseada em "Organização". Isso
      permitirá que múltiplos usuários (membros da família, funcionários) acessem e gerenciem os
      dados da mesma fazenda de forma colaborativa e segura.

---

## 👨‍💻 Desenvolvido por

<a href="https://www.linkedin.com/in/danilloteles/" target="_blank">
  <img src="docs/images/profile.jpg" width="100px;" alt="Foto de Danillo Teles" style="border-radius:50%;"/>
</a>
<br>
<b>Danillo Teles Carneiro</b>
<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Danillo%20Teles-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/danilloteles/)

*Projeto desenvolvido com foco em trazer tecnologia de ponta para o agronegócio, capacitando o
pequeno e médio produtor rural.*
