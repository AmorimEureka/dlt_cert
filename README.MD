Walkthrough Certification dlthub
===

<br>
<br>

<details open>
    <summary><strong>PROBLEMA</strong></summary>
    <p></p>

<ul style="list-style-type: none;">

#### **Extrair dados de 5 endpoints da API do Github e carregá-los no BigQuery:**

- ⛧ repos
- ⛧ contributors
- ⛧ issues (Carregamento Incremental)
- ⛧ forks (Carregamento Incremental)
- ⛧ releases

* ⛧ Habilitar logs:
    - ⛧ Monitoria
    - ⛧ Debug

___

<br>

</ul>

</details>



<br>

<details open>
<summary><strong>CONFIGURAÇÃO DO AMBIENTE</strong></summary>

<br>

<ul style="list-style-type: none;">

<li>

Configurar Github

```bash
git init

git branch -m main

```

</li>


<li>

Definir versão Python do projeto:

```bash
pyenv version

pyenv local 3.12.1

pyenv versions
```

</li>


<li>

Criar Ambiente Virual - Poetry:

```bash
# -- Se criou projeto com mkdir
    poetry init

# ou

# -- repo do zero
    poetry new <Nome_Novo_Porjeto>

# -- habilita gerenciamento do projeto p/ poetry
    poetry config virtualenvs.in-project true


# -- Informa versão python definida pelo Pyenv
    poetry env use 3.12.1

# -- Ativa o ambiente virtual
    source .venv/bin/activate
```

</li>


<li>

Instalar Library dlt

```bash
poetry add dlt --python "^3.12"
```

</li>


</ul>

<br>

___

</details>




