<?php

require 'db.php';

$db = new Database();
$data = $db->getAll('outlet');

foreach($data as $d):
?>
    <p><?= $d['id_outlet']; ?></p>
    <p><?= $d['nama']; ?></p>
    <p><?= $d['alamat']; ?></p>
    <p><?= $d['tlp']; ?></p>
    <hr>
<?php endforeach; ?>