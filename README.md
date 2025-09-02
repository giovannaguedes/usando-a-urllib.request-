# usando-a-urllib.request-
código no modo interativo usando a urllib.request. 

⚠️ Uso exclusivo para fins educacionais • Desenvolvido por M!ss s3c

📝 Guia: Explorando sites com urllib.request em Python

1. Abrir o Python interativo

No terminal, digite:

python3


Você verá o prompt interativo >>>.

2. Importar a biblioteca
>>> from urllib.request import urlopen

3. Abrir um site
>>> site = urlopen("http://nome do site aqui.com.br")

4. Ler o conteúdo da página
>>> print(site.read())  # lê o conteúdo completo

5. Verificar o código HTTP da resposta
>>> print(site.getcode())  # retorna 200, 404, etc.

6. Obter a URL acessada
>>> print(site.geturl())

7. Verificar informações do cabeçalho HTTP
>>> print(site.info())  # mostra todos os headers

8. Consultar o servidor web
>>> head = site.info()
>>> print(head['Server'])

9. Sair do modo interativo
>>> exit()

👉 O que você aprendeu aqui

urlopen() → abre uma URL e retorna um objeto de resposta.

.read() → lê o conteúdo HTML da página.

.getcode() → retorna o código de status HTTP (200 → OK, 404 → Not Found, etc.).

.geturl() → retorna a URL final acessada (útil em redirecionamentos).

.info() → retorna os cabeçalhos HTTP.

Cabeçalho Server → identifica o servidor web utilizado.

O Python interativo é útil para testes rápidos sem criar arquivos.
