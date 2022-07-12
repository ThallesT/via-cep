[![Maven Package](https://github.com/ThallesT/via-cep/actions/workflows/maven-publish.yml/badge.svg)](https://github.com/ThallesT/via-cep/actions/workflows/maven-publish.yml)

# VIA-CEP API

> Uma api para projetos java 11+ com repositorio publico para que os artefatos sejam importados.


### Ajustes e melhorias

O projeto ainda está em desenvolvimento e as próximas atualizações serão voltadas nas seguintes tarefas:

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:
* Java 11+


## 🚀 Instalando a api

Para instalar a api do VIA-CEP, adicione ao seu projeto:

Maven:
```XML
<dependencies>
    <dependency>
        <groupId>com.gtbr</groupId>
        <artifactId>via-cep</artifactId>
        <version>1.0.0</version>
    </dependency>
</dependencies>


<repositories>
    <repository>
        <id>repsy</id>
        <url>https://repo.repsy.io/mvn/thalles/via-cep</url>
    </repository>
</repositories>
```
Gradle:
```
implementation 'com.gtbr:via-cep:1.0.0'
```

## ☕ Usando a api


Para buscar um cep:
```JAVA
public static void main(String[] args){
    Cep cep = ViaCepClient.findCep("01001000");
}
```
Caso precise remover a mascara ou mascarar:
```JAVA
public static void main(String[] args){
    CEPUtils.removeMascaraCep("01001-000");
    //ou
    CEPUtils.mascararCep("01001000")
}
```


## 📫 Contribuindo para o projeto
Para contribuir com essa api, siga estas etapas:

1. Bifurque este repositório.
2. Crie um branch: `git checkout -b <nome_branch>`.
3. Faça suas alterações e confirme-as: `git commit -m '<mensagem_commit>'`
4. Envie para o branch original: `git push origin <nome_do_projeto> / <local>`
5. Crie a solicitação de pull.
   

Como alternativa, consulte a documentação do GitHub em [como criar uma solicitação pull](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).

## Escreva testes de unidade
