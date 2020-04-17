<?php

require 'db.php';

$id_member      =$_POST['id_member'];
$nama           =$_POST['nama'];
$alamat         =$_POST['alamat'];
$jenis_kelamin  =$_POST['jenis_kelamin'];
$tlp            =$_POST['tlp'];

$db = new Database();
$update = $db->update('member',[
    'nama'          => $nama,
    'alamat'        => $alamat,
    'jenis_kelamin' => $jenis_kelamin,
    'tlp'           => $tlp
], ['id_member'     => $id_member]);

if ( $update > 0 ) {
    header('Location:halaman_member.php');
} else {
    echo mysqli_error($db->connect());
}