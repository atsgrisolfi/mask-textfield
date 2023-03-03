# mask textfield
#### Authors: [GRISOLFI, Aline](https://github.com/AlineGrisolfi); GRISOLFI, Álvaro

Usado com kivyMD - MDTextField

mascara para os campos celular (telefone), cep (código endereço postal) cpf (cadastro pessoa fisica)

apos criar o venv, faça uma copia de segurança dos arquivos: 
* venv/lib/python3.10/site-packages/kivymd/uix/textfield/textfield.py 
* venv/lib/python3.10/site-packages/kivymd/uix/textfield/textfield.kv 

substitua-os pelos arquivos contidos aqui no github (observe se sua versão do Python é compativel, não funciona com versão anterior a **3.10**).


para usar, use validator attribute: 
* validator:"phone"
* validator:"cep"
* validator:"cpf"
            
### Exemplo:
     
       MDTextField:
            id:fld_celullar
            pos_hint: {'center_x': 0.5 , 'center_y': 0.7}
            helper_text: "Número do Celular"
            validator:"phone"
             
        MDTextField:
            id:fld_cep
            size_hint_x: .8
            hint_text: 'CEP:'
            pos_hint: {'center_x': 0.5 , 'center_y': 0.6}
            validator:"cep"

        MDTextField:
            id:fld_cpf
            size_hint_x: .8
            hint_text: 'CPF:'
            pos_hint: {'center_x': 0.5 , 'center_y': 0.5}
            validator:"cpf"   

### Caso você  encontre um problema ou queira dar uma sugestão [avise-me](https://github.com/atsgrisolfi/mask-textfield/issues) por favor
