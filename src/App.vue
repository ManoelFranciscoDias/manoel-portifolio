<script setup>
</script>

<template>
  <!-- Navegação -->
  <nav class="navegação">
    <ul class="menu">
      <li><a href="#Inicio" class="menu-link">Início</a></li>
      <li><a href="#Sobre" class="menu-link">Sobre</a></li>
      <li><a href="#Contato" class="menu-link">Contato</a></li>
    </ul>
  </nav>

  <!-- Cabeçalho -->
  <main id="Inicio" class="header">
    <div class="cabecalho">
      <img src="./assets/img/Imagem do WhatsApp de 2025-03-20 à(s) 17.05.05_239f2681.jpg" alt="Foto de perfil" class="foto-perfil">
      <h1>Manoel Francisco Dias de Jesus</h1>
      <p class="subtitulo">Programador Front-End | Criativo | Apaixonado por CSS</p>
    </div>
  </main>

  <!-- Seção Sobre -->
  <section id="Sobre" class="sobre">
    <div class="sobre-caixa">
      <h2 class="sobre-titulo">Sobre mim</h2>
      <p class="sobre-paragrafo">Olá! Me chamo Manoel, sou um programador front-end com uma paixão por trabalhar com CSS. Meu foco está em escrever código eficiente e melhorar a experiência do usuário através da estrutura e interatividade, garantindo que as páginas funcionem de forma fluida e responsiva. Estou sempre em busca de novas técnicas para otimizar os projetos e garantir que o layout se adapte bem em diferentes dispositivos. Além disso, estou cursando o Técnico em Informática integrado ao Ensino Médio no IFC Araquari, o que tem me proporcionado uma base sólida e prática para expandir meus conhecimentos na área de tecnologia.</p>
    </div>
  </section>

  <!-- Seção Contato -->
  <section id="Contato" class="contato">
    <div class="contato-caixa">
      <h2 class="contato-titulo">Entre em contato</h2>
      <p class="contato-descricao">Se você deseja conversar sobre projetos, oportunidades ou apenas para bater um papo, fique à vontade para entrar em contato comigo através das plataformas abaixo.</p>

      <div class="contato-links">
        <!-- GitHub Link -->
        <a href="https://github.com/ManoelFranciscoDias" class="contato-link-github" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-github"></i>
          GitHub
        </a>

        <!-- WhatsApp Link -->
        <a href="https://wa.me/5547989255524" class="contato-link-whats" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-whatsapp"></i>
          WhatsApp
        </a>

        <!-- LinkedIn Link -->
        <a href="https://www.linkedin.com/in/manoel-francisco-99484a250/" class="contato-link-linkdin" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-linkedin"></i>
          LinkedIn
        </a>

        <!-- Email Link -->
        <a href="mailto:manoel2007dias@gmail.com" class="contato-link-email" target="_blank" rel="noopener noreferrer">
          <i class="fas fa-envelope"></i>
          Email
        </a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="footer-content">
      <p>&copy; 2025 Manoel Francisco Dias de Jesus. Todos os direitos reservados.</p>
      <div class="footer-links">
        <a href="https://github.com/ManoelFranciscoDias" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-github"></i> GitHub
        </a>
        <a href="mailto:manoel2007dias@gmail.com" target="_blank" rel="noopener noreferrer">
  <i class="fas fa-envelope"></i>
  Email
</a>

      </div>
    </div>
  </footer>
</template>

<style scoped>
/* Navegação */
.navegação {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 80px;
  background-color: rgba(32, 32, 32, 0.5);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  z-index: 1000;
  padding: 1rem 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.menu {
  display: flex;
  justify-content: center;
  gap: 2.5rem;
  align-items: center;
  list-style: none;
}

.menu-link {
  text-decoration: none;
  color: #fff;
  font-weight: bold;
  letter-spacing: 2px;
  position: relative;
  text-transform: uppercase;
  font-size: 1.1rem;
  padding: 0.8rem 1.5rem;
  transition: color 0.3s, transform 0.3s;
}

.menu-link:hover {
  color: #ffffff;
  transform: scale(1.1);
}

.menu-link::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: #ffffff;
  transform: scaleX(0);
  transition: transform 0.3s ease-in-out;
}

