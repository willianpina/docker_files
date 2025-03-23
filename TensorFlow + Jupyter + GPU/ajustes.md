# 📦 Ambiente Docker: TensorFlow + Jupyter + GPU

Este repositório foi criado para facilitar o uso de **TensorFlow 2.7 (GPU)** com **Jupyter Lab** em projetos particulares ou universitários, além de possibilitar integração direta com o **PyCharm** como interpreter remoto via Docker.

---

## ✅ Recursos:

- Ambiente pré-configurado com TensorFlow GPU.
- Jupyter Lab acessível localmente na porta **8888**, sem token.
- Suporte completo à utilização da GPU (NVIDIA).
- Volume montado para sincronizar o código do host com o container.
- Exemplo de notebook (`Teste.ipynb`) incluído para validação do ambiente.

---

## 📁 Estrutura do repositório:

| Arquivo              | Função                                     |
| -------------------- | ------------------------------------------ |
| `Dockerfile`         | Define a imagem base com TensorFlow GPU.   |
| `docker-compose.yml` | Gerencia o serviço de forma prática.       |
| `entrypoint.sh`      | Script de inicialização do Jupyter Lab.    |
| `Teste.ipynb`        | Notebook de teste para validar o ambiente. |

---

## ▶️ Como usar:

1. Certifique-se de ter instalado:

   - **Docker**
   - **Docker Compose**
   - **NVIDIA drivers** e **Docker NVIDIA Runtime**

2. Clone este repositório:

```bash
git clone https://github.com/willianpina/tensorflow-gpu-pycharm.git
cd tensorflow-gpu-pycharm
```

3. Inicie o ambiente:

```bash
docker-compose up
```

4. Abra o navegador em: [http://localhost:8888](http://localhost:8888)

---

## 💡 Configurando no PyCharm:

1. Vá em: `Settings > Project > Python Interpreter > Add Interpreter > Docker`.
2. Escolha **Docker Compose**, selecione o serviço `tensorflow-gpu` e o interpreter Python correspondente.
3. Confirme e pronto! Agora você pode executar seus notebooks e scripts diretamente do PyCharm com suporte a GPU.

---

> ⭐ Fique à vontade para contribuir ou deixar sugestões!

