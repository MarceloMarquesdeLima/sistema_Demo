# Sistema
* Criar o sistema com o comando ng new sistema

* Na estrutura do projeto no vscode ou outra idei que utilize para trabalho, adicione as seguintes dependencia no projejeto:

* npm install --save-dev electron && npm i electron-builder

* Após a instalação do recurso inclua no script do packege.json na parte dos comando de execusão e build as seguintes linhas:
* "electron": "ng build --base-href ./ && electron .",
* "dist": "ng build --base-href ./ && electron-builder"

* Agora só rodar utilizando estes comando para ter a aplicação descktop em angular
