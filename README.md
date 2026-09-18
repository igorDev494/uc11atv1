#  Nome do Projeto

Leilões TDS - Atividade 1 - UC11

## Explicação do Projeto

Projeto feito em Java, utilizando Banco de Dados MySQL para treinar o versionamento local e remoto.

## Tecnologias Utilizadas

- Java
- MySQL

## Exemplo de Codigo de Conexão

```java
public class conectaDAO {
    
    public Connection connectDB(){
        Connection conn = null
        try {
            conn = DriverManager.getConnection("jdbc:mysql://localhost/uc11?user=root&password="); 
        } catch (SQLException erro){
            JOptionPane.showMessageDialog(null, "Erro ConectaDAO" + erro.getMessage());
        }
        return conn;
    }
}
```
