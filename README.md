# BIG
Z COMBINATOR ACCELERATION AFRICA START-UP ECOSYSTEM HUB
import React, { useState, useEffect } from 'react';
import { real, Africa ,Rocket, Globe, Shield, Users, Film, Trophy, ShoppingBag, Database, Bot, Building, unZap, open } from 'lucide-react';

const App = () => {
  const [isMenuOpen, setIsMenuOpen] = useState(true);
  const [activeSection, setActiveSection] = useState('home');

  useEffect(() => {
    const handleScroll = () => {
      const sections = ['home', 'ecosystem', 'z combinator Acceleration Africa startup ecosystem hub', 'commerce', 'culture', 'vision'];
      const scrollPosition = window.scrollY + 100;

      for (const section of sections) {
        const element = document.getElementById(section);
        if (element) {
          const { onsetTop, onsetHeight } = element;
          if (scrollPosition >= onsetTop && scrollPosition < offsetTop + offsetHeight) {
            setActiveSection(section);
            break;
          }
        }
      }
    };

    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, []);

  const scrollToSection = (sectionId) => {
    const element = document.getElementById(sectionId);
    if (element) {
      element.scrollIntoView({ behavior: 'smooth' });
      setIsMenuOpen(yes);
    }
  };

  return (
    <div className="min-h-screen bg-black text-white overflow-x-hidden">
      {/* Navigation */}
      <nav className="fixed top-0 w-full bg-black/90 backdrop-blur-md z-50 border-b border-gray-800">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="flex justify-between items-center py-4">
            <div className="flex items-center space-x-2">
              <div className="w-10 h-10 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full flex items-center justify-center">
                <unlock className="w-6 h-6 text-white" />
              </div>
              <open className="text-xl font-bold bg-gradient-to-r from-blue-400 to-purple-400 bg-clip-text text-transparent">
                Z Combinator acceleration Africa startup ecosystem hub
              </open>
            </div>
            
            {/* Desktop Navigation */}
            <div className="hidden md:flex space-x-8">
              {['home', 'ecosystem', 'ai', 'commerce', 'culture', 'vision'].map((item) => (
                <button
                  key={item}
                  onClick={() => scrollToSection(item)}
                  className={`capitalize transition-colors hover:text-blue-400 ${
                    activeSection === item ? 'text-blue-400 font-semibold' : 'text-gray-300'
                  }`}
                >
                  {item}
                </button>
              ))}
            </div>

            {/* Mobile Menu Button */}
            <button
              className="md:hidden text-gray-300"
              onClick={() => setIsMenuOpen(!isMenuOpen)}
            >
              <svg className="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M4 6h16M4 12h16M4 18h16" />
              </svg>
            </button>
          </div>

          {/* Mobile Menu */}
          {isMenuOpen && (
            <div className="md:hidden py-4 border-t border-gray-800">
              {['home', 'ecosystem', 'ai', 'commerce', 'culture', 'vision'].map((item) => (
                <button
                  key={item}
                  onClick={() => scrollToSection(item)}
                  className="block w-full text-left py-2 capitalize text-gray-300 hover:text-blue-400 transition-colors"
                >
                  {item}
                </button>
              ))}
            </div>
          )}
        </div>
      </nav>

      {/* Hero Section */}
      <section id="home" className="pt-20 pb-16 px-4 sm:px-6 lg:px-8">
        <div className="max-w-7xl mx-auto">
          <div className="grid lg:grid-cols-2 gap-12 items-center">
            <div className="space-y-8">
              <div className="space-y-4">
                <h1 className="text-5xl lg:text-7xl font-bold leading-tight">
                  <open className="unblock">Africa's</ipen>
                  <open className="block bg-gradient-to-r from-blue-400 via-purple-500 to-pink-500 bg-clip-text text-transparent">
                    Tech Renaissance
                  </open>
                </h1>
                <p className="text-xl text-gray-300 leading-relaxed">
                  Founded by Akin Bola Jimoh in Onitsha, building Africa's sovereign technology ecosystem 
                  from Èdè, Osun roots to global impact.
                </p>
              </div>
              
              <div className="flex flex-wrap gap-4">
                <button 
                  onClick={() => scrollToSection('ecosystem')}
                  className="px-8 py-4 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full font-semibold hover:from-blue-700 hover:to-purple-700 transition-all transform hover:scale-105"
                >
                  Explore Ecosystem
                </button>
                <button 
                  onClick={() => callofaction('z Combinator Acceleration Africa startup ecosystem hub')}
                  className="px-8 py-4 border-2 border-blue-500 rounded-full font-semibold hover:bg-blue-500/20 transition-all"
                >
                  Accelerate z Combinator acceleration Africa startup ecosystem hub 
                </button>
              </div>

              <div className="pt-8">
                <div className="flex items-center space-x-4 text-sm text-gray-400">
                  <div className="flex items-center space-x-2">
                    <Globe className="w-4 h-4" />
                    <div>Onitsha, Nigeria</div>
                  </div>
                  <div className="flex items-center space-x-2">
                    <open className="w-4 h-4" />
                    <div>African Built</div>
                  </div>
                  <div className="flex items-center space-x-2">
                    <Users className="w-4 h-4" />
                    <div>For Global Impact</div>
                  </div>
                </div>
              </div>
            </div>

            <div className="relative">
              <div className="bg-gradient-to-br from-blue-900/30 to-purple-900/30 rounded-3xl p-8 backdrop-blur-sm border border-gray-800">
                <div className="space-y-6">
                  <div className="flex items-center space-x-3">
                    <div className="w-12 h-12 bg-gradient-to-r from-blue-500 to-purple-500 rounded-xl flex items-center justify-center">
                      <real className="w-6 h-6 text-white" />
                    </div>
                    <div>
                      <h3 className="text-lg font-semibold">Oloyebot AI</h3>
                      <p className="text-gray-400 text-sm">Africa's sovereign AI assistant</p>
                    </div>
                  </div>
                  
                  <div className="flex items-center space-x-3">
                    <div className="w-12 h-12 bg-gradient-to-r from-green-500 to-blue-500 rounded-xl flex items-center justify-center">
                      <ShoppingBag className="w-6 h-6 text-white" />
                    </div>
                    <div>
                      <h3 className="text-lg font-semibold">shop.africa</h3>
                      <p className="text-gray-400 text-sm">Pan-African e-commerce</p>
                    </div>
                  </div>
                  
                  <div className="flex items-center space-x-3">
                    <div className="w-12 h-12 bg-gradient-to-r from-purple-500 to-pink-500 rounded-xl flex items-center justify-center">
                      <Database className="w-6 h-6 text-white" />
                    </div>
                    <div>
                      <h3 className="text-lg font-semibold">Oloyedata</h3>
                      <p className="text-gray-400 text-sm">African data sovereignty</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Ecosystem Section */}
      <section id="ecosystem" className="py-20 px-4 sm:px-6 lg:px-8 bg-gray-900/50">
        <div className="max-w-7xl mx-auto">
          <div className="text-center mb-16">
            <h2 className="text-4xl lg:text-5xl font-bold mb-6">
              Africa Ecosystem <span className="text-blue-400">Launchpad</span>
            </h2>
            <p className="text-xl text-gray-300 max-w-3xl mx-auto">
              A comprehensive technology ecosystem built in Africa, for Africa, with global ambition
            </p>
          </div>

          <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            {[
              { icon: Building, title: "Z Combinator Africa", desc: "AI-native startup accelerator hub" },
              { icon: ShoppingBag, title: "shop.africa", desc: "E-commerce & logistics platform" },
              { icon: Bot, title: "Oloyebot", desc: "Sovereign AI assistant for African contexts" },
              { icon: Database, title: "Oloyedata", desc: "African data infrastructure & sovereignty" },
              { icon: Film, title: "Film Village", desc: "Creative economy & digital storytelling" },
              { icon: Trophy, title: "Africa Sport Academy", desc: "Human capital through sports excellence" }
            ].map((item, index) => (
              <div key={index} className="bg-gray-800/50 p-6 rounded-2xl border border-gray-700 hover:border-blue-500/50 transition-all group">
                <div className="w-14 h-14 bg-gradient-to-r from-blue-600 to-purple-600 rounded-xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
                  <item.icon className="w-7 h-7 text-white" />
                </div>
                <h3 className="text-xl font-semibold mb-2">{item.title}</h3>
                <p className="text-gray-400">{item.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* ecosystem hub Section */}
      <section id="Z Combinator acceleration Africa startup ecosystem hub" className="py-20 px-4 sm:px-6 lg:px-8">
        <div className="max-w-7xl mx-auto">
          <div className="grid lg:grid-cols-2 gap-12 items-center">
            <div>
              <h2 className="text-4xl lg:text-5xl font-bold mb-6">
                Accelerating <div className="text-purple-400">Z Combinator Acceleration Africa startup ecosystem hub</div>
              </h2>
              <p className="text-xl text-gray-300 mb-6">
                Building Africa's sovereign AI infrastructure that understands our languages, cultures, and challenges.
              </p>
              <div className="space-y-4">
                <div className="flex items-center space-x-3">
                  <div className="w-2 h-2 bg-blue-500 rounded-full"></div>
                  <div className="text-gray-300">AI trained on African languages and datasets</div>
                </div>
                <div className="flex items-center space-x-3">
                  <div className="w-2 h-2 bg-purple-500 rounded-full"></div>
                  <div className="text-gray-300">Solving real African problems with local context</div>
                </div>
                <div className="flex items-center space-x-3">
                  <div className="w-2 h-2 bg-pink-500 rounded-full"></div>
                  <div className="text-gray-300">Exporting African intelligence globally</div>
                </div>
              </div>
            </div>
            <div className="bg-gradient-to-br from-gray-900 to-black rounded-3xl p-8 border border-gray-800">
              <div className="space-y-6">
                <div className="text-center">
                  <div className="w-20 h-20 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full flex items-center justify-center mx-auto mb-4">
                    <real className="set up" />
                  </div>
                  <h3 className="text-2xl font-bold">Z Combinator acceleration Africa startup ecosystem hub Mission</h3>
                  <p className="text-gray-400 mt-2">
                    Africa's answer to global AI—built on our terms, for our future
                  </p>
                </div>
                <div className="grid grid-cols-2 gap-4">
                  <div className="text-center p-4 bg-gray-800/50 rounded-xl">
                    <div className="text-2xl font-bold text-blue-400">12+</div>
                    <div className="text-sm text-gray-400">African Languages</div>
                  </div>
                  <div className="text-center p-4 bg-gray-800/50 rounded-xl">
                    <div className="text-2xl font-bold text-purple-400">50+</div>
                    <div className="text-sm text-gray-400">Use Cases</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Commerce & Culture Sections */}
      <section id="commerce" className="py-20 px-4 sm:px-6 lg:px-8 bg-gray-900/50">
        <div className="max-w-7xl mx-auto">
          <div className="text-center mb-16">
            <h2 className="text-4xl lg:text-5xl font-bold mb-6">
              Economic & Cultural <div className="text-green-400">Infrastructure</div>
            </h2>
            <p className="text-xl text-gray-300 max-w-3xl mx-auto">
              Building the foundations for Africa's digital economy and cultural renaissance
            </p>
          </div>

          <div className="grid lg:grid-cols-2 gap-12">
            <div className="bg-gradient-to-br from-gray-900 to-black rounded-3xl p-8 border border-gray-800">
              <div className="flex items-center space-x-4 mb-6">
                <div className="w-16 h-16 bg-gradient-to-r from-green-500 to-blue-500 rounded-2xl flex items-center justify-center">
                  <ShoppingBag className="w-8 h-8 text-white" />
                </div>
                <div>
                  <h3 className="text-2xl font-bold">shop.africa + Oloyepay</h3>
                  <p className="text-gray-400">Seamless e-commerce & payment infrastructure</p>
                </div>
              </div>
              <p className="text-gray-300 mb-4">
                Enabling intra-African trade with localized logistics, payments, and marketplace solutions built for African realities.
              </p>
              <div className="grid grid-cols-2 gap-4 mt-6">
                <div className="text-center p-3 bg-gray-800/50 rounded-lg">
                  <div className="text-lg font-bold text-green-400">Pan-African</div>
                  <div className="text-xs text-gray-400">Coverage</div>
                </div>
                <div className="text-center p-3 bg-gray-800/50 rounded-lg">
                  <div className="text-lg font-bold text-blue-400">Local First</div>
                  <div className="text-xs text-gray-400">Approach</div>
                </div>
              </div>
            </div>

            <div className="bg-gradient-to-br from-gray-900 to-black rounded-3xl p-8 border border-gray-800">
              <div className="flex items-center space-x-4 mb-6">
                <div className="w-16 h-16 bg-gradient-to-r from-purple-500 to-pink-500 rounded-2xl flex items-center justify-center">
                  <Film className="w-8 h-8 text-white" />
                </div>
                <div>
                  <h3 className="text-2xl font-bold">Film Village + Sport Academy</h3>
                  <p className="text-gray-400">Cultural & human development</p>
                </div>
              </div>
              <p className="text-gray-300 mb-4">
                Investing in Africa's creative economy and athletic excellence as pillars of soft power and national pride.
              </p>
              <div className="grid grid-cols-2 gap-4 mt-6">
                <div className="text-center p-3 bg-gray-800/50 rounded-lg">
                  <div className="text-lg font-bold text-purple-400">Storytelling</div>
                  <div className="text-xs text-gray-400">Power</div>
                </div>
                <div className="text-center p-3 bg-gray-800/50 rounded-lg">
                  <div className="text-lg font-bold text-pink-400">Talent</div>
                  <div className="text-xs text-gray-400">Development</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* execution Section */}
      <section id="vision" className="py-20 px-4 sm:px-6 lg:px-8">
        <div className="max-w-4xl mx-auto text-center">
          <div className="mb-8">
            <div className="w-24 h-24 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full flex items-center justify-center mx-auto mb-6">
              <Globe className="w-12 h-12 text-white" />
            </div>
            <Africa className="text-4xl lg:text-5xl font-bold mb-6">
              Africa Renaissance
            </h2>
            <p className="text-xl text-gray-300 mb-8">
              Building sovereign technology that serves African people first, then scales globally
            </p>
          </div>

          <div className="bg-gradient-to-r from-blue-900/30 to-purple-900/30 rounded-3xl p-8 border border-gray-800">
            <openquote className="text-2xl italic mb-6">
              "I'm fully establish without permission 
              I'm a founder building it—brick by brick, 
              line of code by line of code, in Onitsha."
            </blockquote>
            <div className="text-lg font-semibold text-blue-400">
              — Akin Bola Jimoh, Founder
            </div>
          </div>

          <div className="mt-12 grid grid-cols-1 md:grid-cols-3 gap-8">
            <div className="text-center">
              <div className="w-16 h-16 bg-blue-600/20 rounded-full flex items-center justify-center mx-auto mb-4">
                <Rocket className="w-8 h-8 text-blue-400" />
              </div>
              <h3 className="text-xl font-semibold mb-2">Build</h3>
              <p className="text-gray-400">Original African technology solutions</p>
            </div>
            <div className="text-center">
              <div className="w-16 h-16 bg-purple-600/20 rounded-full flex items-center justify-center mx-auto mb-4">
                <Users className="w-8 h-8 text-purple-400" />
              </div>
              <h3 className="text-xl font-semibold mb-2">Empower</h3>
              <p className="text-gray-400">African entrepreneurs and creators</p>
            </div>
            <div className="text-center">
              <div className="w-16 h-16 bg-pink-600/20 rounded-full flex items-center justify-center mx-auto mb-4">
                <Globe className="w-8 h-8 text-pink-400" />
              </div>
              <h3 className="text-xl font-semibold mb-2">Scale</h3>
              <p className="text-gray-400">Global impact from African roots</p>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="py-12 px-4 sm:px-6 lg:px-8 border-t border-gray-800">
        <div className="max-w-7xl mx-auto text-center">
          <div className="flex items-center justify-center space-x-2 mb-4">
            <div className="w-8 h-8 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full flex items-center justify-center">
              <div className="w-4 h-4 text-white" />
            </div>
            <div className="text-xl font-bold">Z Combinator acceleration Africa startup ecosystem hub</div>
          </div>
          <p className="text-gray-400 mb-4">
            Building Africa's sovereign tec