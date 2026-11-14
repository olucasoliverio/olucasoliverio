## Lucas Oliverio

Desenvolvedor fullstack na Next Fit e estudante de Engenharia de Software na SATC, em Criciúma/SC.

📫 olucasoliverio@gmail.com

### Projetos

<table>
<tr>
<td width="50%" valign="top">

<a href="https://auttra.com.br"><img src="assets/auttra.jpg" alt="Página inicial da Auttra" width="100%"></a>

**[Auttra](https://auttra.com.br)** · Sistema para Gestão de Oficinas Mecânicas

Estou construindo com o [Lucas Gaspar](https://github.com/LucasGasparA). Junta ordem de serviço, orçamento, agenda, estoque e financeiro, e a tela inicial já aponta o que precisa de atenção: O.S. parada, conta vencida, orçamento sem resposta, peça acabando.

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

</td>
<td width="50%" valign="top">

<a href="https://github.com/olucasoliverio/Doca"><img src="assets/doca.jpg" alt="Doca rodando no Windows 11" width="100%"></a>

**[Doca](https://github.com/olucasoliverio/Doca)** · Dock e Barra de menu do macOS no Windows 11

Substitui a barra de tarefas por uma Dock com ampliação, barra de menu no topo, Spotlight no Alt+Espaço, Central de Controle com Wi-Fi, Bluetooth e som, e controle de música.

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![WPF](https://img.shields.io/badge/WPF-0078D4?style=flat-square&logo=windows&logoColor=white)
![.NET 10](https://img.shields.io/badge/.NET_10-512BD4?style=flat-square&logo=dotnet&logoColor=white)

</td>
</tr>
</table>

### Na Next Fit

Ferramentas internas que fiz para o time de atendimento. O código é fechado.

<table>
<tr>
<td width="50%" valign="top">

**🔀 Roteia**

Distribui as conversas do Freshchat entre os agentes do suporte, respeitando horário, pausas e carga de cada um.

<details>
<summary>O que ele faz</summary>

- **Distribuição**: recebe cada conversa nova por webhook, coloca numa fila e atribui por rodízio, uma de cada vez, para duas conversas que chegam juntas não caírem no mesmo agente.
- **Regras por agente**: limite diário, indisponibilidade no dia ou permanente, e carga reduzida, em que o agente pula algumas vezes depois de receber.
- **Turnos**: conversas que chegam fora do horário ficam pendentes e são distribuídas quando o turno começa. Tem grupos de pausa e sincronização diária dos agentes.
- **Painéis**: dashboard em tempo real com atribuições, resoluções, falhas e gráfico de distribuição, calendário de horários e histórico de alterações. Os agentes têm um painel próprio para cadastrar as ausências.

</details>

<sub>Node.js · BullMQ · Postgres · Redis · React</sub>

</td>
<td width="50%" valign="top">

**📚 Central de Ajuda com IA**

Escreve e mantém os artigos da central de ajuda a partir de uma base vetorial sincronizada com o Freshdesk.

<details>
<summary>O que ela faz</summary>

- **Gerador**: transforma documentos do produto em artigo, passando por plano, ajuste e texto final no padrão de escrita da empresa.
- **Análise de impacto**: recebe o comunicado de uma mudança no produto e aponta quais artigos precisam ser atualizados, com uma segunda etapa que confere cada um.
- **Revisão**: dá nota de qualidade e reescreve artigos existentes.
- **Busca**: combina semântica, palavra-chave, data de atualização e artigos de referência.

</details>

<sub>NestJS · BullMQ · Prisma · pgvector · React · Gemini</sub>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**📊 Análise de Atendimentos**

Lê as conversas de um cliente no Freshchat e gera um relatório do atendimento com Gemini.

<details>
<summary>O que ela faz</summary>

- **Entrada**: busca as conversas pelo e-mail do cliente e analisa uma conversa só ou várias juntas, em lote e em segundo plano.
- **Leitura completa**: além do texto, o modelo vê as imagens, áudios e vídeos enviados. Conversas longas são compactadas antes.
- **Relatório**: resumo executivo, problema principal, linha do tempo, passagens entre agentes, como o atendimento foi conduzido, evidências e ações recomendadas.
- **Risco**: classifica a chance de o cliente voltar a chamar, ficar insatisfeito ou cancelar.

</details>

<sub>Express · Prisma · React · Gemini</sub>

</td>
<td width="50%" valign="top">

**📸 NextPrint**

Fork do Flameshot que envia as capturas de tela direto para o Google Drive de quem está logado, sem servidor próprio.

<details>
<summary>O que ele faz</summary>

- **Login**: OAuth do Google com PKCE, restrito às contas da empresa. Só o refresh token fica guardado, no Keychain do macOS ou no Gerenciador de Credenciais do Windows.
- **Envio**: a captura vai para uma pasta própria no Drive, com um escopo que só enxerga os arquivos criados pelo app. O link é copiado na hora.
- **Compartilhamento**: tenta "qualquer pessoa com o link" e, se a política da empresa bloquear, cai para "qualquer pessoa da empresa".
- **Distribuição**: o instalador do Windows (.msi) é gerado pelo GitHub Actions, e o do macOS sai assinado em .dmg.

</details>

<sub>C++ · Qt 6 · OAuth · GitHub Actions</sub>

</td>
</tr>
</table>

### Faculdade

**[Pipeline de Engenharia de Dados](https://github.com/olucasoliverio/Engenharia_Dados_Final)**: pipeline de um e-commerce em arquitetura medalhão, do MongoDB até um dashboard no Looker Studio.

<sub>Airflow · Spark · Delta Lake · MinIO</sub>

### Tecnologias

[![Tecnologias](https://skillicons.dev/icons?i=ts,react,nodejs,cs,dotnet,cpp,java,python,postgres,redis,docker)](https://skillicons.dev)
