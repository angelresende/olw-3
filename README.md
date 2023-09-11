<p align="center"><a href="https://openlaravelweek.com.br/p1-v1/" target="_blank"><img src="https://openlaravelweek.com.br/wp-content/uploads/elementor/thumbs/logo-full-qbjas20thlvqxd4b5tu7mwy5bx76yerw76w8jjcxkk.png" width="650"></a></p>

# Ambiente
- Windows com WSL2
- VS Code

# Passos

<h3>Criação do ambiente através de linha de comando:</h3>
<p>curl -s "https://laravel.build/olw-3?with=mysql,redis,mailpit" | bash</p> 

<h3>Criação do alias para comandos:</h3>
- Edição do arquivo (utilizando nano): alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail

<h3>Iniciando os containers:</h3>
 sail up -d

<h3>Instalando os recursos de autenticação:</h3>
 sail composer require laravel/breeze --dev
 sail artisan breeze:install 
 sail artisan migrate

<h3>Testando registro via breeze.</h3>

