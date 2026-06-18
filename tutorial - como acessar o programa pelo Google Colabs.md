# Tutorial – Executando o notebook no Google Colab

## 1. Acessando o Google Colab

Acesse o Google Colab e entre com uma conta Google.

O Colab permite executar notebooks Python diretamente no navegador, sem necessidade de instalar programas no computador.

## 2. Abrindo o notebook

1. Clique em **Arquivo → Abrir notebook**.
2. Selecione a aba **GitHub**.
3. No campo de busca, cole o endereço do repositório:

```text
https://github.com/Erik-Roberto/aula-UNIFAC
```

4. Clique em **Pesquisar**.
5. Selecione o arquivo **unifac.ipynb**.

![alt text](imagens\importanto_notebook.png)

O notebook será aberto no Colab. Entretanto, os demais arquivos do repositório ainda não estarão disponíveis no ambiente de execução.

## 3. Clonando o repositório

Crie uma nova célula de código clicando em **+ Código**.

![alt text](imagens\criando_nova_celula.png)

Cole o código abaixo na célula criada:

```python
!git clone https://github.com/Erik-Roberto/aula-UNIFAC.git
%cd aula-UNIFAC
```

Execute a célula clicando no botão de execução à esquerda.

![alt text](imagens\botao_executar.png)

Na primeira execução, o Colab exibirá uma mensagem informando que o notebook foi criado por outra pessoa. Clique em **Executar assim mesmo** para continuar.

Após a execução da célula, todos os arquivos do repositório estarão disponíveis e o notebook poderá ser executado normalmente.

## 4. Executando o notebook

Com o repositório clonado, execute as células do notebook na ordem em que aparecem ou clicando em **Executar tudo** na barra de ferramentas.

O ambiente estará configurado da mesma forma utilizada durante a aula.

Opcionalmente, a célula utilizada para clonar o repositório pode ser removida após sua execução.
