<div align="center">

  <img src="img/davidb_arber_landing_page.png" width="400"/>
  
  ![David Barber Banner](https://img.shields.io/badge/David%20Barber-Barbearia%20Premium-8B4513?style=for-the-badge)
  
  [![Deploy Status](https://img.shields.io/badge/deploy-success-brightgreen?style=flat-square)](https://davidbarber.netlify.app)
  [![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)

  **Sistema completo de agendamento online para barbearias modernas**

  [Demo ao Vivo](https://davidbarber.netlify.app) · [Reportar Bug](https://github.com/WebCash-inc/DavidBarber/issues)

</div>

---

## ✨ Sobre o Projeto

David Barber é uma plataforma web completa desenvolvida para revolucionar a gestão de barbearias, oferecendo um sistema intuitivo de agendamento online. Com design moderno e funcionalidades robustas, o sistema conecta clientes e barbeiros de forma eficiente, proporcionando uma experiência premium do agendamento ao atendimento.

### 🎯 Principais Funcionalidades

- ✅ **Agendamento Online** - Sistema completo de marcação de horários 24/7
- 💈 **Gestão de Serviços** - Catálogo completo de serviços e preços
- 👤 **Perfil de Clientes** - Histórico completo de agendamentos e preferências
- 📅 **Calendário Inteligente** - Visualização clara de horários disponíveis
- 💳 **Pagamento Integrado** - Sistema seguro de pagamentos online
- 📱 **Responsivo** - Funciona perfeitamente em todos os dispositivos
- 🔔 **Notificações** - Lembretes automáticos por email e SMS
- 📊 **Dashboard Administrativo** - Controle total da barbearia
- 🌙 **Modo Escuro** - Interface adaptável para conforto visual
- 🔒 **Segurança** - Autenticação segura e proteção de dados

---

## 🚀 Demonstração

<div align="center">
  
  ### 🎥 Veja o David Barber em Ação
  
  [![Assista ao vídeo de demonstração](https://img.youtube.com/vi/SEU_VIDEO_ID/maxresdefault.jpg)](https://youtu.be/SEU_VIDEO_ID)
  
  *Clique na imagem acima para assistir ao vídeo completo | [Acesse a aplicação](https://davidbarber.netlify.app)*

</div>

---

## 🛠️ Tecnologias Utilizadas

### Frontend
- **React.js** - Biblioteca JavaScript para interfaces
- **TypeScript** - Superset tipado de JavaScript
- **Tailwind CSS** - Framework CSS utilitário
- **React Router** - Navegação entre páginas
- **Framer Motion** - Animações fluidas e modernas
- **Axios** - Cliente HTTP para requisições
- **React Hook Form** - Gerenciamento de formulários
- **Date-fns** - Manipulação de datas

### Backend
- **Node.js** - Ambiente de execução JavaScript
- **Express.js** - Framework web para Node.js
- **MongoDB** - Banco de dados NoSQL
- **Mongoose** - ODM para MongoDB
- **JWT** - Autenticação por tokens
- **Bcrypt** - Criptografia de senhas
- **Nodemailer** - Envio de emails
- **Stripe** - Processamento de pagamentos

### DevOps & Deploy
- **Netlify** - Hospedagem frontend com CI/CD
- **Heroku/Railway** - Deploy do backend
- **Git** - Controle de versão
- **ESLint** - Linter para código limpo
- **Prettier** - Formatação de código

---

## 📦 Instalação

### Pré-requisitos

- Node.js (versão 16 ou superior)
- npm ou yarn
- MongoDB (local ou cloud)
- Conta Stripe (para pagamentos)

### Passo a Passo

1. **Clone o repositório**
```bash
git clone https://github.com/WebCash-inc/DavidBarber.git
cd davidbarber
```

2. **Instale as dependências**
```bash
npm install
# ou
yarn install
```

3. **Configure as variáveis de ambiente**

Crie um arquivo `.env` na raiz do projeto:

```env
# Database
MONGODB_URI=sua_connection_string_mongodb
DATABASE_NAME=davidbarber

# Authentication
JWT_SECRET=seu_jwt_secret_super_seguro
JWT_EXPIRE=7d

# API
API_URL=http://localhost:5000
PORT=5000

# Client
REACT_APP_API_URL=http://localhost:5000

# Email Configuration
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=seu_email@gmail.com
SMTP_PASSWORD=sua_senha_app

# Payment Gateway
STRIPE_PUBLIC_KEY=sua_stripe_public_key
STRIPE_SECRET_KEY=sua_stripe_secret_key

# SMS (Opcional)
TWILIO_ACCOUNT_SID=seu_twilio_sid
TWILIO_AUTH_TOKEN=seu_twilio_token
TWILIO_PHONE_NUMBER=seu_numero_twilio
```

4. **Inicie o servidor de desenvolvimento**

Terminal 1 - Backend:
```bash
cd server
npm run dev
```

Terminal 2 - Frontend:
```bash
npm start
# ou
yarn start
```

5. **Acesse a aplicação**

Abra seu navegador em `http://localhost:3000`

---

## 📁 Estrutura do Projeto

```
davidbarber/
├── src/
│   ├── components/          # Componentes reutilizáveis
│   │   ├── Auth/           # Componentes de autenticação
│   │   ├── Booking/        # Sistema de agendamento
│   │   ├── Services/       # Catálogo de serviços
│   │   ├── Dashboard/      # Painel administrativo
│   │   └── UI/             # Componentes de interface
│   ├── pages/              # Páginas da aplicação
│   │   ├── Home/
│   │   ├── Login/
│   │   ├── Register/
│   │   ├── Booking/
│   │   ├── Profile/
│   │   └── Admin/
│   ├── services/           # Serviços e API calls
│   ├── context/            # Context API
│   ├── hooks/              # Custom hooks
│   ├── utils/              # Funções utilitárias
│   ├── styles/             # Estilos globais
│   └── types/              # TypeScript types
├── server/                 # Backend
│   ├── controllers/        # Controladores
│   │   ├── authController.js
│   │   ├── bookingController.js
│   │   ├── serviceController.js
│   │   └── userController.js
│   ├── models/             # Modelos do banco
│   │   ├── User.js
│   │   ├── Booking.js
│   │   ├── Service.js
│   │   └── Payment.js
│   ├── routes/             # Rotas da API
│   ├── middleware/         # Middlewares
│   ├── utils/              # Utilitários do servidor
│   └── config/             # Configurações
├── public/                 # Arquivos públicos
├── .env.example            # Exemplo de variáveis
├── package.json
└── README.md
```

---

## 🎮 Como Usar

### Para Clientes

1. **Criar Conta**
   - Acesse [davidbarber.netlify.app](https://davidbarber.netlify.app)
   - Clique em "Cadastrar-se"
   - Preencha seus dados
   - Confirme seu email

2. **Fazer Agendamento**
   - Navegue até "Agendar"
   - Escolha o serviço desejado
   - Selecione data e horário disponível
   - Confirme o agendamento

3. **Gerenciar Agendamentos**
   - Acesse "Meus Agendamentos"
   - Visualize histórico completo
   - Reagende ou cancele com antecedência
   - Avalie o serviço recebido

### Para Administradores

1. **Dashboard Administrativo**
   - Acesse com credenciais de admin
   - Visualize agendamentos do dia
   - Gerencie serviços e preços
   - Acompanhe métricas em tempo real

2. **Gestão de Serviços**
   - Adicione novos serviços
   - Defina preços e duração
   - Controle disponibilidade
   - Configure promoções

3. **Controle Financeiro**
   - Acompanhe receitas
   - Exporte relatórios
   - Gerencie pagamentos
   - Monitore cancelamentos

---

## 🎨 Recursos Especiais

### Sistema de Agendamento Inteligente
- Prevenção de conflitos de horários
- Sugestão automática de melhores horários
- Bloqueio de horários indisponíveis
- Fila de espera automática

### Notificações Automáticas
- Email de confirmação de agendamento
- Lembrete 24h antes do horário
- SMS de confirmação (opcional)
- Notificações push no navegador

### Gestão de Fidelidade
- Programa de pontos
- Descontos para clientes frequentes
- Promoções personalizadas
- Histórico de preferências

---

## 🤝 Contribuindo

Contribuições são sempre bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFuncionalidade`)
3. Commit suas mudanças (`git commit -m 'Add: Nova funcionalidade incrível'`)
4. Push para a branch (`git push origin feature/NovaFuncionalidade`)
5. Abra um Pull Request

### Diretrizes de Contribuição

- Siga os padrões de código do projeto
- Escreva commits descritivos em português
- Adicione testes quando aplicável
- Atualize a documentação conforme necessário
- Teste em diferentes navegadores e dispositivos

---

## 🐛 Reportar Problemas

Encontrou um bug? Por favor, abra uma [issue](https://github.com/WebCash-inc/DavidBarber/issues) descrevendo:

- Descrição clara do problema
- Passos para reproduzir
- Comportamento esperado vs atual
- Screenshots ou vídeos (se aplicável)
- Ambiente (navegador, OS, dispositivo)
- Mensagens de erro (se houver)

---

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://github.com/WebCash-inc/DavidBarber/blob/main/LICENSE) para mais detalhes.

---

## 🙏 Agradecimentos

- Barbeiros profissionais que contribuíram com feedback
- Comunidade open source
- Designers que inspiraram o projeto
- Todos os beta testers

---

## 📊 Status do Projeto

![GitHub last commit](https://img.shields.io/github/last-commit/WebCash-inc/DavidBarber?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/WebCash-inc/DavidBarber?style=flat-square)
![GitHub pull requests](https://img.shields.io/github/issues-pr/WebCash-inc/DavidBarber?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/WebCash-inc/DavidBarber?style=flat-square)

---

## 🌟 Roadmap

- [x] Sistema básico de agendamento
- [x] Autenticação de usuários
- [x] Dashboard administrativo
- [x] Integração com pagamentos
- [ ] App mobile (React Native)
- [ ] Sistema de avaliações
- [ ] Programa de fidelidade
- [ ] Integração com redes sociais
- [ ] Suporte multi-idiomas
- [ ] API pública para integrações

---

<div align="center">

**Desenvolvido por WebCash.

[⬆ Voltar ao topo](#-sobre-o-projeto)

</div>
