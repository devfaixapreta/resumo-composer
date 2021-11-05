# Resumo Composer

## Instalação do Composer
* [Link download Composer](https://getcomposer.org/download/)


# Criando um pacote para composer
* Criar repositorio no github
* Criar o arquivo composer.json (composer init)
* Criar conta no Packagist.org
* [Gerenciador de pacotes Packagist.org](https://packagist.org/) 

* Submeter o link do github no Packagist.org
* [Criar pacote Packagist.org](https://packagist.org/packages/submit)

# Comandos Composer

## init
* Cria o arquivo composer.json
```
$ composer init
``` 

## require
* Adicionar uma dependência ao projeto
```
$ composer require <devfaixapreta/packages> "vazio, branch ou versao"
```

exemplo composer.json
```
{
    "require": {
    "devfaixapreta/package": "*, versao ou branch"
    }
}
```

* Adicionar um endereço de repositorio de dependencias
Podendo assim adicionar um repositorio github como dependencia no projeto
*obs:. O repositório para servir como pacote, precisa ter um composer.json com "name"

exemplo composer.json
```
"repositories": [
        {
            "type": "git",
            "url": "https://github.com/devfaixapreta/package"
        }
    ],

    "require": {
        "devfaixapreta/package": "*, versao, ou branch"
    }
```

## install
* Instala os pacotes do arquivo composer.json
```
$ composer install
```

## --version
* Mostra a versão do composer instalada
```
$ composer --version
```

## self-update
* Atualiza o composer para a última versão
```
$ composer self-update
```



