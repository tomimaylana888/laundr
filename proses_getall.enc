<?php

require 'db.php';

$db = new Database();
$data = $db->getAll('member');

foreach($data as $d):
?>
    <p><?= $d['id_member']; ?></p>
    <p><?= $d['nama']; ?></p>
    <p><?= $d['alamat']; ?></p>
    <p><?= $d['jenis_kelamin']; ?></p>
    <p><?= $d['tlp']; ?></p>
    <hr>
<?php endforeach; ?>