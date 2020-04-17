<?php 

include 'db.php';

$nama=$_POST['nama'];
$alamat=$_POST['alamat'];
$tlp=$_POST['tlp'];


$db = new Database();
$insert = $db->insert('outlet', [
    'id_outlet' => '',
    'nama'      =>$nama,
    'alamat'    =>$alamat,
    'tlp'       =>$tlp
]);

if ( $insert > 0) {
    header('Location:halaman_outlet.php');
} else {
    echo "Gagal menambahkan data".mysqli_error($db->connect());
}


