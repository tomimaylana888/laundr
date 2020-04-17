<?php 

include 'db.php';

$db = new Database();
$insert = $db->insert('outlet', [
    'id_outlet' =>'',
    'nama'      =>'Cabang baru pabuaran',
    'alamat'    =>'Pabuaran',
    'tlp'       =>'08312456992'
]);

if ( $insert > 0) {
    echo"Berhasil menambahkan data!";
} else {
    echo "Gagal menambahkan data".mysqli_error($db->connect());
}





// $data =$db->getAll('outlet');

// foreach($data as $d):
//     echo $d['id_outlet'];
//     echo "<br>";
//     echo $d['nama'];
//     echo "<br>";
//     echo $d['alamat'];
//     echo "<br>";
//     echo $d['tlp'];
//     echo "<br>";
//     echo "<hr>";
// endforeach;
