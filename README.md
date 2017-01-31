Precisei ustilizar as funções do wordpress para conexão e manipulação de BD stand alone 

Alterei o arquivo wp-db.php para carregar as funções basicas e não depender de outros arquivos

```php
<?php
DEFINE('WP_DEBUG',false);
$wp_version ="";
require_once("wp-db.php");
$wpdb = new wpdb('root', 'password', 'BD', 'localhost');
?>
```

