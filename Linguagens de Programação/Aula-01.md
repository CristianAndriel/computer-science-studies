# 📚 AULA 001: Programação Orientada a Objetos

---

## 🎯 CONCEITOS FUNDAMENTAIS APRENDIDOS

### 1. **ESTRUTURA BÁSICA DE UMA CLASSE JAVA**
```java
public class NomeDaClasse {
    // Atributos (variáveis)
    // Métodos (funções)
}
```

### 2. **ATRIBUTOS E TIPOS DE DADOS**
```java
private String nome;           // Texto
private int idade;             // Número inteiro
private boolean ativo;         // Verdadeiro ou falso
private double poder;          // Número decimal
```

### 3. **ENCAPSULAMENTO BÁSICO**
- **private**: Atributos não podem ser acessados diretamente de fora da classe
- **public**: Métodos podem ser chamados de qualquer lugar

---

## 🔧 GETTERS E SETTERS

### **Setter (Definir valores):**
```java
public void setNome(String nome, String estilo, String nivel, int idade, boolean marca) {
    this.nome = nome;           // this.nome = atributo da classe
    this.estiloRespiracao = estilo;
    this.nivel = nivel;
    this.idade = idade;
    this.marcaDoCacador = marca;
}
```

### **Getters (Obter valores):**
```java
public String getNome() {
    return nome;
}

public String getEstiloRespiracao() {
    return estiloRespiracao;
}
```

**Por que usar getters/setters?**
- Controle de acesso aos dados
- Validação de dados
- Manutenção do código
- Padrão profissional em Java

---

## 🏗️ HERANÇA (INHERITANCE)

### **Classe Pai (Superclasse):**
```java
public class Cacadores {
    // Atributos e métodos comuns a todos os caçadores
    private String nome;
    private String estiloRespiracao;
    // ... outros atributos
}
```

### **Classe Filha (Subclasse):**
```java
public class Hashiras extends Cacadores {
    // Hashiras herda tudo de Cacadores
    // E pode ter atributos/métodos específicos
    boolean derrotouLuaSuperior;
    String luaSuperiorDerrotada;
}
```

**O que significa `extends`?**
- A classe filha herda todos os atributos e métodos da classe pai
- Pode usar métodos como `getNome()`, `getEstiloRespiracao()`
- Pode sobrescrever métodos para comportamentos específicos

---

## 📝 MÉTODOS

### **Método Principal (Main):**
```java
public static void main(String[] args) {
    // Código que executa quando o programa inicia
    // Ponto de entrada da aplicação
}
```

### **Métodos Personalizados:**
```java
public void informacoesCacador() {
    System.out.println("Nome: " + nome);
    System.out.println("Idade: " + idade);
    // ... outras informações
}
```

---

## 🎮 EXEMPLO PRÁTICO IMPLEMENTADO

### **Criação de Objetos:**
```java
// Criando um caçador básico
Cacadores cacador = new Cacadores();
cacador.setNome("Tanjiro Kamado", "Água", "Kanoe", 14, true);

// Criando um hashira
Hashiras hashira = new Hashiras();
hashira.setNome("Giyu Tomioka", "Água", "Hashira", 21, false);
```

### **Uso de Métodos:**
```java
// Chamando métodos da classe pai
cacador.informacoesCacador();
hashira.informacoesCacador();  // Herda da classe Cacadores

// Chamando métodos específicos da classe filha
hashira.mostrarStatusHashira();
```

---

## 🚀 COMO EXECUTAR O PROGRAMA

### **1. Compilar:**
```bash
javac *.java
```

### **2. Executar:**
```bash
java Main
```

---

## 📋 CONVENÇÕES DE NOMENCLATURA EM JAVA

### **Classes:**
- ✅ **Correto:** `Cacadores`, `Hashiras`
- ❌ **Incorreto:** `cacadores`, `hashiras`

### **Variáveis e Objetos:**
- ✅ **Correto:** `cacador`, `hashira`
- ❌ **Incorreto:** `Cacador`, `Hashira`

### **Métodos:**
- ✅ **Correto:** `informacoesCacador()`, `mostrarStatusHashira()`
- ❌ **Incorreto:** `InformacoesCacador()`, `MostrarStatusHashira()`

---

## 🎯 PRÓXIMOS PASSOS (AULA 002)

### **1. POLIMORFISMO**
- Métodos com mesmo nome, comportamentos diferentes
- Uso da palavra-chave `@Override`

### **2. CONSTRUTORES**
- Criação de objetos de forma mais elegante
- Inicialização automática de atributos

### **3. ENCAPSULAMENTO AVANÇADO**
- Proteção de dados
- Validação de entrada

---

## 💡 DICAS IMPORTANTES

### **Boas Práticas:**
- Sempre use `private` para atributos
- Use getters e setters para acesso aos dados
- Nomes descritivos para classes e métodos
- Comentários explicativos no código

### **Estrutura de Arquivos:**
```
src/
├── Main.java           // Classe principal
├── Cacadores.java      // Classe base
└── Hashiras.java       // Classe que herda
```

---

## 🔍 CONCEITOS-CHAVE PARA REVISAR

- **Classe:** Modelo/template para criar objetos
- **Objeto:** Instância de uma classe
- **Atributo:** Características/propriedades
- **Método:** Ações/comportamentos
- **Herança:** Reutilização de código entre classes
- **Encapsulamento:** Proteção e controle de acesso aos dados

---

## 📚 RECURSOS ADICIONAIS

- **Documentação Oracle Java:** https://docs.oracle.com/javase/
- **Tutorial Java:** https://docs.oracle.com/javase/tutorial/
- **IntelliJ IDEA:** IDE recomendada para desenvolvimento Java

---

**🎉 Parabéns pelo progresso! Você está no caminho certo para se tornar um desenvolvedor Java!**

*Última atualização: Aula 001 - Conceitos Básicos de Java*
