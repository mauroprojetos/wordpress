Precisei ustilizar as fun��es do wordpress para conex�o e manipula��o de BD stand alone 

Alterei o arquivo wp-db.php para carregar as fun��es basicas e n�o depender de outros arquivos


<?php
DEFINE('WP_DEBUG',false);
$wp_version ="";
require_once("wp-db.php");

$wpdb = new wpdb('root', 'password', 'BD', 'localhost');

?>