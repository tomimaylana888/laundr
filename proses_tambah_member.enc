<?php 

include 'db.php';

$nama           =$_POST['nama'];
$alamat         =$_POST['alamat'];
$jenis_kelamin  =$_POST['jenis_kelamin'];
$tlp            =$_POST['tlp'];


$db = new Database();
$insert = $db->insert('member', [
    'id_outlet'     => '',
    'nama'          =>$nama,
    'alamat'        =>$alamat,
    'jenis_kelamin' =>$jenis_kelamin,
    'tlp'           =>$tlp
]);

if ( $insert > 0) {
    header('Location:halaman_member.php');
} else {
    echo "Gagal menambahkan data".mysqli_error($db->connect());
}


