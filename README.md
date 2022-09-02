# ![alt text](https://contaja.com.br/wp-content/themes/contaja/images/contaja-contabilidade-online-logo-2.svg)

# Processo Seletivo Front-End ContaJà

A ContaJá é uma empresa especialista em aberturas de empresas de todo Brasil com processos qualificados e ágeis.

Para que nossos clientes possam desfrutar de uma boa experiência em nossa plataforma de onboarding, nossa equipe de experiência do usuário coletou todos os dados necessários para planejar um novo fluxo de coleta de dados.

Com o novo fluxo planejado, a equipe de prototipação estudou todos os fluxos e implementou a nossa nova interface, você pode conferir como ficou: [Interface do Usuário](http://exemplo.com/).

Uma API foi desenvolvida com todas as funcionalidades necessárias para o desenvolvimento do front-end de forma desacoplada do back-end. Você pode verificar como ficou essas rotas agora mesmo: [API](https://drive.google.com/drive/folders/1ZFXsXljGKcYGUif0ezkiJ8ldHsGvu4kY?usp=sharing).

O projeto contendo o back-end vai ser compartilhado com você através do seu email, qualquer dúvida é só entrar em contato. As instruções para rodar o projeto back-end em sua máquina são:

```
git clone [Vamos te mandar por email o compartilhamento da branch]
cd onboarding-contaja-total
cp .env.example .env  
docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php81-composer:latest \
    composer install --ignore-platform-reqs
sail up -d
sail artisan migrate --seed
```

Para utilizar o comando sail diretamente você pode configurar no seu arquivo .bashrc o seguinte comando:
```
alias sail='bash vendor/bin/sail'
```

O arquivo .env configurado pode ser acessado em: [.env](https://drive.google.com/drive/folders/1sl4n0k896PAPKL-btydpKighKLsQGvHH?usp=sharing)

# E o que você deve fazer ?
O seu objetivo aqui é replicar o front-end desenvolvido acoplado com o back-end, de maneira totalmente independente. Além disso, aplicar suas habilidades de front-end para verificar a responsividade das telas e os padrões projetados. 
