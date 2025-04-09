# 💱 Conversor de Unidades

Aplicativo desktop moderno e simples desenvolvido em Java com Swing e FlatLaf para conversão de:

- 💰 **Moedas** (com cotação em tempo real via API)
- 📏 **Comprimento**
- ⚖️ **Massa**
- 🌡️ **Temperatura**
- 💾 **Armazenamento**

---

## 🖥️ Interface

A interface gráfica utiliza o tema escuro moderno fornecido pela [FlatLaf](https://www.formdev.com/flatlaf/):


<img src="/src/main/resources/images/app.png" alt="Interface do aplicativo" width="600"/>

---

## 🚀 Como executar

### Pré-requisitos
- Java 8 ou superior
- Maven instalado

### Passos

1. Clone o repositório:
   ```bash
   git clone https://github.com/apenasMarcos/conversor-de-moedas.git
   cd conversor-de-moedas

2. Gere o .jar executável:
   ```bash
    mvn clean package

3. Execute o aplicativo:
   ```bash
    java -jar target/Conversor-1.1.jar

🌐 Conversão de Moedas

As cotações são obtidas em tempo real da API Economia Awesome, convertendo automaticamente com base no dólar americano.

Moedas suportadas:

    Real (BRL)

    Dólar (USD)

    Euro (EUR)

    Libra Esterlina (GBP)

    Peso Argentino (ARS)

    Peso Chileno (CLP)

📦 Estrutura do Projeto

```plaintext
src/
├── App.java                # Classe principal
├── GUI/                    # Classes para Interface gráfica (Swing)
├── service/
│   ├── Api.java            # Requisições HTTP e parsing da API
│   └── MoneyService.java   # Atualização de cotações
│   └── Coin.java           # Classe genérica de Mapper
├── units/
│   ├── Unit.java           # Classe genérica de unidade
│   ├── Money.java          # Unidade monetária
│   ├── Length.java         # Unidade de comprimento
│   ├── Mass.java           # Unidade de massa
│   ├── DataStorage.java    # Unidade de armazenamento
│   └── Temperature.java    # Unidade de temperatura
```


🧠 Tecnologias usadas

    Java 8

    Swing (interface gráfica)

    FlatLaf (tema escuro moderno)

    Gson (JSON parsing)

    Maven (build e dependências)

    AwesomeAPI (cotação de moedas)

    Junit (Testes Unitarios)

⚠️ Avisos

    As conversões de moedas dependem de conexão com a internet.

📜 Licença

Projeto feito para fins educacionais. Sinta-se livre para usar, adaptar ou contribuir.