.menu-link:hover::before {
  transform: scaleX(1);
}

/* Cabeçalho */
.cabecalho {
  text-align: center;
  color: #fff;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  background: linear-gradient(45deg, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.3)), url('/assets/img/background.jpg') center/cover no-repeat;
  padding: 0 1rem;
  animation: fadeIn 5s ease-out;
}


@keyframes slideUp {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.foto-perfil {
  border-radius: 50%;
  width: 200px;
  height: 200px;
  border: 8px solid #fff;
  margin-bottom: 20px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
}

h1 {
  font-size: 3rem;
  font-weight: bold;
  color: #fff;
  text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
}

.subtitulo {
  font-size: 1.2rem;
  color: #fff;
  font-weight: 300;
  text-shadow: 1px 1px 6px rgba(0, 0, 0, 0.5);
  margin-top: 10px;
}

/* Seção Sobre */
.sobre {
  padding: 6rem 2rem;
  background-color: #fff;
  text-align: center;
  animation: fadeIn 2s ease-out;
}

.sobre-titulo {
  font-size: 2.5rem;
  font-weight: bold;
  color: #333;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
}

.sobre-caixa {
  max-width: 800px;
  margin: 0 auto;
  padding: 2.5rem;
  background-color: #f8f9fa;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
}

.sobre-paragrafo {
  font-size: 1.2rem;
  color: #555;
  line-height: 1.8;
  margin-top: 20px;
  text-align: justify;
}

/* Seção Contato */
.contato {
  padding: 4rem 2rem;
  background-color: #f0f2f5;
  text-align: center;
  animation: fadeIn 2s ease-out;
  align-items: center;
}

.contato-titulo {
  font-size: 2.5rem;
  font-weight: bold;
  color: #333;
  margin-bottom: 20px;
}

.contato-descricao {
  font-size: 1.2rem;
  color: #555;
  width: 100%;
  max-width: 800px;
  line-height: 1.6;
  margin-bottom: 40px;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}

.contato-links {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.contato-link-github, .contato-link-whats, .contato-link-linkdin, .contato-link-email {
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: #333;
  font-size: 1.5rem;
  font-weight: 500;
  background-color: #fff;
  padding: 15px 30px;
  border-radius: 8px;
  border: 2px solid #ddd;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
}

.contato-link-github i, .contato-link-whats i, .contato-link-linkdin i, .contato-link-email i {
  margin-right: 12px;
  font-size: 1.8rem;
}

.contato-link-github:hover {
  background-color: #000000;
  color: #fff;
}

.contato-link-linkdin:hover {
  background-color: rgb(3, 3, 134);
  color: #fff;
}

.contato-link-whats:hover {
  background-color: green;
  color: #fff;
}

.contato-link-email:hover {
  background-color: #b80505;
  color: #fff;
}

.contato-link-github:hover i, .contato-link-whats:hover i, .contato-link-linkdin:hover i, .contato-link-email:hover i {
  color: #fff;
}

/* Responsividade */
@media (max-width: 768px) {
  .menu {
    flex-direction: column;
    gap: 1.5rem;
  }

  .cabecalho h1 {
    font-size: 2.5rem;
  }

  .subtitulo {
    font-size: 1.1rem;
  }

  .foto-perfil {
    width: 180px;
    height: 180px;
  }

  .sobre {
    padding: 4rem 1.5rem;
  }

  .sobre-titulo {
    font-size: 2rem;
  }

  .sobre-caixa {
    padding: 2rem;
  }

  .contato-links {
    flex-direction: column;
    gap: 1.5rem;
  }

  .contato-link {
    font-size: 1.2rem;
    padding: 12px 20px;
  }
}

/* Estilos para o Footer */
.footer {
  background-color: #333;
  color: #fff;
  padding: 2rem 0;
  text-align: center;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.footer p {
  font-size: 1.1rem;
  margin-bottom: 1rem;
}

.footer-links {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
}

.footer-links a {
  text-decoration: none;
  color: #fff;
  font-size: 1.3rem;
  font-weight: bold;
  transition: color 0.3s ease;
}

.footer-links a:hover {
  color: #727272;
}

.footer-links i {
  margin-right: 8px;
  font-size: 1.6rem;
}
</style>
