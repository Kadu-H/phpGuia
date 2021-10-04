<h1> phpGuia </h1>
<h2>Um guia importante sobre php</h2>
<h3>Esse repositorio serve como um um salvamento de informações necessarias sobre a lingagem php se você tem algo à adicionar adicione.</h3>
<br>
<h2>🦾Ligação do banco de dados ao php</h2> Se você usa php e banco de dados provavelmente ja estabeleceu uma conexão ao banco de dados utilizando php<br>Se você é inciante em desenvolvimento de sites, e ainda não sabe estabelecer uma conexão ao banco de dados com php, este artigo vai mostrar as maneiras mais fáceis de fazer isso.<br> <h3>1º Alternativa</h3><br>

"$conn = mysqli_connect('Nome do servidor','Usuario','Senha do banco','Nome do banco de dados');" &nbsp; &nbsp; //estabelece uma conexão com o banco de dados <br>
"mysqli_close($conn);" &nbsp; &nbsp; //fecha essa conexão <br><br>
Esse é o comando simplificado (sem as aspas).
<br>
<h3>2º Alternativa</h3><br>
//Declara as variaveis <br>
$servername = "Nome do servidor";  <br>
$database = "Nome do banco"; <br>
$username = "Usuario"; <br>
$password = "Senha do banco"; <br>


$conn = mysqli_connect($servername, $username, $password, $database); &nbsp; &nbsp; //Cria conexão <br>
if (!$conn) { &nbsp; &nbsp; //Se tiver erro exibe o erro <br>
    die("Falhou erro: " . mysqli_connect_error()); <br>
} <br>
echo "Conectado"; &nbsp; &nbsp; //Confirma se esta conectado  <br>
mysqli_close($conn); &nbsp; &nbsp; //fecha essa conexão <br>
Esse é o comando mais avançado mas com mais segurança de modificações futuras. <br>
<h3>"🦾Ligação do banco de dados ao php" Finalizada.</h3>
