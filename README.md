# projetoMinerva
PHP/LARAVEL/REACT NATIVE

# comandos para criação da api
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

choco install composer

git clone https://github.com/devtiagoabreu/projetoMinerva.git .

composer global require laravel/installer 

laravel new api

composer require tymon/jwt-auth 

php artisan vendor:publish --provider="Tymon\JWTAuth\Providers\LaravelServiceProvider"

php artisan jwt:secret
