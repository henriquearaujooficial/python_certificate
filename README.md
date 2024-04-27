# Certificado em Python
# Projeto Integrador onde iermos usar o serviço Python na geração dos certificados 
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/henriquearaujooficial/Portfolio/blob/master/LICENSE)

## 🛠️ Projeto construído usando:
- Python

# Certificado em Python e suas descrições:

Uma descrição do que cada parte do código faz:

1 - Classe EditCertificate: Esta classe é responsável por criar certificados dinamicamente e enviar por e-mail para os destinatários listados em um arquivo Excel.

2 - Método __init__: O construtor da classe que inicializa os atributos user_email e user_password com o endereço de e-mail e senha do remetente. Em seguida, chama os métodos read_data() e send_email_with_certificate().

3 - Método read_data(): Este método lê os dados do arquivo Excel 'listaatual.xlsx' e armazena em um DataFrame do pandas.

4 - Método send_email_with_certificate(): Itera sobre cada linha do DataFrame, extrai o nome e o e-mail do destinatário e chama o método create_certificate() para gerar um certificado com o nome fornecido. Em seguida, chama o método send_email_generic() para enviar um e-mail personalizado com o certificado anexado.

5 - Método create_certificate(name): Este método cria um certificado usando uma imagem de modelo chamada 'template.png'. Ele escreve o nome do destinatário e a data atual no certificado usando fontes específicas e salva o certificado com o nome do destinatário.

6 - Método send_email_generic(name, email, certificate_image): Este método envia um e-mail personalizado para o destinatário com o certificado anexado. Utiliza a biblioteca Yagmail para enviar e-mails através do SMTP do Gmail.

7 - Instância da classe EditCertificate: No final do código, cria-se uma instância da classe EditCertificate, passando o endereço de e-mail e a senha do remetente como argumentos para iniciar o processo de envio de e-mails com certificados.

Link para o post no Medium: [Criando certificado em Python](https://github.com/henriquearaujooficial/python_certificate/tree/main)

![gameScreen](./template.png)
