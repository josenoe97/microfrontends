Projeto para aprofundamento em microfrontends.

npx @angular/cli@20 new vendas // Comandos usado para criação do host:vendas

git rm -r --cached vendas// limpeza de cache do git

npx @angular/cli@20 new produtos

npx @angular/cli@20 new grafico

npx ng add @angular-architects/module-federation@20.0.0 --project vendas --port 4200 --type host --skip-confirmation// microfrontend de vendas

npx ng add @angular-architects/module-federation@20.0.0 --project produtos --port 4201 --type remote --skip-confirmation // microfrontend de produtos

npx ng add @angular-architects/module-federation@20.0.0 --project grafico --port 4202 --type remote --skip-confirmation// microfrontend de grafico

npx ng generate c home // para vendas(host)

npx ng g c navbar // para vendas(host)

npx ng add chart.js@4.5.1 //comando gráfico