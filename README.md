# 💱 Conversor de Moedas – Java

Este projeto é um **Conversor de Moedas** desenvolvido em **Java**, utilizando a API de taxas de câmbio para converter valores entre diferentes moedas em tempo real.

---

## 🚀 Funcionalidades

- Conversão entre as principais moedas internacionais.
- Consulta automática à API de câmbio.
- Interface de console simples e intuitiva.
- Tratamento de erros (valores inválidos, moedas inexistentes, problemas na API).
- Código organizado em classes separadas para facilitar manutenção.

---

## 🧰 Tecnologias Utilizadas

- **Java 17+**
- **Maven**
- Biblioteca JSON:
  ```xml
  <dependency>
      <groupId>org.json</groupId>
      <artifactId>json</artifactId>
      <version>20231013</version>
  </dependency>
Requisições HTTP via HttpURLConnection / URI.

---

## 📦 Estrutura do Projeto
conversorMoedas/
 └── src/
     └── main/
         └── java/
             └── org/
                 └── example/
                     ├── ConversorMoedas.java
                     ├── RequisicaoAPI.java
                     └── Util.java
 └── pom.xml

---

## 🔧 Como Executar
1. Certifique-se de ter o Java 17+ instalado
java -version

2. Compile o projeto com Maven
mvn clean package

3. Execute o programa
mvn exec:java -Dexec.mainClass="org.example.ConversorMoedas"


Ou diretamente pelo .jar:

java -jar target/conversorMoedas.jar

---

## 🌐 Configuração da API

A aplicação usa um endpoint público de câmbio (editável dentro da classe RequisicaoAPI):

private static final String API_URL = "https://api.exchangerate-api.com/v4/latest/";


Você pode substituir por qualquer outra API compatível.

---

## 📚 Exemplo de Uso

Informe a moeda de origem (ex: USD).

Informe a moeda de destino (ex: BRL).

Informe o valor a ser convertido.

O sistema exibirá o valor convertido usando as taxas atualizadas.

---

## 🛠️ Melhorias Futuras

Interface gráfica (JavaFX ou Swing)

Suporte a histórico de conversões

Integração com múltiplas APIs

Cache de taxas para reduzir chamadas

---

## 📄 Licença

Este projeto é de uso livre para estudos e modificações.

---

## ✨ Autor

Desenvolvido como parte de estudos em Java e APIs REST.
