<?php

include 'koneksi.php';

$nama       =$_POST['nama'];
$username   =$_POST['username'];
$email      =$_POST['email'];
$password   =$_POST['password'];

$hashed_password= password_hash($password, PASSWORD_DEFAULT);

$query = mysqli_query($koneksi, "INSERT INTO register VALUES ('','$nama','$username','$email','$hashed_password')");

if ($query == TRUE){
    header('Location: login.php');
} else {
    echo "Terjadi kesalahan saat mendaftar!".mysqli_error($koneksi);

    echo "Silahkan daftar kembali <a href='login.php'>disini</a>";
}
        