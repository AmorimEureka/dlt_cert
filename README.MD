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

&nbsp;&nbsp;&nbsp;&nbsp;<details>
&nbsp;&nbsp;&nbsp;&nbsp;<summary><strong>Configurar Github</strong></summary>

&nbsp;&nbsp;&nbsp;&nbsp;```bash
&nbsp;&nbsp;&nbsp;&nbsp;git init

&nbsp;&nbsp;&nbsp;&nbsp;git branch -m main

&nbsp;&nbsp;&nbsp;&nbsp;```

&nbsp;&nbsp;&nbsp;&nbsp;</details>

<br>

&nbsp;&nbsp;&nbsp;&nbsp;<details>
&nbsp;&nbsp;&nbsp;&nbsp;<summary><strong>Definir versão Python do projeto:</strong></summary>

&nbsp;&nbsp;&nbsp;&nbsp;```bash
&nbsp;&nbsp;&nbsp;&nbsp;pyenv version

&nbsp;&nbsp;&nbsp;&nbsp;pyenv local 3.12.1

&nbsp;&nbsp;&nbsp;&nbsp;pyenv versions
&nbsp;&nbsp;&nbsp;&nbsp;```

&nbsp;&nbsp;&nbsp;&nbsp;</details>

<br>

&nbsp;&nbsp;&nbsp;&nbsp;<details open>
&nbsp;&nbsp;&nbsp;&nbsp;<summary><strong>Criar Ambiente Virual - Poetry:</strong></summary>

&nbsp;&nbsp;&nbsp;&nbsp;```bash
&nbsp;&nbsp;&nbsp;&nbsp;# -- Se criou projeto com mkdir
&nbsp;&nbsp;&nbsp;&nbsp;    poetry init

&nbsp;&nbsp;&nbsp;&nbsp;# ou

&nbsp;&nbsp;&nbsp;&nbsp;# -- repo do zero
&nbsp;&nbsp;&nbsp;&nbsp;    poetry new <Nome_Novo_Porjeto>

&nbsp;&nbsp;&nbsp;&nbsp;# -- habilita gerenciamento do projeto p/ poetry
&nbsp;&nbsp;&nbsp;&nbsp;    poetry config virtualenvs.in-project true


&nbsp;&nbsp;&nbsp;&nbsp;# -- Informa versão python definida pelo Pyenv
&nbsp;&nbsp;&nbsp;&nbsp;    poetry env use 3.12.1

&nbsp;&nbsp;&nbsp;&nbsp;# -- Ativa o ambiente virtual
&nbsp;&nbsp;&nbsp;&nbsp;    source .venv/bin/activate
&nbsp;&nbsp;&nbsp;&nbsp;```

&nbsp;&nbsp;&nbsp;&nbsp;</details>

<br>

&nbsp;&nbsp;&nbsp;&nbsp;<details>
&nbsp;&nbsp;&nbsp;&nbsp;<summary><strong>Instalar Library dlt</strong></summary>

&nbsp;&nbsp;&nbsp;&nbsp;```bash
&nbsp;&nbsp;&nbsp;&nbsp;poetry add dlt --python "^3.12"
&nbsp;&nbsp;&nbsp;&nbsp;```

&nbsp;&nbsp;&nbsp;&nbsp;</details>

<br>

___

</details>




