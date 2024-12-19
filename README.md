# Classes-de-um-jogo

class Heroi {
    constructor(nome, idade, tipo) {
      this.nome = nome;
      this.idade = idade;
      this.tipo = tipo;
    }
  
    atacar() {
      let ataque = "";
      switch (this.tipo) {
        case "mago":
          ataque = "usou magia";
          break;
        case "guerreiro":
          ataque = "usou espada";
          break;
        case "monge":
          ataque = "usou artes marciais";
          break;
        case "ninja":
          ataque = "usou shuriken";
          break;
        default:
          ataque = "usou um ataque desconhecido"; //Tratamento para tipos não definidos
      }
  
      console.log(`o ${this.tipo} atacou e ${ataque}`);
    }

    
  }

    
   
  
  
  const mago = new Heroi("Jackson", 40, "mago");
  const guerreiro = new Heroi("Joel", 30, "guerreiro");
  const monge = new Heroi("Felipe", 45, "monge");
  const ninja = new Heroi("Jose", 38, "ninja");
 
  
  mago.atacar();      
  guerreiro.atacar() 
  monge.atacar();
  ninja.atacar();    

