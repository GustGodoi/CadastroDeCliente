# CadastroDeCliente
package cadastrocliente;

import modelo.Cliente;

public class CadastroCliente {

    public static void main(String[] args) {

        Cliente cli = new Cliente();

        cli.codigo = 10;
        cli.nome = "Marcos";
        cli.cpf = "088.542.123-01";
        cli.email = "marcos@étois";
        cli.endereco = "Av. 1° de maio";
        cli.cep = 88352490;
        cli.telefone = "33504226";
        cli.aposentado = false;
        
        
        //Array  de clientes
        Cliente[] listaDeClientes = new Cliente[3];
        listaDeClientes[0] = cli;
        
        cli = new Cliente();
        cli.nome = "Gustavo";
        cli.cpf = "015.263.458-52";
        listaDeClientes[1] = cli;
        
        cli = new Cliente();
        cli.nome = "Linda";
        cli.cpf = "154.892.644-03";
        listaDeClientes[2] = cli;
        
        
        for (int i = 0; i < listaDeClientes.length; i++) {
            cli = listaDeClientes[i];
            
            System.out.println("nome: "+cli.nome);
            System.out.println("CPF: "+cli.cpf);
            System.out.println("");
            
        }
        
    }

}

\\CLIENTE

package modelo;
public class Cliente {
    
    public int cep;
    public String nome;
    public String cpf;
    public String telefone;
    public String email;
    public String endereco;
    public int codigo;
    public boolean aposentado;
    
}
