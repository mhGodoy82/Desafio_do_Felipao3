class Heroi {
    constructor(nome, idade, tipo) {
      this.nome = nome;
      this.idade = idade;
      this.tipo = tipo.toLowerCase();
    }
  
    atacar() {
      let ataque;
  
      switch (this.tipo) {
        case "mago":
          ataque = "magia";
          break;
        case "guerreiro":
          ataque = "espada";
          break;
        case "monge":
          ataque = "artes marciais";
          break;
        case "ninja":
          ataque = "shuriken";
          break;
        default:
          ataque = "ataque desconhecido";
      }
  
      console.log(`${this.nome}, o ${this.tipo}, atacou usando ${ataque}`);
    }
  }
  
  
  const heroi1 = new Heroi("Ze Gotinhas", 30, "guerreiro");
  const heroi2 = new Heroi("Chaves", 201, "mago");
  const heroi3 = new Heroi("Kiko", 25, "monge");
  const heroi4 = new Heroi("Seu Madriga", 17, "ninja");
  
  heroi1.atacar();
  heroi2.atacar();
  heroi3.atacar();
  heroi4.atacar();
