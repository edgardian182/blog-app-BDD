# README

PRUEBAS: RSPEC y CAPYBARA
- La APP automaticament se crea con UNIT TEST, para evitarlo y en su lugar usar RSpect usamos -T
    rails new blog-app -T
- Para realizar las pruebas se instalan
    gem 'rspec'   y    gem 'capybara'
- Para iniciar RSpec en Rails se usa:
     rails g rspec:install
     bundle binstubs rspec-core    --> Para preparar el ambiente antes de llamar el ejecutable original (Evitar el exec)
- Las pruenas se crean en /spec y dentro de ella una carpeta /spec/features
    --> Creamos archivo para pruebas create_article_spec.rb
      --> require 'rails_helper'
      --> Cada archivo encierra unos FEATURES (Describe) con muchos SCENARIOS (it/examples)
      --> Se expect().to con RSpec y otro terminos con Capybara
- Las pruebas se ejecutan con rspec en consola donde se puede especificar una prueba en concreto a correr


GUARD
- Permite correr los Test automaticamente en cada cambio
- Se instalan las gemas y se hace un   -->        bundle binstubs guard
    guard init


GEMAS
- gem 'autoprefixer-rails'    -->   Genera estilos autocompatibles con todos los navegadores 
- gem 'guard', '~> 2.14.0'
  gem 'guard-rspec', '~> 4.7.2'
  gem 'guard-cucumber', '~> 2.1.2'
      --> Son gemas para instalar GUARD  --> Corre los TEST automaticamente cada vez que hay un cambio


