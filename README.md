# mask_textfield
# author:Aline Grisolfi
# author:Álvaro Grisolfi

mascara para os campos celular (telefone), cep (código endereço postal) cpf (cadastro pessoa fisica)




apos criar o venv, faça uma copia de segurança do arquivo: venv/lib/python3.10/site-packages/kivymd/uix/textfield/textfield.py 
substitua pelo arquivo contido aqui no github (observe se sua versão do Python é compativel, não funciona com versão anterior a 3.10).


para usar, mas colocar o 
         validator:"phone"
         validator:"cep"
         validator:"cpf"
            


       MDTextField:
            id:fld_celullar
            size_hint_x: .8
            hint_text: 'Celular:(xx)x xxxx-xxxx'
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

