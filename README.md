import React from 'react';
import { Github, Linkedin, Mail, Code2, Rows as Browser, Database, Terminal } from 'lucide-react';

function App() {
  return (
    <div className="min-h-screen bg-gray-50">
      {/* Header/Hero Section */}
      <header className="bg-gradient-to-r from-blue-600 to-blue-800 text-white">
        <div className="container mx-auto px-6 py-24">
          <div className="flex flex-col items-center text-center">
            <img
              src="https://images.unsplash.com/photo-1539571696357-5a69c17a67c6?w=400&h=400&fit=crop"
              alt="Foto de Perfil"
              className="w-32 h-32 rounded-full border-4 border-white shadow-xl mb-6"
            />
            <h1 className="text-4xl md:text-5xl font-bold mb-4">João Silva</h1>
            <p className="text-xl md:text-2xl text-blue-100 mb-8">Desenvolvedor Full Stack</p>
            <div className="flex gap-4">
              <a href="#" className="text-white hover:text-blue-200 transition-colors">
                <Github size={24} />
              </a>
              <a href="#" className="text-white hover:text-blue-200 transition-colors">
                <Linkedin size={24} />
              </a>
              <a href="#" className="text-white hover:text-blue-200 transition-colors">
                <Mail size={24} />
              </a>
            </div>
          </div>
        </div>
      </header>

      {/* Sobre Section */}
      <section className="py-20">
        <div className="container mx-auto px-6">
          <h2 className="text-3xl font-bold text-center mb-12">Sobre Mim</h2>
          <div className="max-w-3xl mx-auto text-lg text-gray-600 leading-relaxed">
            <p className="mb-6">
              Olá! Sou um desenvolvedor full stack apaixonado por criar soluções web inovadoras e
              eficientes. Com mais de 5 anos de experiência no desenvolvimento de aplicações web,
              especializo-me em React, Node.js e arquiteturas cloud.
            </p>
            <p>
              Busco constantemente aprender novas tecnologias e melhores práticas para entregar
              produtos de alta qualidade que fazem a diferença na vida dos usuários.
            </p>
          </div>
        </div>
      </section>

      {/* Habilidades Section */}
      <section className="py-20 bg-white">
        <div className="container mx-auto px-6">
          <h2 className="text-3xl font-bold text-center mb-12">Habilidades</h2>
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div className="p-6 bg-gray-50 rounded-lg text-center">
              <Code2 className="w-12 h-12 mx-auto mb-4 text-blue-600" />
              <h3 className="text-xl font-semibold mb-4">Frontend</h3>
              <p className="text-gray-600">
                React, TypeScript, Tailwind CSS, Next.js
              </p>
            </div>
            <div className="p-6 bg-gray-50 rounded-lg text-center">
              <Terminal className="w-12 h-12 mx-auto mb-4 text-blue-600" />
              <h3 className="text-xl font-semibold mb-4">Backend</h3>
              <p className="text-gray-600">
                Node.js, Express, NestJS, Python
              </p>
            </div>
            <div className="p-6 bg-gray-50 rounded-lg text-center">
              <Database className="w-12 h-12 mx-auto mb-4 text-blue-600" />
              <h3 className="text-xl font-semibold mb-4">Banco de Dados</h3>
              <p className="text-gray-600">
                PostgreSQL, MongoDB, Redis
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Projetos Section */}
      <section className="py-20">
        <div className="container mx-auto px-6">
          <h2 className="text-3xl font-bold text-center mb-12">Projetos em Destaque</h2>
          <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
            <div className="bg-white rounded-lg overflow-hidden shadow-lg">
              <img
                src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=800&h=500&fit=crop"
                alt="Projeto E-commerce"
                className="w-full h-48 object-cover"
              />
              <div className="p-6">
                <h3 className="text-xl font-semibold mb-2">E-commerce Platform</h3>
                <p className="text-gray-600 mb-4">
                  Plataforma completa de e-commerce desenvolvida com React, Node.js e PostgreSQL.
                  Implementação de pagamentos, gestão de produtos e análises em tempo real.
                </p>
                <a href="#" className="text-blue-600 hover:text-blue-800 font-medium flex items-center gap-2">
                  <Browser size={20} />
                  Ver Projeto
                </a>
              </div>
            </div>
            <div className="bg-white rounded-lg overflow-hidden shadow-lg">
              <img
                src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=800&h=500&fit=crop"
                alt="App de Gestão"
                className="w-full h-48 object-cover"
              />
              <div className="p-6">
                <h3 className="text-xl font-semibold mb-2">Sistema de Gestão</h3>
                <p className="text-gray-600 mb-4">
                  Dashboard administrativo para gestão de equipes e projetos. 
                  Desenvolvido com Next.js, TypeScript e integração com várias APIs.
                </p>
                <a href="#" className="text-blue-600 hover:text-blue-800 font-medium flex items-center gap-2">
                  <Browser size={20} />
                  Ver Projeto
                </a>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Contato Section */}
      <section className="py-20 bg-gray-900 text-white">
        <div className="container mx-auto px-6 text-center">
          <h2 className="text-3xl font-bold mb-8">Vamos Conversar?</h2>
          <p className="text-gray-300 mb-8 max-w-2xl mx-auto">
            Estou sempre interessado em novos projetos e oportunidades de colaboração.
            Se você tem um projeto em mente, não hesite em entrar em contato!
          </p>
          <a
            href="mailto:contato@exemplo.com"
            className="inline-flex items-center gap-2 bg-blue-600 text-white px-8 py-3 rounded-lg hover:bg-blue-700 transition-colors"
          >
            <Mail size={20} />
            Enviar Email
          </a>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-gray-900 text-gray-400 py-8">
        <div className="container mx-auto px-6 text-center">
          <p>© 2024 João Silva. Todos os direitos reservados.</p>
        </div>
      </footer>
    </div>
  );
}

export default App;  
