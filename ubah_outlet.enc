<?php

require 'db.php';

$id_outlet  =$_POST['id_outlet'];
$nama       =$_POST['nama'];
$alamat     =$_POST['alamat'];
$tlp        =$_POST['tlp'];

$db = new Database();
$update = $db->update('outlet',[
    'nama'      => $nama,
    'alamat'    => $alamat,
    'tlp'       => $tlp
], ['id_outlet' => $id_outlet]);

if ( $update > 0 ) {
    header('Location:halaman_outlet.php');
} else {
    echo mysqli_error($db->connect());
}