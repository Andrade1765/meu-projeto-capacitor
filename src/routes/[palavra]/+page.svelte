<script>
    let palavras = [
      { termo: "Abraço", definicao: "Ato de envolver alguém com os braços, geralmente como demonstração de afeto." },
      { termo: "Afeto", definicao: "Sentimento de carinho ou amor." },
      { termo: "Amanhecer", definicao: "O nascer do sol; o início do dia." },
      { termo: "Amizade", definicao: "Relação de carinho e afeto entre pessoas." },
      { termo: "Aroma", definicao: "Odor agradável." },
      { termo: "Aurora", definicao: "Primeiro orvalho do dia; começo de algo." },
      { termo: "Beleza", definicao: "Qualidade que agrada os sentidos ou a mente." },
      { termo: "Bênção", definicao: "Ato de abençoar; graça divina." },
      { termo: "Biblioteca", definicao: "Um conjunto de funções e recursos pré-escritos para uso em software." },
      { termo: "Bolo", definicao: "Alimento doce, geralmente assado, feito com massa à base de farinha, ovos, açúcar e outros ingredientes, e frequentemente coberto com glacê ou recheio." },
      { termo: "Borboleta", definicao: "Inseto com asas grandes e coloridas." },
      { termo: "Brisa", definicao: "Vento leve e suave." },
      { termo: "Cachoeira", definicao: "Queda d'água natural." },
      { termo: "Caminho", definicao: "Rota ou trilha a ser seguida." },
      { termo: "Canto", definicao: "Ato de cantar; melodia." },
      { termo: "Céu", definicao: "Espaço acima da Terra, onde se veem as nuvens e as estrelas." },
      { termo: "Chuva", definicao: "Precipitação de água em gotas da atmosfera." },
      { termo: "Coragem", definicao: "Força moral para enfrentar o perigo ou o medo." },
      { termo: "Dança", definicao: "Movimento rítmico do corpo." },
      { termo: "Deleite", definicao: "Grande prazer ou satisfação." },
      { termo: "Doce", definicao: "Alimento com sabor açucarado." },
      { termo: "Doçura", definicao: "Qualidade de ser doce ou gentil." },
      { termo: "Elegância", definicao: "Qualidade de ser gracioso e estiloso." },
      { termo: "Esperança", definicao: "Sentimento de expectativa e desejo de algo positivo." },
      { termo: "Espelho", definicao: "Superfície que reflete imagens." },
      { termo: "Estrela", definicao: "Corpo celeste que brilha com luz própria." },
      { termo: "Fantasia", definicao: "Imagem criada pela imaginação." },
      { termo: "Felicidade", definicao: "Estado de bem-estar e contentamento." },
      { termo: "Flor", definicao: "Parte reprodutiva de uma planta comumente colorida." },
      { termo: "Fruto", definicao: "Produto comestível de uma planta." },
      { termo: "Gargalhada", definicao: "Risada alta e prolongada." },
      { termo: "Gentileza", definicao: "Qualidade de ser gentil, amável." },
      { termo: "Gesto", definicao: "Movimento do corpo ou das mãos para expressar algo." },
      { termo: "Gratidão", definicao: "Sentimento de agradecimento." },
      { termo: "Harmonia", definicao: "Combinação agradável de elementos." },
      { termo: "História", definicao: "Narrativa de eventos passados." },
      { termo: "Horizonte", definicao: "Linha onde o céu parece encontrar a terra ou o mar." },
      { termo: "Imaginação", definicao: "Capacidade de formar novas ideias e imagens na mente." },
      { termo: "Inspiração", definicao: "Estímulo criativo." },
      { termo: "Intuição", definicao: "Capacidade de compreender algo sem a necessidade de raciocínio." },
      { termo: "Inverno", definicao: "Estação do ano mais fria." },
      { termo: "Janela", definicao: "Abertura em uma parede para permitir a entrada de luz e ar." },
      { termo: "Jardim", definicao: "Área cultivada com plantas e flores." },
      { termo: "Jóia", definicao: "Objeto de valor usado como adorno." },
      { termo: "Lago", definicao: "Grande massa de água doce rodeada por terra." },
      { termo: "Leitura", definicao: "Ato de decifrar e compreender um texto." },
      { termo: "Liberdade", definicao: "Estado de não estar preso ou restrito." },
      { termo: "Lua", definicao: "Satélite natural da Terra." },
      { termo: "Luz", definicao: "Energia eletromagnética que torna as coisas visíveis." },
      { termo: "Mar", definicao: "Grande extensão de água salgada." },
      { termo: "Melodia", definicao: "Sequência de notas musicais que formam um tema." },
      { termo: "Memória", definicao: "Capacidade de reter e recordar informações." },
      { termo: "Música", definicao: "Arte de combinar sons de forma agradável." },
      { termo: "Natureza", definicao: "O mundo físico e seus fenômenos." },
      { termo: "Ninho", definicao: "Construção feita por aves para seus ovos." },
      { termo: "Nostalgia", definicao: "Saudade de algo ou alguém do passado." },
      { termo: "Nuvem", definicao: "Massa visível de gotículas de água suspensas na atmosfera." },
      { termo: "Oceano", definicao: "Grande massa de água salgada que cobre grande parte da Terra." },
      { termo: "Ondas", definicao: "Movimento da água do mar." },
      { termo: "Oração", definicao: "Pedido ou súplica a uma divindade." },
      { termo: "Ouro", definicao: "Metal precioso, amarelo e brilhante." },
      { termo: "Pão", definicao: "Alimento básico feito de farinha (geralmente de trigo), água e levedura, amassado e assado." },
      { termo: "Pássaro", definicao: "Animal vertebrado com penas e asas, capaz de voar." },
      { termo: "Paz", definicao: "Estado de tranquilidade e ausência de conflitos." },
      { termo: "Pintura", definicao: "Obra de arte feita com tintas." },
      { termo: "Poesia", definicao: "Arte de expressar ideias e emoções em versos." },
      { termo: "Prédio", definicao: "Edificação de vários andares destinada a habitação, escritórios ou outros fins." },
      { termo: "Quadrinho", definicao: "Sequência de desenhos que contam uma história." },
      { termo: "Quimera", definicao: "Criatura mitológica imaginária; ilusão." },
      { termo: "Quietude", definicao: "Estado de calma e silêncio." },
      { termo: "Refúgio", definicao: "Lugar que oferece proteção ou abrigo." },
      { termo: "Rio", definicao: "Curso de água natural que flui para um oceano, lago ou outro rio." },
      { termo: "Risada", definicao: "Som de alegria e divertimento." },
      { termo: "Romance", definicao: "Gênero literário narrativo extenso." },
      { termo: "Sabedoria", definicao: "Conhecimento profundo e experiência." },
      { termo: "Silêncio", definicao: "Ausência de som." },
      { termo: "Sol", definicao: "Estrela central do nosso sistema planetário." },
      { termo: "Sonho", definicao: "Sucessão de imagens, ideias e emoções que ocorrem durante o sono." },
      { termo: "Tempestade", definicao: "Fenômeno meteorológico caracterizado por ventos fortes e chuva intensa." },
      { termo: "Ternura", definicao: "Sentimento de carinho e afeto." },
      { termo: "Terra", definicao: "Planeta em que vivemos." },
      { termo: "Tranquilidade", definicao: "Estado de calma e serenidade." },
      { termo: "União", definicao: "Ato de juntar ou combinar." },
      { termo: "Universo", definicao: "A totalidade de toda a matéria, energia, planetas e estrelas." },
      { termo: "Utopia", definicao: "Lugar ou estado ideal, mas irrealizável." },
      { termo: "Vagalume", definicao: "Inseto que emite luz." },
      { termo: "Vento", definicao: "Movimento do ar na atmosfera." },
      { termo: "Viagem", definicao: "Deslocamento de um lugar para outro." },
      { termo: "Voz", definicao: "Som produzido pelas cordas vocais." },
      { termo: "Walkman", definicao: "Antigo aparelho portátil para ouvir música." },
      { termo: "Whisky", definicao: "Bebida alcoólica destilada." },
      { termo: "Xadrez", definicao: "Jogo de tabuleiro estratégico." },
      { termo: "Xerife", definicao: "Oficial de polícia em algumas regiões." },
      { termo: "Xícara", definicao: "Pequeno recipiente com alça para beber líquidos." },
      { termo: "Xilofone", definicao: "Instrumento musical de percussão." },
      { termo: "Yacht", definicao: "Barco de luxo para lazer." },
      { termo: "Yoga", definicao: "Prática física, mental e espiritual." },
      { termo: "Yogurte", definicao: "Alimento lácteo fermentado." },
      { termo: "Zelo", definicao: "Grande dedicação e cuidado." },
      { termo: "Ziguezague", definicao: "Trajeto em forma de 'Z'." },
      { termo: "Zumbido", definicao: "Som contínuo e monótono." },
    ];
    
      let termoPesquisado = '';
    
      $: termosFiltrados = palavras.filter(palavra => palavra.termo.toLowerCase().includes(termoPesquisado.toLowerCase()));
    </script>
    
    <style>
      main {
        font-family: sans-serif;
        max-width: 800px;
        margin: 20px auto;
        padding: 20px;
        border: 1px solid #eee;
        border-radius: 8px;
        box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      }
      h1 {
        text-align: center;
        color: #333;
      }
      input {
        width: calc(100% - 20px);
        padding: 10px;
        margin-bottom: 20px;
        border: 1px solid #ddd;
        border-radius: 4px;
        font-size: 16px;
      }
      .termo {
        margin-bottom: 15px;
        padding: 10px;
        border: 1px solid #e0e0e0;
        border-radius: 6px;
        background-color: #f9f9f9;
      }
      .termo h2 {
        margin-top: 0;
        color: #007bff;
        font-size: 1.2em;
      }
      .termo p {
        margin-bottom: 0;
        color: #555;
        line-height: 1.5;
      }
      .no-results {
        text-align: center;
        color: #777;
        padding: 20px;
      }
    </style>
    
    <main>
      <h1>Dicionário de Termos de Desenvolvimento</h1>
    
      <input
        type="text"
        bind:value={termoPesquisado}
        placeholder="Pesquise por um termo..."
      />
    
      {#if termosFiltrados.length > 0}
        {#each termosFiltrados as palavra}
          <div class="termo">
            <h2>{palavra.termo}</h2>
            <p>{palavra.definicao}</p>
          </div>
        {/each}
      {:else}
        <p class="no-results">Nenhum termo encontrado para "{termoPesquisado}".</p>
      {/if}
    </main>    