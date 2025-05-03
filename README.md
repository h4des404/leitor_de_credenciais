# Leitor de Credenciais `.txt`

Uma aplicação simples em Python com interface gráfica (Tkinter) para leitura e extração de credenciais de arquivos `.txt`. Útil para analistas de segurança, pentesters ou administradores que precisam analisar dumps de credenciais estruturadas em formatos variados.

---

### 🖥️ Funcionalidades

- Interface gráfica amigável com **Tkinter**.
- Leitura de arquivos `.txt` contendo credenciais no formato:
  - `URL: site.com USER: admin PASS: 123456`
  - ou em três linhas separadas: 
    ```
    URL: site.com
    USER: admin
    PASS: 123456
    ```
  - ou em formato reduzido: `site.com:admin:123456`
- Filtro por palavra-chave (em URL, usuário ou senha).
- Evita exibir credenciais duplicadas.
- Possibilidade de **parar a busca** em andamento.
- Área de resultado com **scroll**.
- Totalmente offline — nenhum dado é enviado para fora da aplicação.

---

### 🚀 Como Executar

1. **Requisitos:**

   - Python 3.7 ou superior
   - Bibliotecas nativas do Python (não é necessário instalar nada extra)

2. **Clone o repositório ou baixe o script:**

   ```bash
   git clone https://github.com/seu-usuario/leitor-credenciais.git
   cd leitor-credenciais
   ```

3. **Execute o script:**

   ```bash
   python leitor_credenciais.py
   ```

   > Obs: Se estiver usando Windows, clique duas vezes no `.py` se a associação com Python estiver configurada.

---

### 💡 Exemplo de Uso

Imagine que você recebeu um dump de credenciais extraído de uma análise forense, e o conteúdo é parecido com:

```
URL: ftp.empresa.com
USER: suporte
PASS: 123456

URL: painel.empresa.com USER: admin PASS: senha123

exemplo.com:user1:abc123
```

Com essa aplicação, você pode:

- Carregar o arquivo `.txt` contendo as credenciais.
- Inserir palavras-chave como `admin`, `painel` ou `ftp` para filtrar rapidamente os dados relevantes.
- Parar a busca a qualquer momento.
- Evitar repetição de credenciais já processadas.

---

### 🛠️ Estrutura do Projeto

```
📁 leitor-credenciais
├── leitor_credenciais.py
└── README.md
```

---

### 🙋‍♂️ Autor

Desenvolvido por **h4des404**  
💀 Discord: [discord.gg/d34athsec](https://discord.gg/d34athsec)

---

### 📜 Licença

Este projeto está sob a licença MIT. Sinta-se livre para utilizar, modificar e distribuir com os devidos créditos.
