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
## dump
* Atualiza o arquivo autoload.php
```
$ composer dump
```
# Instalando e Atualizando Composer

## install
* Instala os pacotes do arquivo composer.json
```
$ composer install
```

## update
* Atualiza os paoctes em relação ao seu composer.json. O composer.lock será atualizado.
```
$ composer update
```

## require {pacote}
* Atualiza ou instala a versão do pacote mais recente. O composer.lock e o composer.json serão atualizados.
```
$ composer require {nomedopacote}
```

## remove {pacote}
* Desinstala um pacote.
```
$ composer remove {pacote}
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

## self-update --rollback
* Retorna para a versão anterior
```
$ composer self-update --rollback
```



