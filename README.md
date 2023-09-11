<p align="center"><a href="https://openlaravelweek.com.br/p1-v1/" target="_blank"><img src="https://openlaravelweek.com.br/wp-content/uploads/elementor/thumbs/logo-full-qbjas20thlvqxd4b5tu7mwy5bx76yerw76w8jjcxkk.png" width="650"></a></p>

# Ambiente
- Windows com WSL2
- VS Code

# Passos

<p>Criação do ambiente através de linha de comando:</p>
 curl -s "https://laravel.build/olw-3?with=mysql,redis,mailpit" | bash

<p>Criação do alias para comandos:</p>
- Edição do arquivo (utilizando nano).
 alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail

<p>Iniciando os containers:</p>
 sail up -d

<p>Instalando os recursos de autenticação:</p>
 sail composer require laravel/breeze --dev
 sail artisan breeze:install 
 sail artisan migrate

<p>Testando registro via breeze.</p>

